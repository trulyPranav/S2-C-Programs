## Code:
```c
#include <stdio.h>

void main(){
    int a[100][100],b[100][100],m[100][100],r1,r2,c1,c2,i,j,k;

    printf("Enter the Row and Column of the First Matrix:");
    scanf("%d %d",&r1,&c1);
    printf("Enter the First Matrix:\n");
    // Reading the first matrix:
    for(i=0;i<r1;i++){
        for(j=0;j<c1;j++){
            scanf("%d", &a[i][j]);
        }
    }

    printf("Enter the Row and Column of the Second Matrix:");
    scanf("%d %d",&r2,%c2);
    printf("Enter the Second Matrix\n");
    // Reading the second matrix:
    for(i=0;i<r2;i++){
        for(j=0;j<c2;j++){
            scanf("%d",&b[i][j]);
        }
    }

    if(c1==r2){ // Matrix Multiplication can be only done if column of first matrix is equal to row of second matrix
        for(i=0;i<r1;i++){
            for(j=0;j<c2;j++){ // taking r1 and c2 as the limits as the product matrix will be of the size r1 x c2
                m[i][j]=0; // Important 
                for(k=0;k<r2;k++){ // k can be less than r2 or c1 (k<c1 is also correct)
                    m[i][j] += a[i][k]*b[k][j]; // The Most Important Step
                }
            }
        }
        // Displaying the Product Matrix:
        for(i=0;i<r1;i++){
            for(j=0;j<c2;j++){
                printf("%d", m[i][j]);
            }
            printf("\n"); // Ensures the row wise printing of the matrix
        }
    } else {
        printf("The given matrices cannot be multiplied as the column of first matrix is not equal to the row of the second matrix");
    }

}
```

## Algorithm:

> Will be updated