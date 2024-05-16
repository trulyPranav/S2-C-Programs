## Code:
```c
#include<stdio.h>
int main()
{
    char name[100],rev[100];
    int i,count=0;
    printf("Enter string:");
    fgets(name,100,stdin);                    //If we use scanf(), it stops reading after encountering a whitespace

    while(name[i]!='\0'){           //Null character ('\0') is at the end of every string, we have to only calculate upto the null character
        count++;           //Length of string is calculated
        i++;
    }

      //(IMP) here we use count-1 instead of count because the first character of the string we have entered will be stored in the index 0
       printf("Length of the string: %d",count-1);
    return 0;
}
```

## Algorithm:
> will be updated