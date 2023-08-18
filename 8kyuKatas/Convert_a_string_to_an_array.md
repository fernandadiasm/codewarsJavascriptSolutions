# CodeWars JavaScript Solutions

---

## Convert a string to an array


**Descrição**

Escreva uma função para dividir uma string e convertê-la em uma matriz de palavras.

Exemplos (Entrada ==> Saída):

```
"Robin Singh" ==> ["Robin", "Singh"]
"I love arrays they are my favorite" ==> ["I", "love", "arrays", "they", "are", "my", "favorite"]
```

---

### Código dado

```` JavaScript
function stringToArray(string){
	// code code code
}
````

---
### Minha Solução

```` JavaScript
function stringToArray(string){
return string.split(' ');
}
```` 

<details>
<summary>Explicação</summary>

A função `split()` é usada para dividir uma string em partes, com base em um separador. Nesse caso, o espaço em branco dentro das aspas é um separador.

</details>

---

[Exercício no CodeWars.com](https://www.codewars.com/kata/57e76bc428d6fbc2d500036d/train/javascript)