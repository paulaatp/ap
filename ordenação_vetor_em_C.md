# ap
algoritmos
#include <stdio.h>
#include <stdlib.h>
#include <string.h>

main(){
	
	int vetor[5]={9,7,3,5,1}, i, ord, j;
	
	for(i=0;i<5;i++){
	  for(j=4;j>i;j--){
		 if(vetor[j]<vetor[j-1]) {
			ord=vetor[j];
			vetor[j]=vetor[j-1];
			vetor[j-1]=ord;
			}
		}
	}
	
	for(i=0;i<5;i++){
		printf("%d\t", vetor[i]);
	}
	
}
