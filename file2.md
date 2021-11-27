# Name

+ [Problem 3](#problem-3)

## Problem 3

link3

``` java
private ListNode middleNode(ListNode head) {
    ListNode slowPointer = head;
    ListNode fastPointer = head;

    while (fastPointer != null && fastPointer.next != null) {
        slowPointer = slowPointer.next;
        fastPointer = fastPointer.next.next;
    }

    return slowPointer;
}
```