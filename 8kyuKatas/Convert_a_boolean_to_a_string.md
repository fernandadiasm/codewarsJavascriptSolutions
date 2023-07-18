# CodeWars JavaScript Solutions

---

## Convert a Boolean to a String


**Descrição**

Implemente uma função que converta o valor booleano fornecido em sua representação de string.

Nota: Apenas entradas válidas serão dadas.

---

### Código dado

```JavaScript
function booleanToString(b){
  //your code here
}
```

---
### Minha Solução

```JavaScript
function booleanToString(b){
  return b.toString()
}
```

<details>
<summary>Explicação</summary>

Nesta função, usei o método `toString()` para converter o valor booleano em sua representação de string. O método toString() é uma função embutida em valores booleanos em JavaScript que retorna a representação em string do valor.

Testando a função com alguns exemplos:

```` javascript
console.log(booleanToString(true));   // Output: "true"
console.log(booleanToString(false));  // Output: "false"
console.log(booleanToString(0));      // Output: "false" (0 é considerado falso)
console.log(booleanToString(1));      // Output: "true" (qualquer valor diferente de 0 é considerado verdadeiro)
````

A função irá retornar a representação em string correspondente ao valor booleano fornecido.

</details>

---

[Exercício no CodeWars.com](https://www.codewars.com/kata/551b4501ac0447318f0009cd/train/javascript)