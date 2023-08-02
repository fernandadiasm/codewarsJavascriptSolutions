# CodeWars JavaScript Solutions

---

## Sentence Smash

**Descrição**

Escreva uma função que pegue um array de palavras e as junte em uma frase e retorne a frase. Você pode ignorar qualquer necessidade de limpar palavras ou adicionar pontuação, mas deve adicionar espaços entre cada palavra. Tenha cuidado, não deve haver um espaço no início ou no final da frase!

**Exemplo**

````
['hello', 'world', 'this', 'is', 'great']  =>  'hello world this is great'
````

---

### Código dado

```` JavaScript
function smash (words) {
   return ""
};
````

---

### Minha Solução

```` JavaScript
function smash (words) {
  if(!words || words.length === 0){
   return '';
}
const phrase = words.join(' ');
return phrase
  }
````

<details>
<summary>Explicação</summary>

```` javascript
function juntarPalavrasEmFrase(palavras) {
  // Verifica se o array está vazio ou é nulo
  if (!palavras || palavras.length === 0) {
    return '';
  }

  // Usa o método join() para unir as palavras em uma frase
  const frase = palavras.join(' ');

  return frase;
}

// Exemplo de uso:
const arrayDePalavras = ['Esta', 'é', 'uma', 'frase', 'exemplo'];
const fraseResultante = juntarPalavrasEmFrase(arrayDePalavras);
console.log(fraseResultante); // Saída: "Esta é uma frase exemplo"

````
</details>

---

[Exercício no CodeWars.com](https://www.codewars.com/kata/53dc23c68a0c93699800041d/train/javascript)
