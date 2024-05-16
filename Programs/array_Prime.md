## Code:
```c
#include <stdio.h>

void main() {
    int a[100],flag,n,i,j;
    printf("Enter the Size of the array:");
    scanf("%d",&n);
    printf("Enter the array elements:");
    for(i=0;i<n;i++){
        scanf("%d",&a[i]);
    }
    for(i=0;i<n;i++){ // This for loop goes each element by element
        flag = 0;
        if(a[i]<=1){
            flag = 1; // Since numbers less than & equal to 1 is not prime
        }
        else if(a[i]==2){
            flag = 0;
        }
        else {
            for(j=2;j<a[i];j++){
                // This for loop checks the prime number condition for the 
                // current a[i] element we are in, iff a[i]>2
                if(a[i]%j==0){
                    flag = 1;
                    break;
                }
            }
            if (flag == 0){
                printf("%d is a Prime Number\n",a[i]);
            } else {
                printf("%d is not a Prime Number\n", a[i]);
            }
        }
    }
}
```