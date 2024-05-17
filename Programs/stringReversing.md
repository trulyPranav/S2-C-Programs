## Code:
```c
#include<stdio.h>
#include<string.h>

void main(){
    char str[100], revStr[100];
    int i, j = 0, length;

    printf("Enter the string to be reversed :");
    gets(str); //gets used instead of scanf to accept white spaces as well

    length = strlen(str); //standard library function used for finding length of string

    for(i = length - 1; i >= 0; i--){
        revStr[j++] = str[i]; 
        //stores the last element in the str array as the first element in the revStr array
    }
    revStr[i] = '\0'; //declares the last element as null value

    printf("String after reversing : %s", revStr);
}
```
## Algorithm: