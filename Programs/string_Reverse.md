## Code:
```c
#include<stdio.h>
int main()
{
    char name[100],rev[100];
int i,count=0;
    printf("Enter string:");
    fgets(name,100,stdin);     //If we use scanf(), it stops reading after encountering a whitespace
    //To find the length of the string
    while(name[i]!='\0'){
        count++;
        i++;
    }
    //Reversing a string
    for(i=0;i<count;i++){
      rev[i]=name[count-i-1];

    }
    printf("%s",rev);
    return 0;
}
```

## Algorithm:
> will be updated