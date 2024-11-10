# 📊 Algoritmo Bubble Sort 🔄

## 💡 O que é?

O **Bubble Sort** é um algoritmo simples de ordenação que funciona repetidamente comparando elementos adjacentes em uma lista e trocando-os se estiverem na ordem errada. O maior elemento "flutua" para o final da lista a cada passagem.

---

## 🧑‍💻 Como Funciona?

### 1️⃣ **Inicialização:**
- A função `bubble_sort` recebe um array (`arr`) como entrada.
- A variável `n` armazena o comprimento da lista.

### 2️⃣ **Loop Externo:**
- O primeiro `for` itera de `i = 0` até `n-1`.
- Cada passagem garante que o maior elemento não ordenado "flutua" para o final.

### 3️⃣ **Loop Interno:**
- O segundo `for` itera de `j = 0` até `n-i-2`.
- A cada iteração do loop externo, você verifica um número a menos, pois os últimos `i` elementos já estão ordenados.

### 4️⃣ **Comparação e Troca:**
- A condição `if arr[j] > arr[j+1]` compara os elementos atuais (`arr[j]`) e o próximo (`arr[j+1]`).
- Se o elemento atual é maior, os dois são trocados para garantir a ordem correta.

---

## 🔄 Resultado

Após a execução do algoritmo, a lista estará ordenada! Exemplo:

```python
lista = [34, 12, 7, 19, 21, 4, 10]
print(bubble_sort(lista))
Saída:

python
Copiar código
[4, 7, 10, 12, 19, 21, 34]
📚 Complexidade
Melhor Caso (lista já ordenada): O(n)
Pior Caso (lista invertida): O(n²)
Caso Médio: O(n²)
⚙️ Implementação
Aqui está a implementação do Bubble Sort em Python:

python
Copiar código
def bubble_sort(arr):
    n = len(arr)
    for i in range(n):
        for j in range(n - i - 1):
            if arr[j] > arr[j + 1]:
                arr[j], arr[j + 1] = arr[j + 1], arr[j]
    return arr
