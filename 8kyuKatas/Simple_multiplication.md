# CodeWars JavaScript Solutions

---

## Simple multiplication


**Descrição**

Este kata consiste em multiplicar um determinado número por oito se for um número par e por nove caso contrário.

---

### Código dado

```JavaScript
function simpleMultiplication(number) {
    // your code........
}
```

---
### Minha Solução

```JavaScript
function simpleMultiplication(number) {
      if (number % 2 === 0) {
    return number * 8;
  } else {
    return number * 9;
  }
}
```

<details>
<summary>Explicação</summary>

A função `simpleMultiplication` verifica se o número é par usando o operador % (módulo). Se o resto da divisão por 2 for igual a zero, o número é par, e então o número é multiplicado por 8. Caso contrário, o número é ímpar, e é multiplicado por 9.

</details>

---

[Exercício no CodeWars.com](https://www.codewars.com/kata/583710ccaa6717322c000105/train/javascript)