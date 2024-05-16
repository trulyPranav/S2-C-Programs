## Code:
```c
#include<stdio.h>
int main()
{
    int a[100][100],i=0,j=0,r=0,c=0,sum=0;
    printf("Enter the row and column size:");
    scanf("%d%d",&r,&c);
    printf("Enter the array elements:");
    for(i=0;i<r;i++){
        for(j=0;j<c;j++)
        {
            scanf("%d",&a[i][j]);
        }
    }
        printf("Matrix:\n");
     for(i=0;i<r;i++){
        for(j=0;j<c;j++)
        {
            printf("%d\t",a[i][j]);
        }
        printf("\n");
     }
     for(i=0;i<r;i++){
         for(j=0;j<c;j++){
             if(i==j)
             {
                 sum=sum+a[i][j];
             }
         }
     }
     printf("Sum of diagonal elements=%d",sum);
    return 0;
}
```

## Algorithm:
#### will be updated