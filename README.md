#define _CRT_SECURE_NO_WARNINGS 
#include<stdio.h>

int main() {

    int N, K;
    int a = 0;
    int i;
    scanf("%d %d", &N, &K);


    for (i = 1; i <= N; i++) {
    
        if (N % i == 0) {
        
            a++;
        }
        if (a == K) {
            break;
        }
    }
    if (i <= N) {
    
        printf("%d", i);
    }
    else {
    
        printf("0");
    }
    return 0;
}
