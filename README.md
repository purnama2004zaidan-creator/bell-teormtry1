#include <stdio.h>

void proses(int a) {
    for (int i = a; i > 0; i--) {
        int b = a - i;

        printf("%d-%d=%d\n", a, i, b);

        if (b > 0) {
            proses(b);
        }
    }
}

int main() {
    int a;
    scanf("%d", &a);

    proses(a);

    return 0;
}
