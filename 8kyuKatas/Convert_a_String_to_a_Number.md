# CodeWars JavaScript Solutions

---

## Convert a Number to a String!


**Descrição**

Precisamos de uma função que possa transformar um número (inteiro) em uma string. Que maneiras de conseguir isso você conhece?

### Exemplos (entrada --> saída):
```123  --> "123"
999  --> "999"
-100 --> "-100"
```

---

### Código dado

```JavaScript
function numberToString(num) {
  // Return a string of the number here!
}
```
---
### Minha Solução

```JavaScript
function numberToString(num) {
  return num.toString();
}
```
<details>
<summary>Explicação</summary>
Esse código é uma função chamada numberToString que converte um número em uma string. Ele utiliza o método toString() disponível para objetos numéricos em JavaScript para realizar essa conversão.

O método toString() converte um número em sua representação como string. Ele retorna uma string que representa o número original.

No código fornecido, a função numberToString recebe um argumento num, que é o número a ser convertido em uma string. Em seguida, a função chama num.toString() para converter o número em uma string e retorna o resultado.

Exemplo:
```` javascript
const result = numberToString(42);
console.log(result); // Output: "42"
````

Nesse exemplo, a função numberToString recebe o número 42 e o converte em uma string usando toString(). O resultado é então retornado e atribuído à variável result, que é impressa no console.

O método toString() também pode receber um parâmetro opcional para especificar a base numérica da string resultante. Por exemplo, num.toString(2) converte o número em uma representação binária (base 2), enquanto num.toString(16) converte o número em uma representação hexadecimal (base 16). Se nenhum parâmetro for fornecido, assume-se a base 10.

É importante notar que a função numberToString retorna a representação da string do número fornecido. Se a função receber um valor não numérico, como null ou undefined, o comportamento pode ser imprevisível, pois o método toString() pode não estar disponível para esses tipos de valor.
</details>

---

[Exercício no CodeWars.com](https://www.codewars.com/kata/5265326f5fda8eb1160004c8/javascript)