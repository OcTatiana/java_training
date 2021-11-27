# Name

+ [Problem 1](#problem-1)
+ [Problem 2](#problem-2)
+ [Problem 3](#problem-3)

## Problem 1

link1

## Problem 2

link 2

``` java
private ListNode reverseList(ListNode head) {
    ListNode next = null;
    ListNode cur = head;
    ListNode prev = null;

    while (cur != null) {
        next = cur.next;
        cur.next = prev;
        prev = cur;
        cur = next;
    }
    return prev;
}
```

## Problem 3

link 3

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