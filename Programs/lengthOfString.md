## Code:
```c
#include <stdio.h>

void main(){
    char str[1000];
    int i;
    printf("Enter the String: ");
    scanf("%s", &str); //accepts string from the user

    for(i = 0; str[i] != '\0'; ++i); 
    //to find the number of elements by iteration of empty for loop and store it in variable i 
    printf("The length of string is : %d", i);
}
```

## Algorithm: