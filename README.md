# Fibonacci-Series
Write fibonacci series in c 

#include<stdio.h>
int fibonacci (int);
    int main (){
        int num, res, i =0;
        printf("Enter the number of terms: ");
        scanf("%d",&num);
        printf("Fibonacci series\n");
        for ( i = 0; i <num; i++)
        {
            res = fibonacci (i);
            printf(" %d",res);
        }  
    return 0;
}
int fibonacci (int num){
    if (num == 0)
    return 0;
    else if (num == 1)
    return 1;
    else
    return (fibonacci(num - 1) + fibonacci(num - 2));
}
