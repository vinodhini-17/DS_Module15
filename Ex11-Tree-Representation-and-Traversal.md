# Ex11 Tree Representation and Traversal
## DATE : 26.04.2025
## AIM:
To write a C function to perform post order traversal of a binary tree.

## Algorithm
1. Start and define display_postorder(root_node).
2. If root_node is not null, recursively call left and right children.
3. After both calls, print the current node’s value.
4. End.

## Program:
```
/*
Program to perform post order traversal of a binary tree.
Developed by: vinodhini k
RegisterNumber:  212223230245
*/
/*struct node
{
int value;
struct node*left_child, *right_child;
};*/
void display_postorder(struct node*root_node){
if(root_node)
{
display_postorder(root_node->left_child);
display_postorder(root_node->right_child);
printf("%d\n",root_node->value);
}
}

```

## Output:

![image](https://github.com/user-attachments/assets/5014bff7-1df7-4065-8335-b1bc587e64b1)


## Result:
Thus, the function to perform post order traversal of a binary tree is implemented successfully
