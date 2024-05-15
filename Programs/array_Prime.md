## Code:
```c
#include<stdio.h>
int main()
{

    int a[10],i,flag=0,limit=0;
    printf("Enter limit");
    scanf("%d",&limit);

    printf("Enter the array elements:");
    for(i=0;i<limit;i++)
    {
        scanf("%d",&a[i]);
    }

    for(i=2;i<limit;i++)
    {
        if(a[i]%i==0)
        {
            flag=1;
             continue;
        }
       
    }
        if(flag==1)
        {
            printf("Elements are not Prime.");
        }
        else 
        {
            printf("Elements are Prime.");
        }
        return 0;
    }