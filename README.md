# Fa-a-um-algoritmo-que-receba-3-n-meros-e-depois-mostre-eles-em-ordem-crescente
#include <stdio.h>

int main()
{
    //Declarando a variavel 
    int Num1,Num2,Num3,x=0;
    
    //Declarando a variavel 
    printf("\nDigite 3 numeros.\nPrimeiro numero:");
    scanf("%d",&Num1);

    printf("Segundo numero:");
    scanf("%d",&Num2);

    printf("Terceiro numero:");
    scanf("%d",&Num3);
    
//Verificação Condicional 
    if(Num1 > Num2){
        x=Num1;
        Num1=Num2;
        Num2=x;
    }
    if(Num2 <= Num3){
        printf("A ordem crescente e: %d %d %d\n",Num1,Num2,Num3);
    }
    else
    {
        if(Num1 <= Num3){
            printf("A ordem crescente e: %d %d %d\n",Num1,Num3,Num2);
        }
        else
        {
            printf("A ordem crescente e: %d %d %d\n",Num3,Num1,Num2);
        }
    }
    
    return 0;
}
