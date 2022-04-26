#include <stdio.h>
#include <math.h>
#define f(x)=x*x-4

int main()
{
    int i;
    int N=100;
    double x=1.0;
    double xx=3.0;
    double xxx;
    double eps=1e-15;
    
    for(i=0;i<N;i++)
    {
        xxx=(x+xx)/2;
        
        if(fabs(xxx)<eps)
        break;
    }
    
    printf("x=%10lf\n",xxx);
    return 0;
}


