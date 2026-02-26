# ShawnQuickSort# 

A clean, in-place implementation of the **QuickSort** algorithm in C, with both **ascending** and **descending** order variants using the Lomuto partition scheme.

## Features

- In-place sorting (no extra array needed)
- Uses **Lomuto partition** scheme
- Recursive implementation
- Supports sorting in **ascending** and **descending** order
- Simple and readable variable names

## Code Overview

| File/Function       | Description                                      |
|---------------------|--------------------------------------------------|
| `quickSort()`       | Ascending order QuickSort (smaller elements left) |
| `quickSortDesc()`   | Descending order QuickSort (larger elements left)|

Both functions follow this signature:

```c
void quickSort(int numbers[], int start, int end);
void quickSortDesc(int numbers[], int start, int end);
#include <stdio.h>

void quickSort(int numbers[], int start, int end) {
    
}

void quickSortDesc(int numbers[], int start, int end) {
    
}

int main() {
    int arr[] = {64, 34, 25, 12, 22, 11, 90};
    int n = sizeof(arr) / sizeof(arr[0]);

    printf("Original array: ");
    for (int i = 0; i < n; i++) printf("%d ", arr[i]);
    printf("\n");

    quickSort(arr, 0, n - 1);
    printf("Sorted ascending : ");
    for (int i = 0; i < n; i++) printf("%d ", arr[i]);
    printf("\n");

    int arr2[] = {64, 34, 25, 12, 22, 11, 90};

    quickSortDesc(arr2, 0, n - 1);
    printf("Sorted descending: ");
    for (int i = 0; i < n; i++) printf("%d ", arr2[i]);
    printf("\n");

    return 0;
}
void quickSort(int numbers[], int start, int end);
void quickSortDesc(int numbers[], int start, int end);
quickSort(arr, 0, size - 1);       // ascending
quickSortDesc(arr, 0, size - 1);   // descending
