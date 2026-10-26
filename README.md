# Atividades-de-sala
Atividade slide 25
#include <stdio.h>
int main() {
	 float consumo, soma = 0;
	 for (int i = 1; i <= 5; i++)
	  {
	     printf("Digite o consumo do morador %d (m3): ", i);
	     scanf("%f", &consumo);
	 
	     soma += consumo;
	 
	     if (consumo <= 20) {
	     printf("Morador %d: Dentro da media.\n", i);
	     } 
	 
	     else {
	     printf("Morador %d: Acima da media.\n", i);
	     }
	 
	     }
	     printf("\nConsumo medio geral: %.2f m3\n", soma / 5);
	     return 0;
	}



  atividade slide 26
  #include <stdio.h>

int main() {
    float moeda, total = 0;
    
    printf("Digite as moedas (0.50, 1.00 ou 2.00). Digite 0 para encerrar:\n");
    
    do {
        printf("Adicionar moeda R$: ");
        scanf("%f", &moeda);
        
        if (moeda == 0.50 || moeda == 1.00 || moeda == 2.00) {
            total += moeda; 
        } 
        else if (moeda != 0) {
            printf("Valor invalido! Apenas moedas de 0.50, 1.00 ou 2.00.\n");
        }
        
    } while (moeda != 0);
    
    printf("\nTotal acumulado no cofrinho: R$ %.2f\n", total);
    
    return 0;
}



atividade slide 27
#include <stdio.h>

int main() {
    float nota, soma = 0, media;
    
    for (int i = 1; i <= 10; i++) {
        printf("Digite a nota do cliente %d (0 a 10): ", i);
        scanf("%f", &nota); 
        soma += nota;
    }
    
    media = soma / 10;
    
    printf("\nMedia geral de atendimento: %.2f\n", media);
    
    if (media < 7) {
        printf("ALERTA: A media do atendimento ficou abaixo de 7!\n"); 
    }
    
    return 0;
}
atividade slide 28
#include <stdio.h>

int main() {
    int passos, total_passos = 0;
    int horas = 0;

    printf(" Acompanhamento de Passos (Meta: 10.000) \n");

    
    while (total_passos < 10000) {
        horas++;
        printf("Digite os passos dados na hora %d: ", horas);
        scanf("%d", &passos);

        total_passos += passos;
    }

    printf("\n Meta Atingida!\n");
    printf("Total de passos acumulados: %d\n", total_passos);
    printf("Foram necessárias %d horas para atingir ou ultrapassar a meta de 10.000 passos.\n", horas);

    return 0;
}
