# Ex13 Expression Tree
## DATE:
## AIM:
To write a C function to construct an Expression Tree for the given Postfix Expression and display the output in the format of In-order ,Pre-order and Post-order traversal.

## Algorithm
1. Read the postfix expression from input.
2. For each character in the postfix expression:
If it is an operand, create a node and push it onto a stack.
If it is an operator, pop two nodes from the stack, make them left and right children of a new node with the operator, and push this node back onto the stack.
3. The remaining node in the stack is the root of the Expression Tree.
4. Traverse the tree using In-order, Pre-order, and Post-order to display results.
  

## Program:
```
/*
Program to construct an Expression Tree for the given Postfix Expression and display the output in the format of In-order ,Pre-order and Post-order traversal.
Developed by: SWETHA S
RegisterNumber: 212222230155 
*/
```
```
/*
/*
struct n {
   char d;
   struct n *l;
   struct n *r;
};*/
void preOrder(struct n *tree) {
    if(tree)
    {
    printf("%c",tree->d);
    preOrder(tree->l);
    preOrder(tree->r);
    }
 // Type your code here
   
}
void inOrder(struct n *tree) {
    {
        if(tree)
        {
            inOrder(tree->l);
            printf("%c",tree->d);
            inOrder(tree->r);
        }
    }
  //type your code here
   
}
void postOrder(struct n *tree) {
    if(tree)
    {
        postOrder(tree->l);
        postOrder(tree->r);
        printf("%c",tree->d);
    }
  //type your code here 
}
*/
```
## Output:

<img width="380" height="266" alt="image" src="https://github.com/user-attachments/assets/84a2b7e0-49b9-4e37-9f55-aee4c0011428" />


## Result:
Thus, the C program to display the Expression Tree in the format of In-order ,Pre-order and Post-order traversal.
