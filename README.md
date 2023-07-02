# recursive-function
To generate fibonaccic series up to n terms using recursive function
#include<stdio.h>
#include<conio.h>
int fib(int n);
int main()
{
    int n,i;
    printf("enter number:\n");
    scanf("%d",&n);
    printf("\n fibonacci number u to %d terms\n",n);
    for(i=0;i<=n;i++)
    printf("%d\t",fib(i));
    return 0;
}
int fib(int n)
{
    if (n==0)
    return 0;
    if(n==1)
    return 1;
    else
    return fib(n-1)+fib(n-2);
}
