/*	Nome: Victor Melly Cabredo
	TIA: 31836895				*/

#include <stdio.h>
#include <stdlib.h>

/*Verifica linhas e diagonais*/
int verifica(int *tabuleiro){
	int i,j;
	for(i=0;i<8;i++){
		for(j=i+1;j<8;j++){
			/*Linhas*/
			if((tabuleiro[i]%8)==(tabuleiro[j]%8)){
				return 1;
			}
			/*Diagonais*/
			if(abs((tabuleiro[i]%8)-(tabuleiro[j])%8)==abs(i-j)){
				return 1;
			}
		}
	}
	return 0;
}
/*Impressao em notacao de xadrez*/
void imprime(int *tabuleiro){
	int i;
	char colunas[8]={'a','b','c','d','e','f','g','h'};
	for(i=0;i<8;i++){
		printf("Q%c%d, ",colunas[i],(tabuleiro[i]%8)+1);
	}
	printf("\n");
}

int solucao(){
	int tabuleiro[8]={00,00,00,00,00,00,00,00};
	int a,b,c,d,e,f,g,h;
	for(a=0;a<8;a++){
		for(b=0;b<8;b++){
			for(c=0;c<8;c++){
				for(d=0;d<8;d++){
					for(e=0;e<8;e++){
						for(f=0;f<8;f++){
							for(g=0;g<8;g++){
								for(h=0;h<8;h++){
									if(verifica(tabuleiro)==0){
										imprime(tabuleiro);
										/*return 0;*/
/*Retire o <return 0> acima para obter todas as solucoes*/
									}
									tabuleiro[7]++;
									}
								tabuleiro[6]++;
								}
							tabuleiro[5]++;
							}
						tabuleiro[4]++;
						}
					tabuleiro[3]++;
					}
				tabuleiro[2]++;
				}
			tabuleiro[1]++;
			}
		tabuleiro[0]++;
		}
	return 1;
}

int main(){
	solucao();
	return 0;
}
