# Name

+ [Problem 1](#problem-1)
+ [Problem 2](#problem-2)
+ [Problem 3](#problem-3)

## Problem 1

link1

``` java
public boolean isPalindrome(ListNode head) {
    ListNode input = head;
    ListNode reverse = reverseList(middleNode(head));
    while (reverse != null) {
        if (input.val != reverse.val)
            return false;
        input = input.next;
        reverse = reverse.next;
    }
    return true;
}
```

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