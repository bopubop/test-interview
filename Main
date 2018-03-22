public class Main {
    public static void main(String[] args) {

        Node<Integer> linkedListHead = new Node<>(1);
        linkedListHead
                .setNextNode(new Node<>(2))
                .setNextNode(new Node<>(3))
                .setNextNode(new Node<>(4));

        print(linkedListHead);
        System.out.println();
        print(reverse(linkedListHead));
    }

    private static void print(Node<Integer> head) {

        Node<Integer> curNode = head;
        while (curNode != null) {

            System.out.print(curNode.value);

            curNode = curNode.getNextNode();
            if (curNode != null) System.out.print("->");
        }
    }

    private static Node<Integer> reverse(Node<Integer> head) {

        Node<Integer> prev = null;
        Node<Integer> current = head;
        Node<Integer> next = null;
        while (current != null) {
            next = current.getNextNode();
            current.setNextNode( prev);
            prev = current;
            current = next;
        }
        head= prev;
        return head;
    }
}
