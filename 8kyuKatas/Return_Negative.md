# CodeWars JavaScript Solutions

---

## Return Negative


**Descrição**

Nesta tarefa simples, você recebe um número e deve torná-lo negativo. Mas talvez o número já seja negativo?

### Exemplos
```
makeNegative(1);    // return -1
makeNegative(-5);   // return -5
makeNegative(0);    // return 0
makeNegative(0.12); // return -0.12
```
### Notas
O número já pode ser negativo, caso em que nenhuma alteração é necessária.
Zero (0) não é verificado para nenhum sinal específico. Zeros negativos não fazem sentido matemático.

---

### Código dado

```JavaScript
function makeNegative(num) {
  // Code?
}
```
---
### Minha Solução

```JavaScript
function makeNegative(num) {
  if(num <= 0){
    return num;
  }else{
    return -Math.abs(num);
  }
}
```

<details>
<summary>Explicação</summary>
A primeira coisa que precisa ser feita é escrever uma instrução if que verifica se num um valor menor ou igual a zero, porque não faz faz sentido transformar zero ou um número negativo em negativo, certo? Então, se a afirmação for verdadeira, ela não precisa ser alterada:

```` javascript
if(num <= 0){ 
    return num; 
}
````

Se o num não atender à primeira condição, então é preciso escrever uma instrução else que converte o valor positivo em negativo, é possível fazer isso da seguinte forma: converter o número para seu valor absoluto usando `Math.abs()`, e então multiplicando por -1 para torná-lo negativo, e esse valor negativo é retornado:

```` javascript
return -Math.abs(num);
````

exemplo de uso da função makeNegative:

``` javascript
const result1 = makeNegative(5);
console.log(result1); // Output: -5

const result2 = makeNegative(-2);
console.log(result2); // Output: -2

const result3 = makeNegative(0);
console.log(result3); // Output: 0 (não negativo, retorna o próprio número)

```
</details>

---

[Exercício no CodeWars.com](https://www.codewars.com/kata/55685cd7ad70877c23000102/train/javascript)