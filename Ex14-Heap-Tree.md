# Ex14 Heap Tree
## DATE:
## AIM:
To write a C function to delete an element in a Heap Tree.

## Algorithm
1. Find the index of the element to be deleted.
2. Swap it with the last element in the heap.
3. Reduce the heap size by 1.
4. Heapify the tree from the root to maintain the heap property. 
5. Repeat until the heap property is restored.  

## Program:
```
/*
Program to delete an element in a Heap Tree
Developed by: SWETHA S
RegisterNumber: 212222230155
*/
```
```
/*
void deleteRoot(int array[], int num)
{
    int i;
    for(i=0;i<size;i++)
    {
        if(num==array[i])
        {
            break;
        }
    }
    swap(&array[i],&array[size-1]);
    size-=1;
    for(int i=size/2-1;i>=0;i--)
    {
        heapify(array,size,i);
    }
  // type your code here
}
*/
```
## Output:

<img width="1103" height="273" alt="image" src="https://github.com/user-attachments/assets/9a4012e3-721c-4b10-999e-bd44f6e3d952" />


## Result:
Thus, the function to delete an element in a Heap Tree is implemented successfully.
