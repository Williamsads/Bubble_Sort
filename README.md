Como Funciona o Bubble Sort

Inicialização:

A função bubble_sort recebe um array (arr) como entrada.

A variável n armazena o comprimento da lista.

Loop Externo:

O primeiro for itera i de 0 até n-1. Esse loop controla quantas passagens o algoritmo fará. A cada passagem, o maior elemento não ordenado "flutua" para o final da lista.

Loop Interno:

O segundo for itera j de 0 até n-i-2. Isso significa que, a cada iteração do loop externo, você verifica um número a menos, pois os últimos i elementos já estão na posição correta.

Comparação e Troca:

A condição if arr[j] > arr[j+1] compara o elemento atual (arr[j]) com o próximo (arr[j+1]).
Se o elemento atual é maior que o próximo, os dois elementos são trocados para que o menor fique à frente. Isso é feito na linha arr[j], arr[j+1] = arr[j+1], arr[j].

Resultado:

Depois que todos os loops são concluídos, a lista está ordenada e é retornada pela função.

Quando você executa print(bubble_sort(lista)), a saída é:
[0, 1, 3, 4, 6, 7, 8, 10, 11, 12, 16, 17, 19, 21, 29, 30, 34, 39, 43, 56, 61, 67, 82]
