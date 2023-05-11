#include <stdio.h>

int main() {
    printf("************************************\n");
    printf("* Bem-vindo ao Jogo de Adivinhação *\n");
    printf("************************************\n");

    int numerosecreto;
    numerosecreto = 42;

    int chute;

    printf("Qual é o seu chute? ");
    scanf("%d", &chute);
    printf("Você chutou o número %d!\n", chute);

    if (chute == numerosecreto) {
        printf("Parabéns, você acertou!\n");
    } else {
        printf("Poxa vida, você errou!\n");
    }

    printf("Qual é o seu chute? ");
    scanf("%d", &chute);
    printf("Seu chute foi %d\n", chute);

    if (chute == numerosecreto) {
        printf("Parabéns, você acertou!\n");
        printf("Jogue de novo, você é um bom jogador!\n");
    } else {
        printf("Você errou!\n");
        printf("Mas não desanime, tente de novo!\n");
    }

    printf("Qual é o seu chute? ");
    scanf("%d", &chute);
    printf("Seu chute foi %d\n", chute);

    if (chute == numerosecreto) {
        printf("Parabéns, você acertou!\n");
    } else {
        if (chute > numerosecreto) {
            printf("Seu chute foi maior que o número secreto!\n");
        } else {
            printf("Seu chute foi menor do que o número secreto!\n");
        }
    }

    int acertou = chute == numerosecreto;

    if (acertou) {
        printf("Parabéns, você acertou!\n");
    } else {
        if (chute > numerosecreto) {
            printf("Seu chute foi menor que o número secreto!\n");
        } else {
            printf("Seu chute foi maior do que o número secreto!\n");
        }
    }

    return 0;
}
