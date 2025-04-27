# Ex14 Heap Tree
## DATE : 26.04.2025
## AIM:
To write a C function to delete an element in a Heap Tree.

## Algorithm
1. Start and find the index of num in the array.
2. Swap num with the last element.
3. Decrease the array size by 1.
4. Heapify from the last non-leaf node (size/2 - 1) upwards.
5. End after restoring the heap property.
## Program:
```
/*
Program to delete an element in a Heap Tree
Developed by: VINODHINI K
RegisterNumber: 212223230245
*/
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
for(i=size/2-1;i>=0;i--)
{
heapify(array,size,i);
}
}
```

## Output:

![image](https://github.com/user-attachments/assets/a01e00f9-20da-43dd-b7b5-317be8229772)


## Result:
Thus, the function to delete an element in a Heap Tree is implemented successfully.
