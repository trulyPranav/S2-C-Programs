## Code:
```c
#include<stdio.h>

void main(){
    int a[100][100],i=0,j=0,r=0,c=0,sum=0;
    printf("Enter the row and column size:");
    scanf("%d %d",&r,&c);
    printf("Enter the elements of the Matrix:");
    for(i=0;i<r;i++){
        for(j=0;j<c;j++){
            scanf("%d",&a[i][j]);
        }
    }
    printf("Matrix:\n");
    for(i=0;i<r;i++){
        for(j=0;j<c;j++){
            printf("%d\t",a[i][j]);
        }
        printf("\n");
    }
    for(i=0;i<r;i++){
         for(j=0;j<c;j++){
             if(i==j){
                 sum += a[i][j];
             }
         }
     }
    printf("Sum of diagonal elements = %d",sum);
}
```

## Algorithm:
> Will be updated