# CodeWars JavaScript Solutions

---

## Even or Odd


**Descrição**

Crie uma função que receba um número inteiro como argumento e retorne "Even"para números pares ou "Odd"ímpares.

---

### Código dado

```` JavaScript
function evenOrOdd(number) {
  
}
````

---
### Minha Solução

```` JavaScript
function evenOrOdd(number) {
    if (number % 2 === 0) {
        return "Even";
    } else {
        return "Odd";
    }
}
```` 

<details>
<summary>Explicação</summary>

`number % 2 === 0`; - verifica se o número é divisível por 2 sem deixar um resto, ou seja, se é par.

Se a condição for verdadeira, a função retorna "Even" (par); caso contrário, retorna "Odd" (ímpar).

</details>

---

[Exercício no CodeWars.com](https://www.codewars.com/kata/53da3dbb4a5168369a0000fe/train/javascript)