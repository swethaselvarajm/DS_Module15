# Ex11 Tree Representation and Traversal
## DATE:
## AIM:
To write a C function to perform post order traversal of a binary tree.

## Algorithm
1. Start from the root node of the binary tree.
2. Recursively traverse the left subtree in post-order.
3. Recursively traverse the right subtree in post-order.
4. Visit (print) the current node’s value. 
5. Repeat steps 2–4 until all nodes are visited.  

## Program:
```
/*
Program to perform post order traversal of a binary tree.
Developed by: SWETHA S
RegisterNumber:  212222230155
*/
```
```
/*
/*struct node
{
int value;
struct node *left_child, *right_child;
};*/
void display_postorder(struct node *root_node) {
    if(root_node)
    {
        display_postorder(root_node->left_child);
        display_postorder(root_node->right_child);
        printf("%d\n",root_node->value);
    }
    //write your code here
}
*/
```
## Output:

<img width="893" height="485" alt="image" src="https://github.com/user-attachments/assets/b9ec714b-6ea4-42a4-8a49-ca8266f0a238" />


## Result:
Thus, the function to perform post order traversal of a binary tree is implemented successfully
