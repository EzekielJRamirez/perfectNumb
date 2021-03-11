#include <stdio.h>
#include <stdbool.h>
#include <math.h>

bool isPerfect(int n){
    int sum = 1;
    
    for(int i = 2; i * i <= n; i++){
        if(n % i ==0){
            if(i*i != n)
                sum = sum + i + n / i;
            else
                sum = sum + i;
        }
    }
    
    if(sum == n && n != 1)
        return true;
    
    return false;
    
}


int main()
{
  
    int cpu = 32;
    float allInOne = (pow(2, cpu - 1))/2 - 1;
    printf("%f", allInOne);
    printf("Below are all perfect numbers\n");
    for(int n = 2; n < allInOne; n++){
        if(isPerfect(n)){
            printf("%d\n", n);
        }
    }

    return 0;
}
