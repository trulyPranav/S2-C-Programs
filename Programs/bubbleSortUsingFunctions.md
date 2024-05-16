## Code:
```c
#include <stdio.h>

// Function to perform Bubble Sort
void bubbleSort(int arr[], int n) {
    for (int i = 0; i < n - 1; ++i) {
        for (int j = 0; j < n - i - 1; ++j) {
            if (arr[j] > arr[j + 1]) {
                // Swap arr[j] and arr[j+1]
                int temp = arr[j];
                arr[j] = arr[j + 1];
                arr[j + 1] = temp;
            }
        }
    }
}

// Function to print array
void printArray(int arr[], int n) {
    for (int i = 0; i < n; ++i) {
        printf("%d ", arr[i]);
    }
    printf("\n");
}

void main() {
    int n, arr[100];
    printf("Enter the number of elements: ");
    scanf("%d", &n);

    printf("Enter %d elements of the array:\n", n);
    for (int i = 0; i < n; ++i) {
        scanf("%d", &arr[i]);
    }

    printf("Original array: \n");
    printArray(arr, n); // Prints the user inputted array

    // Performing Bubble Sort
    bubbleSort(arr, n);

    printf("Sorted array: ");
    printArray(arr, n); // Prints the Sorted array
}
```

## Algorithm:

> Will be updated