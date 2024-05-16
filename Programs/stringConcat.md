## Code:
```c
#include <stdio.h>

void main(){
    char str1[100], str2[100];
    int i, j;

    printf("Enter first string : "); //accepts first string
    scanf("%s", &str1);

    printf("Enter second string : "); //accepts second string
    scanf("%s", &str2);
    
    //calculates the number of elements in string 1 and strores it in i
    for(i = 0; str[i] != '\0'; ++i); 

    //assigns the first element of string 2 to the last element of string 1 by looping
    for(j = 0; str2[j] != '\0'; ++j, ++i){
        str1[i] = str2[j];
    } 
    
    str1[i] = '\0';
    printf("The string after concatenation : %s", str1);
}
```

## Algorithm: