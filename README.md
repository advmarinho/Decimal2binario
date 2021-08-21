#include <stdio.h>

#define TAM 41

void main (){

int numeroDecimal, binario[TAM], aux;       //no int, precisamos definir as variaveis a ser utilizado.

printf("\n Digite um numero decimal: ");    //entrada de dados pelo operador/cliente
scanf("%d", &numeroDecimal);                //Recuperação dos valores digitados pelo operador cliente

    for(aux= TAM-1; aux >= 0; aux--){       //++ ou -- Incremento e decremento prefixo,
    binario[aux]= (numeroDecimal % 2)==0 ? 0 : 1;  //* / %	Multiplicação, divisão, e módulo resto
    numeroDecimal = numeroDecimal / 2;
                                            //Definido como o cálculo será efetuado, nesse caso aux com o tamanho definido em define menos
                                            //primeiro caractere, com mais dois operadores.
}

printf("\n\t");
for(aux=1; aux < TAM; aux++){
    printf("%d", binario[aux]);
    if((aux%4)==0)
        printf(" ");

}

 printf("\n");

 }
