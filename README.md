#include <stdio.h>

int main() {
    int arr[50], n, i;

    // Input size of the array
    printf("Enter the size of the array (1 to 50): ");
    scanf("%d", &n);

    // Check if size is valid
    if (n < 1 || n > 50) {
        printf("Invalid array size. Please enter a size between 1 and 50.\n");
        return 1;
    }

    // Input elements of the array
    printf("Enter %d elements of the array:\n", n);
    for (i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }

    // Display the array in reverse order
    printf("Reversed array: ");
    for (i = n - 1; i >= 0; i--) {
        printf("%d ", arr[i]);
    }
    printf("\n");

    return 0;
}
