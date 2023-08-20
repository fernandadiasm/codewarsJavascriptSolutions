# CodeWars JavaScript Solutions

---

## Remove exclamation marks


**Descrição**

Escreva a função RemoveExclamationMarks que remove todos os pontos de exclamação de uma determinada string.
---

### Código dado

```` JavaScript
function removeExclamationMarks(s) {
  return '';
}
````

---
### Minha Solução

```` JavaScript
function removeExclamationMarks(s) {
   return s.replace(/!/g, '');
}
```` 

<details>
<summary>Explicação</summary>

Retirando o sinal de exclamação: A função `replace()` é usada para substituir um padrão por outro em uma string. Nesse caso, usei a `expressão regular /!/g` como padrão para encontrar todos os pontos de exclamação na string e substituí-los por uma string vazia '', o que efetivamente remove os pontos de exclamação.

</details>

---

[Exercício no CodeWars.com](https://www.codewars.com/kata/57a0885cbb9944e24c00008e/train/javascript)