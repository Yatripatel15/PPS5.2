# PPS5.2
about perfect numbers
#include <stdio.h>

int main() {
    int num, sum = 0;

    // Asking for input
    printf("Enter a positive number: ");
    scanf("%d", &num);

    // Loop to find the divisors and calculate the sum of divisors (excluding the number itself)
    for(int i = 1; i < num; i++) {
        if(num % i == 0) {
            sum += i;
        }
    }

    // Check if the sum of divisors is equal to the original number
    if(sum == num) {
        printf("%d is a perfect number.\n", num);
    } else {
        printf("%d is not a perfect number.\n", num);
    }

    return 0;
}


(explained by mam)
#include <stdio.h>
int main()
{
    int i,n,sum=0;
    printf("Enter the number:");
    
    scanf("%d",&n);
    //printf("the divisor of the %d is:",n);
    for(i=1;i<=n/2;i++)
    {
        if (n%i==0)
        sum=sum+i;
        printf("%d\n",i);
    }
    if (sum==n)
    printf("The number is a perfect number.");
    else
    printf("The number is not a perfect number");
    return 0;
}

