## Code:
```c
#include<stdio.h>

void main()
{

    int a[10][10],b[10][10],i=0,j=0,s[10][10],r,c;
    printf("Enter row & column size:");
    scanf("%d%d",&r,&c);              //Row & Column size will be same for Matrix Addition
 
    printf("Enter 1st matrix elements:");
    for(i=0;i<r;i++)                  //Loop For Row 
    {
        for(j=0;j<c;j++)              //Loop For Column
        {
            scanf("%d",&a[i][j]);             //Reads First Matrix
        }
    }

     printf("Enter 2nd matrix elements:");
    for(i=0;i<r;i++)                                      //Loop For Row 
    {
        for(j=0;j<c;j++)                                  //Loop For Column
        {
            scanf("%d",&b[i][j]);              //Reads Second Matrix
        }
    }
    

    for(i=0;i<r;i++)
    {
        for(j=0;j<c;j++)
        {
            s[i][j]=a[i][j]+b[i][j];            //Matrix addition
        }
    }

     for(i=0;i<r;i++)
     {
        for(j=0;j<c;j++)
        {
           printf("%d\t",s[i][j]);         //Prints the resultant matrix
        }
        printf("\n");                    // This will helps to print the elements row-wise
    }
}