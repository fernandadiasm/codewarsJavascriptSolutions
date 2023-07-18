# CodeWars JavaScript Solutions

---

## Ordem Inversa da Lista


**Descrição**

Neste kata você criará uma função que recebe uma lista e retorna uma lista com a ordem inversa.

### Exemplos (Input -> Output)
```
* [1, 2, 3, 4]  -> [4, 3, 2, 1]
* [9, 2, 0, 7]  -> [7, 0, 2, 9]
```


---

### Código dado

```JavaScript
function reverseList(list) {
}
```

---
### Minha Solução

```JavaScript
function reverseList(list) {
return list.reverse()
}
```

<details>
<summary>Explicação</summary>
O método reverse() é uma função embutida em arrays (listas) em JavaScript que inverte a ordem dos elementos de um array. Ele modifica o array original, alterando a posição dos elementos.

Ao chamar reverse() em um array, a ordem dos elementos é revertida. O primeiro elemento se torna o último e o último elemento se torna o primeiro, e assim por diante. O método reverse() afeta o array original e retorna uma referência para o próprio array invertido.
</details>

---

[Exercício no CodeWars.com](https://www.codewars.com/kata/53da6d8d112bd1a0dc00008b)