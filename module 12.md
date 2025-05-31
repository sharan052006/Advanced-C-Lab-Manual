## NAME: Sharan I
## REG NO: 212224040308
## EXP NO 26: C PROGRAM TO DISPLAY STACK ELEMENTS USING LINKED LIST.

## Aim:
To write a C program to display stack elements using linked list.

## Algorithm:
1.	Define a structure Node with two members: data to store the integer value and next to point to the next node in the linked list.
2.	Declare a global variable head representing the starting node of the linked list.
3.	Define a function display to print the elements of the linked list.
4.	Declare a pointer p and initialize it with the head of the linked list.
5.	Use a while loop to traverse the linked list:
6.	Print the data of the current node.
7.	Move to the next node using the next pointer.
 
## Program:
```
struct Node
{
int data;
struct Node *next;
}*head;
void display()
{
struct Node *p; p=head; while(p!=NULL)
{
printf("%d\n",p->data); p=p->next;
}
}
```
## Output:

![437747541-3d86a971-1d51-4a42-a145-bbdcfed49d89](https://github.com/user-attachments/assets/8c94e342-c3ad-494a-ae91-82b6bceb5770)

## Result:
Thus, the program to display stack elements using linked list is verified successfully. 


## EXP.NO 27: C PROGRAM TO POP AN ELEMENT FROM THE GIVEN STACK USING LINKED LIST.

## Aim:
To write a C program to pop an element from the given stack using liked list.

## Algorithm:
1.	Check for Empty Stack
2.	If head is equal to NULL, Print "Stack is empty."
3.	Else Proceed to the next step.
4.	Set head to point to the next node in the stack.
 
## Program:
```
struct Node
{
int data;
struct Node *next;
}*head; void pop()
{
if(head==NULL)
{
printf("stack is empty");
}
else
{
head=head->next;
}
}
```
## Output:

![437747563-3d8b2780-a098-421c-908f-15ac1a7865d1](https://github.com/user-attachments/assets/8ed6c2b9-45f7-4fb7-b5b5-6396f2619f34)

## Result:
Thus, the program to pop an element from the given stack using liked list is verified successfully.

 
## EXP NO:28 C PROGRAM TO DISPLAY QUEUE ELEMENTS USING LINKED LIST.

## Aim:
To write a C program to display queue elements using linked list.

## Algorithm:
1.	Check if Queue is Empty
2.	Display Queue Elements
3.	Print the data of the current node pointed to by front
4.	Update front to point to the next node.
5.	End the display function.
 
## Program:
```
struct Node
{
char data;
struct Node *next;
}*front=NULL,*rear=NULL; void display()
{
if(front==NULL)
{
printf("queue is empty");
}
else
{
printf("queue elements:\n"); while(front!=NULL)
{
printf("%c\n",front->data); front=front->next;
}
}
}
```
## Output:

![437747572-fa16d58e-e382-4c83-8f9e-fb4fbbbc2e99](https://github.com/user-attachments/assets/322bb60d-9f5c-4a39-8b14-95e499ec4618)

## Result:
Thus, the program to display queue elements using linked list is verified successfully.


 
## EXP NO:29 C PROGRAM TO INSERT ELEMENTS IN QUEUE USING LINKED LIST

## Aim:
To write a C program to insert elements in queue using linked list.

## Algorithm:
1.	Allocate Memory for New Node
2.	Set Data and Next Pointer
3.	Check if Queue is Empty
4.	Set both front and rear to point to the new node p.
5.	Set the next pointer of the current rear to point to the new node p.
6.	End of Enqueue Operation
 
## Program:
```
struct Node
{
int data;
struct Node *next;
}*front=NULL,*rear=NULL; void enqueue(int data)
{
struct Node *p=(struct Node*)malloc(sizeof(struct Node)); p->data=data;
p->next=NULL; if(front==NULL)
{
front=rear=p;
}
else
{
rear->next=p; rear=p;
}
}
```
## Output:

![437747581-f2597c00-c947-4662-81cd-21a8e837a2e4](https://github.com/user-attachments/assets/1590bf29-4c76-4d72-aa93-1529ef6f6bc1)

## Result:
Thus, the program to insert elements in queue using linked list is verified successfully.



## EXP NO:30 C FUNCTION TO FIND THE PEEK OF QUEUE USING LINKED LIST.

## Aim:

The aim of this function is to retrieve the "peek" (the front element) of a queue implemented using a linked list

## Algorithm:

1.	Check if the queue is empty:
o	If the queue is empty (i.e., the front pointer is NULL), return an error or a message indicating that the queue is empty.
2.	Access the front element:
o	If the queue is not empty, return the data stored in the front node of the linked list (i.e., the element at the head of the queue).

## Program:
```
struct Node
{
   char data;
   struct Node *next;
}*front=NULL,*rear=NULL;
void peek()
{
    printf("%c",front->data);
}
```
## Output:

![437747589-51d7c4c0-b31c-411e-a799-abb8d6b034da](https://github.com/user-attachments/assets/d2b380dc-cf50-46bf-bc07-ff578efd6185)

## Result:

Thus, the program to retrieve the "peek" (the front element) of a queue implemented using a linked list is verified successfully.
