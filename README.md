#include <iostream>
#include <stdio.h>
using namespace std;

int main()
{
    int i,n,a[1000];
    int sum=0,temp=0;
    scanf("%d",&n);
    for(i=0;i<n;i++)
    {
        scanf("%d",&a[i]);
    }
    for(i=0;i<n;i++)
    {
        if(temp>0)
        {
            temp=temp+a[i];
        }
        else
        {
        temp=a[i];
        }
        if(temp>sum)
        {
            sum=temp;
        }
    }
    printf("%d",sum);
    return 0;
}
