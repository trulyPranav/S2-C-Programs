## Code:
```c
#include <stdio.h>

void main(){
    char str[1000];
    int i;
    printf("Enter the String: ");
    scanf("%s", &str);

    for(i = 0; str[i] != '\0'; ++i);
    printf("The length of string is : %d", i);
}
```

## Algorithm: