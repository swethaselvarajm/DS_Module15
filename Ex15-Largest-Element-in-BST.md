# Ex15 Largest Element in BST
## DATE: 
## AIM:
To Write a c program to find the largest value in a Binary Search Tree.

## Algorithm
1. Initialize a pointer to the root of the BST. 
2. Move to the right child in a loop while it exists. 
3. Stop when the right child is NULL. 
4. Return the current node’s value as the largest.

## Program:
```c
/*
Program to find and display the priority of the operator in the given Postfix expression
Developed by: SWETHA S
Register Number: 212222230155
*/

#include <stdio.h>
#include <stdlib.h>
struct node
{
    int info;
    struct node *left, *right;
};
struct node *createnode(int key)
{
    struct node *newnode = (struct node *)malloc(sizeof(struct node));
    newnode->info = key;
    newnode->left = NULL;
    newnode->right = NULL;
    return (newnode);
}
void inorder(struct node *root)
{
    if (root != NULL)
    {
        inorder(root->left);
        printf(" %d ", root->info);
        inorder(root->right);
    }
}
void largest(struct node *root)
{
    while (root != NULL && root->right != NULL)
    {
        root = root->right;
    }
    printf("\nLargest value is %d", root->info);
}
int main()
{
    /* Creating first Tree. */
    struct node *newnode = createnode(25);
    newnode->left = createnode(17);
    newnode->right = createnode(35);
    newnode->left->left = createnode(13);
    newnode->left->right = createnode(19);
    newnode->right->left = createnode(27);
    newnode->right->right = createnode(55);

    printf("Inorder traversal of tree 1 :");
    inorder(newnode);
    largest(newnode);

    return 0;
}
```

## Output:
<img width="834" height="97" alt="image" src="https://github.com/user-attachments/assets/4c3f7cdd-f632-4fc7-a98c-4cf6364730cc" />

## Result:
Thus, the C program to find the largest value in a Binary Search Tree is implemented successfully.
