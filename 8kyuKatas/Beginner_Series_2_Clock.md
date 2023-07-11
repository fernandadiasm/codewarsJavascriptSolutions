# CodeWars JavaScript Solutions

---

## Beginner Series #2 Clock


**Descrição**

Relógio mostra hhoras, mminutos e ssegundos depois da meia-noite.

Sua tarefa é escrever uma função que retorne a hora desde a meia-noite em milissegundos.

### Exemplos
```
h = 0
m = 1
s = 1

result = 61000
```

### Restrições de entrada
```
0 <= h <= 23
0 <= m <= 59
0 <= s <= 59
```

---

### Código dado

```JavaScript
function past(h, m, s){
}
```
---
### Minha Solução

```JavaScript
function past(h, m, s){
const convertHours = h * 60 * 60 * 1000;
const convertMinutes = m * 60 * 1000;
const convertSeconds = s * 1000;
return convertHours + convertMinutes + convertSeconds;
}
```

<details>
<summary>Explicação</summary>


```` javascript

````

</details>

---

[Exercício no CodeWars.com](https://www.codewars.com/kata/55f9bca8ecaa9eac7100004a/train/javascript)