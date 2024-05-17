## Code:
```c
#include <stdio.h>

void main() {
    int year;

    // Read the year from the user
    printf("Enter a year: ");
    scanf("%d", &year);

    // A year is a leap year if it is divisible by 4 and NOT divisible by 100
    // but a leap year if it divisible by 400

    // Check if the year is a leap year
    if ((year % 4 == 0 && year % 100 != 0) || (year % 400 == 0)) {
        printf("%d is a leap year.\n", year);
    } else {
        printf("%d is not a leap year.\n", year);
    }
}
```
## Algorithm:

### Step 1: Start

### Step 2: Initialize year

### Step 2: Read the year from the user and store it in year

### Step 3: Check if the year is divisible by 4 and not divisible by 100:
- If true, Display "year is a leap year."

### Step 4: else check if the year is divisible by 400:
- If true, Display "year is a leap year."

### Step 5: else if neither Step 3 nor Step 4 conditions are met:
- Display "year is not a leap year."

### Step 6: Stop


