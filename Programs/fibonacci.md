## Code

```c
#include <stdio.h>
// Function to calculate Fibonacci number using recursion
int fibonacci(int n) {
    if (n <= 0) {
        return 0;
    } else if (n == 1) {
        return 1;
    } else {
        return fibonacci(n - 1) + fibonacci(n - 2);
    }
}

int main() {
    int n;

    printf("Enter the number of terms: ");
    scanf("%d", &n);

    printf("Fibonacci series:\n");
    for (int i = 0; i < n; i++) {
        printf("%d\n", fibonacci(i));
    }

    return 0;
}
```
## Algorithm
## Step 1 : Start
## Step 2 : Define the Recursive function :
- If n is 0, return 0.
- If n is 1, return 1.
- Otherwise, return the sum of the Fibonacci number at position n-1 and the Fibonacci number at position n-2.
## Step 3 : Define the main() :
- Prompt the user to input the number of terms n.
- For each integer i from 0 to n-1, call the recursive function to compute the Fibonacci number at position i and print the result.
## Step 4 : Stop
