# CodeWars JavaScript Solutions

---

## Convert number to reversed array of digits


**Descrição**
Dado um número aleatório não negativo, você deve retornar os dígitos desse número em uma matriz na ordem inversa.

Exemplo (Entrada => Saída):
```
35231 => [1,3,2,5,3]
0 => [0]
```

---

### Código dado

```` JavaScript
function digitize(n) {
}
````

---
### Minha Solução

``` JavaScript
function digitize(n) {
 return n.toString().split('').reverse().map(Number);
}
```

<details>
<summary>Explicação</summary>

**n.toString()**: converte o número 'n' em uma string para poder usar o método `split` para conseguir dividir os dígitos.

**.slipt()**: o método `split('')` é usado na string convertida. Passar uma string vazia como argumento faz com que a string seja dividida em um array de caracteres individuais (os caracteres se tornam elementos separados de um array).

**.reverse()**: o método `reverse()` inverte a ordem dos elementos no array.

**.map(Number)**: o método `map()` é usado para aplicar a função `Number` em cada elemento no array, converte cada caractere em um número.

**digitize**: a função `digitize` combina todas essas etapas anteriores para realizar a conversão dos dígitos de um número em uma matriz na ordem inversa.

</details>

---

[Exercício no CodeWars.com](https://www.codewars.com/kata/5583090cbe83f4fd8c000051/train/javascript)