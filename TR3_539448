#include <stdio.h>
#include <stdlib.h>

//MODELO DE EXEMPLO

int main(){
   
   	//VariÃ¡veis que podem ser usadas
   	unsigned int x[200];
   	int y;
   	int z;
   	int k;
   	int w;
   	int j;
   	int i;
   	
   	//#########################
   	
   	for(i = 0; i <= 199; i++){// for usado para zerar o bit set
           x[i]= 0;
        }

   	while(1){// whilhe true realiza a coleta dos numeros digitados pelo usuário

           printf("Digite um numero! ");
           scanf("%i", &z);

           if(z == -1){// caso de saida do while
              break;
           }

           else{// onde é definido a posição do vetor em que o numero sera armazenado
              w = z/32;
              x[w] = x[w] | (1 << (z - 32*w));
           }
        }

        z = 0;
        y = 0;
	
	//imprimir os valores digitados
        while(y <= 199){// caminha pelo vetor para acessar cada posiçao do bit set

           for(z; z <= 31; z++){// procura e acessa cada sub-posiçao do bit set preenchida

              if(1 & (x[y] >> z)){
     
                 printf("%i \n", (z+(32*y))); // impressao dos valores encontrados
              }

           }
           y++;
           z = 0;
        }
   	//#########################
   
	return 0;  
}
