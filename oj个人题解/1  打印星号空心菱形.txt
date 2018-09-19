#include<stdio.h>
int main()
{
    int i,j,n,count,temp;
    scanf("%d",&n);
    for(i=(n-1)/2,j=1,temp=0;j<=n+1;j=j+2,i--,temp++)
    {
        for(count=0;count<i;count++)
        printf(" ");
        printf("*");
        for(count=2;count<j;count++)
        printf(" ");
        if (temp>=1)
        printf("*");
        printf("\n");
    }
    for(j=j-4,i=i+2,temp=0;j>=1;j=j-2,i++,temp++)
    {
        for(count=0;count<i;count++)
        printf(" ");
        printf("*");
        for(count=2;count<j;count++)
        printf(" ");
        if (count>2)
        printf("*");
        printf("\n");
    }
    return 0;
}
