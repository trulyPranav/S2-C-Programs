## Code:
```c
#include <stdio.h>

void main(){
    int a[100],i,n,flag=0,search;
    
    printf("Enter size of the array:");
    
    scanf("%d",&n);
    
    printf("Enter the %d elements of the array:", n);
    
    for(i=0;i<n;i++){
        scanf("%d",&a[i]);
    }
    
    printf("Enter the element to be searched:");
    
    scanf("%d", &search);
    
    for(i=0;i<n;i++){
        if(a[i]==search){
            flag=1;
            break; // important
        }
    }

    if(f==1)
        printf("Element %d found at index %d", search, i);
    else 
        printf("Element not found");
}
```

## Algorithm:

### Step 1: Start

### Step 2: initialize a[100],i,n,flag=0 and search

### Step 3: Read the number of elements of array and store it in n

### Step 4: Read the elements of array by initializing a for loop form i=0 till i<n

### Step 5: Read the element to be searched and store it in search

### Step 6: initialize a for loop from i=0 till i<n

#### Step 6.1: if a[i] = search, flag = 1

### Step 7: if flag = 1, Display 'Element search found at index i'

### Step 8: else Display 'Element not found'

### Step 9: Stop
