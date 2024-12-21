# Unidades-de-volume-litro-mililitro-metros-c-bicos-
#include <stdio.h>

void converterLitrosParaMililitros(float litros) {
    printf("%.2f Litros = %.2f Mililitros\n", litros, litros * 1000);
}

void converterMililitrosParaLitros(float mililitros) {
    printf("%.2f Mililitros = %.2f Litros\n", mililitros, mililitros / 1000);
}

void converterLitrosParaMetrosCubicos(float litros) {
    printf("%.2f Litros = %.6f Metros Cúbicos\n", litros, litros / 1000);
}
No branches
No branches match the search
void converterMetrosCubicosParaLitros(float metrosCubicos) {
    printf("%.6f Metros Cúbicos = %.2f Litros\n", metrosCubicos, metrosCubicos * 1000);
}

void converterMililitrosParaMetrosCubicos(float mililitros) {
    printf("%.2f Mililitros = %.6f Metros Cúbicos\n", mililitros, mililitros / 1000000);
}

void converterMetrosCubicosParaMililitros(float metrosCubicos) {
    printf("%.6f Metros Cúbicos = %.2f Mililitros\n", metrosCubicos, metrosCubicos * 1000000);
}

int main() {
    float valor;
    int escolha;

    printf("Escolha a conversão desejada:\n");
    printf("1. Litros para Mililitros\n");
    printf("2. Mililitros para Litros\n");
    printf("3. Litros para Metros Cúbicos\n");
    printf("4. Metros Cúbicos para Litros\n");
    printf("5. Mililitros para Metros Cúbicos\n");
    printf("6. Metros Cúbicos para Mililitros\n");
    printf("Digite o número da opção desejada: ");
    scanf("%d", &escolha);

    printf("Digite o valor a ser convertido: ");
    scanf("%f", &valor);

    switch (escolha) {
        case 1:
            converterLitrosParaMililitros(valor);
            break;
        case 2:
            converterMililitrosParaLitros(valor);
            break;
        case 3:
            converterLitrosParaMetrosCubicos(valor);
            break;
        case 4:
            converterMetrosCubicosParaLitros(valor);
            break;
        case 5:
            converterMililitrosParaMetrosCubicos(valor);
            break;
        case 6:
            converterMetrosCubicosParaMililitros(valor);
            break;
        default:
            printf("Opção inválida!\n");
    }

    return 0;
}

    
