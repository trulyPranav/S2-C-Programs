## Code:
```c
#include<stdio.h>
void main{

  int a,b,c; // Declaring three variables for storing the numbers
  printf("Enter three numbers:");
  scanf("%d%d%d", &a, &b, &c);//Reads three numbers


// For comparing the numbers, we are using Logical AND (&&) operator
  if( (a>b) && (a>c) ) 
  {
    printf("%d is the greatest number.",a);
  }
  else if( (b>a) && (b>c) ){
    printf("%d is the greatest number.",b);
  }
  else{
    printf("%d is the greatest number.",c);
  }

}
```

## Algorithm:

### Step 1:Start
### Step 2: Read three numbers and store it in a,b,c
### Step 3: if( (a>b) && (a>c) ) 
- Display a is the greatest number.
####   else if( (b>a) && (b>c) )
- Display b is the greatest number.
#### else
- Display c is the greatest number.
### Step 4: Stop