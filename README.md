# atividade-3-11








#include <stdio.h>
#include <stdlib.h>
#include <unistd.h>
#include <locale.h>

	int main (){
	setlocale(LC_ALL,"");
	system("color f9");	
	 int n1,i, resultado = 0;	
	
	printf("Digite um número: ");
	scanf("%d",&n1);
	   for (i = 2; i <= n1 / 2; i++){
	   	if(n1 % i == 0){
	   		resultado++;
	   		break;
	       }
	   }	
	
	if(resultado == 0){
		printf("%d é um número primo \n", n1);
    }else{	
     	printf("%d não é um número primo \n",n1);
    }
	return 0;
}
