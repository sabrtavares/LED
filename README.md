//LED

#include <stdio.h>
  
int main() {
  
    int n, y, l[10] = {6, 2, 5, 5, 4, 5, 6, 3, 7, 6};
    char d;
    scanf("%d", &n);
    getchar();
    
    while(n--){
        y = 0;
        while((d = getchar()) != '\n'){
            y += l[d - '0'];
        }
        printf("%d leds\n", y);
    }
  
    return 0;
}
