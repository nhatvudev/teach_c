- Tìm số lớn thứ 2 trong 1 mảng. Ví dụ mảng
```
int numbers[] = {1, 3, 7, 2, 5, 9, 11, 6};
```

- Lời giải:
```C
#include <stdio.h>

int main() {
    int numbers[] = {1, 3, 7, 2, 5, 9, 11, 6};
    int numbersLength = sizeof(numbers)/sizeof(int);
    int max1 = numbers[0];
    int max2 = numbers[1];

    if (max1 < max2) {
        int temp = max1;
        max1 = max2;
        max2 = temp;
    }

    for (int i = 2; i < numbersLength; i++) {
        if (max2 < numbers[i])
            max2 = numbers[i];

        if (max1 < max2) {
            int temp = max1;
            max1 = max2;
            max2 = temp;
        }
    }

    printf("max2 = %d\n", max2);
    return 0;
}
```