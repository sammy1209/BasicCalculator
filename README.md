#include <stdio.h>
#include <stdlib.h>
#include <math.h>

int main()
{
    int op;
    float a,b;
    while(1)
    {
        
        printf("\n1. Addition");
        printf("\n2. Subtraction");
        printf("\n3. Multiplication");
        printf("\n4. Divsion");
        printf("\n5. Power");
        printf("\n6. EXIT");
    
        printf("\nEnter Your cohoice: ");
        scanf("%d", &op);
        switch(op)
        {
            case 1:
            printf("Enter two Numbers: ");
            scanf("%f%f",&a,&b);
            printf("\nSum is %.01f", a+b);
            break;
        
            case 2:
            printf("Enter two Numbers: ");
            scanf("%f%f",&a,&b);
            if (a>b)
            printf("\nSub is %.01f", a-b);
            else
            printf("\nSub is %.01f", b-a);
            break;
        
            case 3:
            printf("Enter two Numbers: ");
            scanf("%f%f",&a,&b);
            printf("\nMultiplication is %.01f", a*b);
            break;
            
            case 4:
            printf("Enter two Numbers: ");
            scanf("%f%f",&a,&b);
            printf("\nDivision is %.01f", a/b);
            break;
        
            case 5:
            printf("Enter two Numbers: ");
            scanf("%f%f",&a,&b);
            printf("\nSum is %.01f", pow(a,b));
            break;
        
            case 6: exit(0);
        
            default:
            printf("INVALID OPTION");
        }
    }
    
}
