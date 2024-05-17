## Code:
```c
#include <stdio.h>

// Function to perform linear search
int linearSearch(int arr[], int n, int search) {
    for (int i = 0; i < n; ++i) {
        if (arr[i] == search) {
            return i; // Return the index where the search key is found
        }
    }
    return -1; // Return -1 if key is not found
}

void main() {
    int n, arr[100],search;
    printf("Enter the number of elements: ");
    scanf("%d", &n);

    printf("Enter %d elements:\n", n);
    for (int i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }

    
    printf("Enter the element to search: ");
    scanf("%d", &search);

    // Perform Linear Search
    int result = linearSearch(arr, n, search);

    if (result != -1) {
        printf("Element %d found at index %d\n", search, result);
    } else {
        printf("Element %d not found in the array\n", search);
    }
}
```

## Algorithm:

> Will be updated
