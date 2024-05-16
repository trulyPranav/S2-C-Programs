### Code:
```c
#include <stdio.h>
//define recursive function fact
int fact(int n){
    if(n==0||n==1){
        return 1; // returns 1 since 0! and 1! is 1
    } else{
        return n*fact(n-1); // logic > n = 3, 3 * fact(2)=> 3 * 2 * fact(1) = 6
    }
}

void main(){
    int n;
    printf("enter a number");
    scanf("%d",&n);
    printf("Factorial of %d is : %d",n,fact(n));// calling the function in the main
}
```

## Algorithm

### Step 1: Define Function fact(n)
- input integer n
- output factorial of n

### Step 2: Cases :
- IF n is 0 or 1
    - return the value 1
- IF n is greater than 1:
    - return n*fact(n-1)

### Step 3: Writing main():
- initialize an integer variable n
- read a value for n
- print the message "factorial of n is result" , where result is returned by fact(n)

### Step 4: Stop