# ap
algoritmos
#include <stdio.h>
#include <stdlib.h>
#include <string.h>
//ORDENANDO VETOR
main(){
	
	int vetor[5]={9,7,3,5,1}, i, ord, j;
	//ASSIM
	for(i=0;i<5;i++){
	  for(j=4;j>i;j--){
		 if(vetor[j]<vetor[j-1]) {
			ord=vetor[j];
			vetor[j]=vetor[j-1];
			vetor[j-1]=ord;
			}
		}
	}
	// OU ASSIM
	/*
	for(i=0;i<5;i++){
	  for(j=0;j<5;j++){
		 if(vetor[i]<vetor[j]) {
			ord=vetor[i];
			vetor[i]=vetor[j];
			vetor[j]=ord;
			}
		}
	}
	*/
	
	for(i=0;i<5;i++){
		printf("%d\t", vetor[i]);
	}
	
}
