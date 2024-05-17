## Code:
```c
#include <stdio.h>
#include <math.h> //for using pow() function

// An Armstrong Number example = 153 because (1³+5³+3³ = 153)

void main(){
    int num,originalNum,remainder,digits=0,result=0;
    printf("Enter your number:");
    scanf("%d", &num);
    originalNum = num; // doing this will not alter the value stored in num

    //Now we calculate the number of digits:
    while(originalNum!=0){
        originalNum/=10; // same as that of originalNum = originalNum/10
        digits++; // digits are increased by 1 => digits = digits + 1
    }
    // The above process is nothing but we divide our number by 10 until it reaches zero,
    // and for each division by 10, we increase digit count by 1
    
    originalNum = num; // This reassigning is important!

    //Now we add the individual number raised to the digits, and is stored in the result variable
    while(originalNum!=0){
        remainder = originalNum%10; // finding individual numbers, eg: 153%10 = 3, now this 3 is used in the just below step
        result += pow(remainder,digits); // here individual numbers are raised to the digits we calculated above
        originalNum/=10; //to eliminate the used digit
    }

    //Checking Armstrong or Not
    if(result == num){
        printf("%d is an Armstrong Number", num);
    }
    else {
        printf("%d is not an Armstong Number", num);
    }

}
```
## Algorithm:

### Step 1: Start

### Step 2: initialize num,originalNum,result,remainder,digits

### Step 3: Read the number

### Step 4: originalNum = num

### Step 5: initialize a while loop until originalNum is not equal to 0.
- originalNum = originalNum/10
- digits++

### Step 6: originalNum = num

### Step 7: initialize a while loop until originalNum is not equal to 0.
- remainder = originalNum%10
- result = result + (remainder raised to digits)
- originalNum = originalNum/10

### Step 8: if result == num
- Display "An Armstrong Number"

#### else
- Display "Not an Armstrong Number"

### Step 9: Stop
