# Ex12 Binary Search Tree
## DATE:
## AIM:
To write a C function to insert the elements in the binary search tree

## Algorithm
1. If the tree is empty, create a new node and return it as the root.
2. Compare the key to be inserted with the root node’s key.
3. If the key is smaller, recursively insert it into the left subtree.
4. If the key is larger, recursively insert it into the right subtree. 
5. Return the root node after insertion.  

## Program:
```
/*
Program to insert the elements in the binary search tree
Developed by: SWETHA S
RegisterNumber: 212222230155
*/
```
```
/*
/*struct node {
   int key;
   struct node *left, *right;
};*/
struct node* insert(struct node* node, int key) {
    if(node == NULL)
        return newNode(key);

    if(key < node->key)
        node->left = insert(node->left,key);
    else if(key > node->key)
        node->right = insert(node->right,key);
        
    return node;
    
    //type your code here
}
*/
```
## Output:
<img width="547" height="277" alt="image" src="https://github.com/user-attachments/assets/b74fb39a-1175-4bf3-a2bf-fbb3ba1f875e" />



## Result:
Thus, the C function to insert the elements in the binary search tree is implemented successfully.
