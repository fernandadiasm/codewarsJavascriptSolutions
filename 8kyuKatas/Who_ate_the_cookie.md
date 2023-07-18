# CodeWars JavaScript Solutions

---

## Who ate the cookie?


**Descrição**

Para esse problema você deve criar um programa que diga quem comeu o último biscoito. Se a entrada for uma string, então "Zach" comeu o cookie. Se a entrada for float ou int, então "Monica" comeu o cookie. Se a entrada for qualquer outra coisa, "o cachorro" comeu o biscoito. A forma de retornar a declaração é: "Quem comeu o último biscoito? Foi (nome)!"

Ex: Entrada = "oi" --> Saída = "Quem comeu o último biscoito? Foi Zach! (A razão pela qual você retorna Zach é porque a entrada é uma string)

Nota: Certifique-se de retornar a mensagem correta com os espaços e pontuação corretos.

---

### Código dado

```JavaScript
function cookie(x){
  // ...
}
```

---
### Minha Solução

```JavaScript
function cookie(x){
    if (typeof x === 'string') {
    return "Who ate the last cookie? It was Zach!";
  } else if (typeof x === 'number') {
    return "Who ate the last cookie? It was Monica!";
  }  else {
    return "Who ate the last cookie? It was the dog!";
  }
}
```

<details>
<summary>Explicação</summary>

Nesta função, usei o operador typeof para verificar o tipo da entrada e, com base nisso, retorna a mensagem adequada.

</details>

---

[Exercício no CodeWars.com](https://www.codewars.com/kata/55a996e0e8520afab9000055)