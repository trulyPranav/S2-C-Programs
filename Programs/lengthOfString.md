## Code:
```c
#include <stdio.h>

void main(){
    char str[1000];
    int count=0,i=0;
    printf("Enter the String: ");
    scanf("%s", str); // Accepts string from the user

    while(str[i]!='\0'){
        count++;
        i++;
    }

    printf("Length of the String is %d", count);
}
```

## Algorithm:
> Will be updated