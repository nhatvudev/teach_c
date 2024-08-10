```C
#include <stdio.h>

int mysqrt( int n ){
    int x = n;
    while( 1 ){
        int y = (x + n/x)/2;
        if( y >= x ) 
            return x;
        x = y;
    }
}

int main() {
    int n = 0;

    printf("n = ");
    scanf("%d", &n);

    int result = mysqrt(n);

    printf("square root of the largest square number which is smaller than n: %d", result);
    return 0;
}
```