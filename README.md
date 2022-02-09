# reverse-a-string
#include <stdio.h>
char stack[100],top=-1;
void push(int k)
{
    stack[++top]=k;
}
char pop()
{
    return stack[top--];
}
void main()
{
    char a[20],l;
    int j,i=0;
    printf("enter a:");
    scanf("%s",a);
    while (a[i]!='\0')
    {
       push(a[i]);
       i++;
    }
    for (j=top;j>=0;j--)
    {
        printf("%c",pop());
    }
   
}
ot:
enter a:world
dlrow

