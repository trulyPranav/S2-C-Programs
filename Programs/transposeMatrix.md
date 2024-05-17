## Code:
```c
#include <stdio.h>

void main()
{

    int a[10][10],i=0,j=0,t[10][10],r,c;
    printf("Enter row & column size:");
    scanf("%d%d",&r,&c);
 
    printf("Enter the matrix elements:");
    for(i=0;i<r;i++){ // Loop For Row 
        for(j=0;j<c;j++){ // Loop For Column
            scanf("%d",&a[i][j]); // Reads the Matrix
        }
    }
    
    // Transposing the Matrices
    for(i=0;i<r;i++){
        for(j=0;j<c;j++){
            t[j][i]=a[i][j]; //Swapping Indexes
        }
    }

    printf("Transpose is:\n");
    for(i=0;i<c;i++){
        for(j=0;j<r;j++){
           printf("%d\t",t[i][j]); // Prints the resultant transpose
        }
        printf("\n"); // This will helps to print the elements row-wise
    }
}


```

## Algorithm:

> Will be updated
