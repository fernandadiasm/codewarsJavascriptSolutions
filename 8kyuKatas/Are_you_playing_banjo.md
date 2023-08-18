# CodeWars JavaScript Solutions

---

## Are You Playing Banjo?



**Descrição**
Crie uma função que responda à pergunta "Você está tocando banjo?".
Se o seu nome começa com a letra "R" ou "r" minúsculo, você está tocando banjo!

A função usa um nome como seu único argumento e retorna uma das seguintes strings:

```
name + " plays banjo" 
name + " does not play banjo"
```

Os nomes fornecidos são sempre cadeias de caracteres válidas.

---

### Código dado

```` JavaScript
function areYouPlayingBanjo(name) {
  // Implement me
  return name;
}
````

---
### Minha Solução

```` JavaScript
function areYouPlayingBanjo(name) {
  if (name[0].toLowerCase() === 'r') {
  return name + ' plays banjo';
  } else {
    return name + ' does not play banjo';
  }
}
```` 

<details>
<summary>Explicação</summary>

Verificação da primeira letra: Dentro da função, utilizei a propriedade `name[0]` para acessar o primeiro caractere do nome fornecido como argumento. Em seguida, usei o método `toLowerCase()` para transformar esse caractere em minúsculo, garantindo que seja possível fazer uma comparação sem considerar a diferenciação entre maiúsculas e minúsculas.

Decisão com base na letra inicial: Dentro do bloco if, verifiquei se o primeiro caractere é igual a "r" minúsculo. Se for, retorna a mensagem indicando que a pessoa está tocando banjo, concatenando o nome com a frase.

Caso contrário: Se o primeiro caractere não for "r", o bloco else é executado e retorna a mensagem de que a pessoa não está tocando banjo.

Teste da função: Para verificar se a função está funcionando corretamente. Chamei a função com diferentes nomes e imprimi as saídas correspondentes.

``` Javascript
console.log(areYouPlayingBanjo("Ringo"));  // Saída: "Ringo plays banjo"
console.log(areYouPlayingBanjo("John"));   // Saída: "John does not play banjo"
console.log(areYouPlayingBanjo("rachel")); // Saída: "rachel plays banjo"
console.log(areYouPlayingBanjo("Megan"));  // Saída: "Megan does not play banjo"
```

</details>

---

[Exercício no CodeWars.com](https://www.codewars.com/kata/53af2b8861023f1d88000832/train/javascript)