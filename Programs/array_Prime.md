## Code:
```c
#include <stdio.h>

void main() {
    int a[100],flag,n,i,j;
    printf("Enter the Size of the array:");
    scanf("%d",&n);
    printf("Enter the array elements:");
    for(i=0;i<n;i++){
        scanf("%d",&a[i]);
    }
    for(i=0;i<n;i++){ // This for loop goes each element by element
        flag = 0;
        if(a[i]<=1){
            // Since numbers less than & equal to 1 is not prime
            printf("%d is not a Prime Number\n", a[i]);
        }
        else if(a[i]==2){
            printf("%d is a Prime Number\n",a[i]);
        }
        else {
            for(j=2;j<=a[i];j++){
                // This for loop checks the prime number condition for the 
                // current a[i] element we are in, iff a[i]>2
                if(a[i]%j==0){
                    flag = 1;
                    break;
                }
            }
            if (flag == 0){
                printf("%d is a Prime Number\n",a[i]);
            } else {
                printf("%d is not a Prime Number\n", a[i]);
            }
        }
    }
}
```

## Algorithm:

### Step 1: Start

### Step 2: Initialize a[100], n, i, j, flag

### Step 3: Read Size of Array and store it in n

### Step 4: Read the elements of the array by initializing a for loop from i=0 till i<n

### Step 5: Initialize a for loop from i=0 and repeat the below till i<n

#### Step 5.1: flag = 0

#### Step 5.2: Check if a[i] is less than or equal to 1:
- If true, Display 'a[i] is not a Prime Number'
- Otherwise, check if a[i] equals 2:
- If true, Display 'a[i] is a Prime Number'
- Otherwise, proceed to step 5.2.1
<pre>
5.2.1: Initialize a for loop from j=2 till j<=a[i]/2
            if a[i]%j=0, flag=0 and break the loop
5.2.2: After the loop, check flag value:
            - If flag equals 0, Display 'a[i] is a Prime Number'
            - Otherwise, Display 'a[i] is not a Prime Number'
</pre>

### Step 6: Stop
