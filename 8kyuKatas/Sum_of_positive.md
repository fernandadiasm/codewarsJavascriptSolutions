# CodeWars JavaScript Solutions

---

## Sum of positive

**Descrição**

Você obtém uma matriz de números, retorna a soma de todos os positivos.

Exemplo `[1,-4,7,12]=>1 + 7 + 12 = 20`

Nota: se não houver nada para somar, a soma é padrão para 0.

---

### Código dado

```` JavaScript
function positiveSum(arr) {
  
}
````

---

### Minha Solução

```` JavaScript
function positiveSum(arr) {
      let sum = 0;

    for (let i = 0; i < arr.length; i++) {
        if (arr[i] > 0) {
            sum += arr[i];
        }
    }

    return sum;
}
````

<details>
<summary>Explicação</summary>

1. A função `positiveSum` recebe uma matriz de números chamada arr como parâmetro.
2. Inicializamos a variável sum com o valor 0, que armazenará a soma dos números positivos encontrados na matriz.
3. Em seguida, percorremos a matriz usando um loop for.
4. Dentro do loop, verificamos se o valor do elemento atual (arr[i]) é maior que 0. Se for positivo, somamos esse valor à variável sum.
5. Ao final do loop, a variável sum conterá a soma de todos os números positivos na matriz.
6. A função retorna o valor da variável sum.

No exemplo de uso, fornecemos uma matriz [1, -4, 7, 12] e chamamos a função somarPositivos com essa matriz. A função calcula a soma dos números positivos (1 + 7 + 12) e a exibe usando console.log. Se a matriz não contiver nenhum número positivo, a função retornará o valor 0, como especificado na nota.

```` javascript
// Exemplo de uso:
const numeros = [1, -4, 7, 12];
const somaPositivos = somarPositivos(numeros);
console.log('A soma dos números positivos é: ' + somaPositivos); // Saída: A soma dos números positivos é: 20
````

</details>

---

[Exercício no CodeWars.com](https://www.codewars.com/kata/5715eaedb436cf5606000381/train/javascript)
