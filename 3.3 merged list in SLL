#include <stdio.h>
#include <stdlib.h>
struct ListNode {
    int val;
    struct ListNode* next;
};
struct ListNode* mergeTwoLists(struct ListNode* l1, struct ListNode* l2) {
    struct ListNode dummy;
    struct ListNode* tail = &dummy;
    dummy.next = NULL;
    while (l1 != NULL && l2 != NULL) {
        if (l1->val < l2->val) {
            tail->next = l1;
            l1 = l1->next;
        } else {
            tail->next = l2;
            l2 = l2->next;
        }
        tail = tail->next;
    }
    if (l1 != NULL) {
        tail->next = l1;
    } else {
        tail->next = l2;
    }
    return dummy.next;
}
void printList(struct ListNode* head) {
    while (head != NULL) {
        printf("%d -> ", head->val);
        head = head->next;
    }
    printf("NULL\n");
}
struct ListNode* newNode(int val) {
    struct ListNode* node = (struct ListNode*)malloc(sizeof(struct ListNode));
    node->val = val;
    node->next = NULL;
    return node;
}

int main() {
    struct ListNode* l1 = newNode(1);
    l1->next = newNode(3);
    l1->next->next = newNode(5);

    struct ListNode* l2 = newNode(2);
    l2->next = newNode(4);
    l2->next->next = newNode(6);
    struct ListNode* mergedList = mergeTwoLists(l1, l2);
    printf("vijayalakshmi G ,192321080\n");
    printf("Merged List: ");
    printList(mergedList);
    free(l1);
    free(l2);

    return 0;
}
