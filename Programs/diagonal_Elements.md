## Code:
```c
#include<stdio.h>

void main(){
    int a[100][100],i=0,j=0,r=0,c=0;

    printf("Enter the row and column size:");
    scanf("%d %d",&r,&c);
    printf("Enter the elements of the Matrix:");
    // Reading the matrix
    for(i=0;i<r;i++){
        for(j=0;j<c;j++) {
            scanf("%d",&a[i][j]);
        }
    }
    printf("Matrix:\n"); // Printing the matrix user just inputted
    for(i=0;i<r;i++){
        for(j=0;j<c;j++){
            printf("%d\t",a[i][j]);
        }
        printf("\n");
    }
    printf("Diagonal Elements are:");
    for(i=0;i<r;i++){
        for(j=0;j<c;j++){
            if(i==j) {// For diagonal elements,its row and column value will be same
                printf("%d\t",a[i][j]);// Diagonal Elements will be printed
            }
        }
    }
}
```
## Algorithm:
> will be updated