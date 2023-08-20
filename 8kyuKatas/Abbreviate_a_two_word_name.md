# CodeWars JavaScript Solutions

---

## Abbreviate a Two Word Name

**Descrição**

Escreva uma função para converter um nome em iniciais. Este kata leva estritamente duas palavras com um espaço entre elas.

A saída deve ser duas letras maiúsculas com um ponto separando-as.

Deve ficar assim:

```
Sam Harris=> S.H
Patrick Feeney=> P.F
```

---

### Código dado

```` JavaScript
function abbrevName(name) {
}
````

---

### Minha Solução

```` JavaScript
function abbrevName(name) {
  let nameSplit = name.split(" ");
  let firstLetter = nameSplit[0].charAt(0).toUpperCase();
  let secondLetter = nameSplit[1].charAt(0).toUpperCase();
  return `${firstLetter}.${secondLetter}`;
}
````

<details>
<summary>Explicação</summary>

`let nameSplit = name.split(" ");` - Divide o nome em partes separadas pelo espaço em branco e as armazena em uma matriz chamada nameSplit.

`let firstLetter = nameSplit[0].charAt(0).toUpperCase();` - Obtém a primeira letra do primeiro nome, converte-a para maiúscula e a armazena em firstLetter.

`let secondLetter = nameSplit[1].charAt(0).toUpperCase();` - Obtém a primeira letra do segundo nome, converte-a para maiúscula e a armazena em secondLetter.

`return ``${firstLetter}.${secondLetter}``;` - Retorna as iniciais com um ponto entre elas usando a interpolação de strings.

</details>


---

[Exercício no CodeWars.com](https://www.codewars.com/kata/57eadb7ecd143f4c9c0000a3/train/javascript)
