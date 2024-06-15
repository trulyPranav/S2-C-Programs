## Code:
```c
#include <stdio.h>
#include <math.h>

int main() {
    int a[100], flag, n, i, j;
    printf("Enter the Size of the array: ");
    scanf("%d", &n);
    printf("Enter the array elements: ");
    for(i = 0; i < n; i++) {
        scanf("%d", &a[i]);
    }
    for(i = 0; i < n; i++) { // This for loop goes each element by element
        flag = 0;
        if(a[i] <= 1) {
            // Since numbers less than & equal to 1 are not prime
            printf("%d is not a Prime Number\n", a[i]);
        }
        else if(a[i] == 2) {
            printf("%d is a Prime Number\n", a[i]);
        }
        else {
            for(j = 2; j <= sqrt(a[i]); j++) {
                // This for loop checks the prime number condition for the 
                // current a[i] element we are in, if a[i] > 2
                if(a[i] % j == 0) {
                    flag = 1;
                    break;
                }
            }
            if(flag == 0) {
                printf("%d is a Prime Number\n", a[i]);
            } else {
                printf("%d is not a Prime Number\n", a[i]);
            }
        }
    }
    return 0;
}

```

## Algorithm:

### Step 1: Start

### Step 2: Initialize a[100],i,j,lim,temp

### Step 3: Read the size of array and store it in lim

### Step 4: Input array elements using a for loop

### Step 5: Initialize a for loop from i=0 till i<lim-1

#### Step 5.1: Initialize a for loop from j=0 till j < lim-i-1 and do the following if a[j]>a[j+1]
<pre>
Step 5.1.1:
    temp = a[j];
    a[j] = a[j+1];
    a[j+1] = temp;
</pre>

### Step 6: Display the Sorted Array

### Step 7: Stop

