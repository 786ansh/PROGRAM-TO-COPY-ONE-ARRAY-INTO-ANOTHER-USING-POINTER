# PROGRAM-TO-COPY-ONE-ARRAY-INTO-ANOTHER-USING-POINTER
#include<stdio.h>
int main()
{
    int n,i;
    scanf("%d",&n);
    int a[n], *p;
    p=a;
    for (int i=0;i<n;i++)
    scanf("%d",(p+i));
    for (int i=0;i<n;i++)
    printf("%d\t",*(p+i));
    int b[n],*q;
    q=b;
    for (int i=0;i<n;i++)
    //*(q+i)=*(p+i);
    scanf("%d",(q+i));
    for (int i=0;i<n;i++)
    printf(" elements of b=%d\t",*(q+i));
    
 int temp[n];
 
 for (int i=0;i<n;i++)
 {
     temp[n]=*(a+i);
     *(a+i)=*(b+i);
     *(b+i)=temp[n];
    printf("%d %d \t",*(a+i),*(b+i));
 }
 


    return 0;

}
