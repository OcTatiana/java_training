# Name

+ [Problem 2](#problem-2)

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