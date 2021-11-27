# Name

+ [Problem 1](#problem-1)

# Problem 1

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