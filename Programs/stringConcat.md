## Code:
```c
#include <stdio.h>

void main(){
    char str1[100], str2[100];
    int len1=0,len2=0,i=0;

    printf("Enter first string : "); // Accepts first string
    scanf("%s", str1);

    printf("Enter second string : "); // Accepts second string
    scanf("%s", str2);
    
    // Calculating the number of elements in String 1 and storing it in len1
    while(str1[i]!='\0'){
        len1++;
        i++;
    }

    i=0; // Resetting i to 0 to calculate len2

    // Calculating the number of elements in String 2 and storing it in len2
    while(str2[i]!='\0'){
        len2++;
        i++;
    }

    // Concatenating
    for(i=0; i <= len2; i++){
        str1[len1+i] = str2[i];
    }

    printf("The string after concatenation : %s", str1);
}
```

## Algorithm:

> Will be updated