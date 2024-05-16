## Code:
```c
#include<stdio.h>
#include<string.h>

void main(){
    char str[100];
    int i, len, flag = 0;

    printf("\nEnter the string: ");
    gets(str); //reads a string

    len = strlen(str); //finds the length of string using library function

    for(i = 0; i < len; i++){
        if(str[i] != str[len- i - 1]){
          flag = 1;
          break;//breaks the for loop if the condition is true
        }
    }

    if(flag == 0){
        printf("\nThe string %s is Palindrome", str);
    }
    else{
        printf("\nThe string %s is not Palindrome", str);
    }
}
```
## Algorithm: