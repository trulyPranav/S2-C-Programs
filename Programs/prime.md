## Code:
```c
#include <stdio.h>

void main(){
    int n,flag=0,i;
    printf("Enter the Number:");
    scanf("%d", &n);
    if (n<=1){
        printf("Not a Prime Number");
    }
    else if(n == 2){
        printf("A Prime Number");
    }
    else{
        for(i=2 ; i<=(n/2) ; i++){
            if(n%i==0){
                flag = 1;
                break; // this is important
            }
        }  
        if(flag == 0){
            printf("A Prime Number");
        } else {
            printf("Not a Prime Number");
        }
    }
}
```

## Algorithm:

### Step 1: Start

### Step 2: initialize flag=0,n,i

### Step 3: Read n

### Step 4: if n<=1, Display 'Not a Prime Number'

### Step 5: else if n=2, Display 'A Prime Number'

### Step 6: Else repeat the following from i=2 until i<=n/2 
- if num%i = 0, flag = 1, go to step 7
- else increment i by 1

### Step 7: if flag = 1, Display 'Not a Prime Number'

#### else Display 'A Prime Number'

### Step 8: Stop