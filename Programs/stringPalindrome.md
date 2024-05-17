## Code:
```c
#include<stdio.h>

void main(){
    char a[100],b[100];
    int flag=0,len=0,i=0;

    printf("Enter the Word:");
    scanf("%s",a);

    // Calculating lenth of the string:
    while(a[i] != '\0'){
        len++;
        i++;
    }

    // Reversing string:
    for(i=0; i<len; i++){
        if(a[i] != '\0'){
            b[len-1-i] = a[i];
        }
    }

    // Checking Palindrome:
    for(i=0; i<n; i++){
        if(a[i]!=b[i]){
            flag = 1;
            break;
        }
    }

    if(flag == 1)
        printf("Not a Palindrome");
    else 
        printf("A Palindrome");
}
```
## Algorithm:

> Will be updated