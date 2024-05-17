## Code:
```c
#include <stdio.h>

void main(){
    char s1[10],s2[10];
    int flag=0;

    printf("Enter the First String:");
    scanf("%s", s1);

    printf("Enter the Second String");
    scanf("%s", s2);

    for(int i=0; s[i] != '\0' || s[i] != '\0'; i++){ // i.e, the program must go on until one of the string ends
        if(s1[i] != s2[i]){
            flag = 1;
            break; // Important
        }
    }

    if(flag == 1)
        printf("The strings are not same");
    else
        printf("The strings are same");
}
```