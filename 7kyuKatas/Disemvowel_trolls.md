# CodeWars JavaScript Solutions

## Disemvowel Trolls
 
### Descrição

Trolls estão atacando sua seção de comentários!

Uma forma comum de lidar com essa situação é retirar todas as vogais dos comentários dos trolls, neutralizando a ameaça.

Sua tarefa é escrever uma função que recebe uma string e retorna uma nova string com todas as vogais removidas.

Por exemplo, a string "Este site é para perdedores LOL!" se tornaria "Ths wbst s fr lsrs LL!".

Nota: para este kata ynão é considerado uma vogal.
[Link do exercício.](https://www.codewars.com/kata/52fba66badcd10859f00097e/train/javascript)

---

### Código dado

```JavaScript
function disemvowel(str) {
  return str
}
```

---
### Minha Solução

```JavaScript
function disemvowel(str) {
  return str.replace(/[aeiouAEIOU]/g, '');
}
```

<details>
<summary><strong>Explicação</strong></summary>

1. A função disemvowel recebe a string str como argumento.

2. Em seguida, usamos o método `replace` para substituir todas as vogais encontradas na string pelo caractere vazio ' '.

3. Usamos uma expressão regular `[aeiouAEIOU]` para encontrar todas as ocorrências de vogais, tanto minúsculas quanto maiúsculas, na string.

* Os colchetes [ ] definem uma classe de caracteres, que especifica um conjunto de caracteres possíveis.

* Dentro da classe de caracteres, aeiouAEIOU lista todas as vogais em minúsculas e maiúsculas.

4. A flag g é usada após a expressão regular para indicar que queremos substituir todas as ocorrências de vogais na string, não apenas a primeira encontrada.

5. A função retorna a nova string resultante após a remoção das vogais.

Aqui está um exemplo de como usar essa função:
```` javascript
const textoOriginal = "Este site é para perdedores LOL!";
const textoSemVogais = removerVogais(textoOriginal);
console.log(textoSemVogais);
// saída:Ths st prt prddrs LL!
````

A função replace faz todo o trabalho pesado de buscar e substituir as vogais na string, tornando a solução simples e concisa.

Observação: a sintaxe geral do método replace é a seguinte:

```` javascript
stringOriginal.replace(valorAntigo, valorNovo);
````

Onde: 

- stringOriginal: A string original na qual você deseja realizar as substituições.

- valorAntigo: A string ou expressão regular que você deseja substituir.

- valorNovo: A string que será usada como substituição.

</details>

---

