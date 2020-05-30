# My-Captain-ac
Developed by Pragya Pandey

#include<stdio.h>

int find_lcm(int, int);   

int main()
{
    printf("Studytonight - Best place to learn");
    int a, b, lcm;
    printf("Enter 2 integers to find LCM of:\n");
    scanf("%d%d", &a, &b);
    lcm =lcm(a,b);    
    printf("LCM of %d and %d is: %d\n\n", a, b, lcm);
    printf("Coding is Fun");
    return 0;
}

int lcm(int a, int b)  
{
    int temp = 1;    
    if(temp%a == 0 && temp%b == 0)
    {
        return temp;
    }
    else
    {
        temp++;
        lcm(a,b);
        return temp;
    }
}
