## Code:
```c
#include <stdio.h>

void main(){
    char str[100], revStr[100];
    int i, length;

    printf("Enter the string to be reversed:");
    scanf("%s", str);

    // Calculate the length:
    while(str[i] != '\0'){
        length++;
        i++;
    }

    // Reversing the string:
    for(i=0; i<length; i++){
        if(str[i] != '\0'){
            revStr[length-1-i] = str[i];
        }
    }

    printf("String after reversing : %s", revStr);
}
```
## Algorithm:

> Will be updated