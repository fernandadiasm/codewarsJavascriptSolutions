# CodeWars JavaScript Solutions

---

## Convert a String to a Number!


**Descrição**

Precisamos de uma função que possa transformar uma string em um número. Que maneiras de conseguir isso você conhece?

Observação: não se preocupe, todas as entradas serão strings e cada string é uma representação perfeitamente válida de um número inteiro.

### Exemplos
```"1234" --> 1234
"605"  --> 605
"1405" --> 1405
"-7" --> -7 
```

---

### Código dado

```JavaScript
const stringToNumber = function(str){
  // put your code here
  return null;
}
```
---
### Minha Solução

```JavaScript
const stringToNumber = function(str){
  return parseInt(str);
}
```
<details>
<summary>Explicação</summary>

A função parseInt() em JavaScript converte uma string em um número inteiro. Ela analisa a string fornecida e retorna um número com base no conteúdo da string. Se a string contiver apenas dígitos numéricos, parseInt() retornará o valor inteiro equivalente. Se houver outros caracteres não numéricos na string, eles serão ignorados durante a conversão.

No código fornecido, a função stringToNumber recebe um argumento str, que é a string a ser convertida em número. Em seguida, a função chama parseInt(str) para converter a string em um número inteiro e retorna o resultado.

Nesse exemplo, a função stringToNumber recebe a string "42" e a converte em um número inteiro 42 usando parseInt(). O resultado é então retornado e atribuído à variável result, que é impressa no console:

```` javascript
var result = stringToNumber("42");
console.log(result); // Output: 42
````
</details>

---

[Exercício no CodeWars.com](https://www.codewars.com/kata/56676e8fabd2d1ff3000000c)