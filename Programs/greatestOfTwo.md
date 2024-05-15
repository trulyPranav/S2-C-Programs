## Code:
```c
#include<stdio.h>

void main(){
    int num1, num2;
    printf("Enter two numbers:"); //input two numbers for checking the greatest
    scanf("%d %d",&num1, &num2); //accepts two numbers using scanf
    //checks if num1 greater than num2
    if(num1>num2){
      //if yes prints num1 is greatest
      printf("%d is the greatest",num1);
    }
    else{
        //if no print num2 is greatest
      printf("%d is the greatest",num2);
    }
    //you can add an extra else if statement to check whether both the numbers are same
}
```
## Algorithm:

### Step 1: Start

### Step 2: Read two numbers store it in variables num1 and num2

### Step 3: If num1 greater than num2
- print num1 is greatest
#### else
-print num2 is greatest
### Step 4: Stop