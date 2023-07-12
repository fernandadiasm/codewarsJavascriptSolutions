# CodeWars JavaScript Solutions

## Reverse words
 
### Descrição

Conclua a função que aceita um parâmetro de string e inverte cada palavra na string. Todos os espaços na string devem ser mantidos. 
[Link do exercício.](https://www.codewars.com/kata/5259b20d6021e9e14c0010d4/train/javascript)

### Exemplos
```
"This is an example!" ==> "sihT si na !elpmaxe"
"double  spaces"      ==> "elbuod  secaps"
```


---

### Código dado

```JavaScript
function reverseWords(str) {
  // Go for it
}
```
---
### Minha Solução

```JavaScript
function reverseWords(str) {
    return str 
.split('') 
.reverse() 
.join('') 
.split(' ') 
.reverse() 
.join(' '); 
}
```

<details>
<summary><strong>Explicação</strong></summary>

A primeira coisa que precisamos fazer é usar `str.split('')` para retornar uma matriz de caracteres. Para isso, você pode usar .split('') ou .split(' '). **Se você estiver usando a divisão sem espaço entre as aspas, ela será dividida após cada caractere. Se você usar split com um espaço entre as aspas, ele será dividido a cada espaço na string**. Para este desafio, escolhi usar .split('').

```` javascript
function reverseWords(str) { 
    return str.split('') 
}  // Saída: [‘T’, ‘h’, ‘e’, ‘ ‘, ‘q’, ‘u’, ’i’, ’c’, ’k’,’ ‘, ‘b’, ’r’, ’o’, ’w’, ’n’, ’ ‘, ’f’, ’o’, ’x’, ’ ‘, ’j’, ’u’, ’m’, ’p’, ’s’, ’ ‘, ’o’, ’v’, ’e’, ’r’, ’ , ’t’, ’h’, ’e’, ’ ‘, ’l’, ’a’, ’z’, ’y’, ’ ‘, ’d’, ’o’, ’g’, ’.’].
````

Agora que temos essa enorme matriz dividida em cada caractere, podemos adicionar `.reverse()` e inverter as letras. Ao usar os métodos .split() e .reverse(), você não precisa criar variáveis ​​diferentes e encadeá-las, basta adicioná-las como: str.split('').reverse(). Vamos verificar a saída e ver o que temos:

```` javascript
function reverseWords(str) { 
    return str.split('').reverse() 
} //Saída:[‘.’, ’g’, ’o’, ’d’, ’ ‘, ’y’, ’z’, ’a’, ’l’, ’ ‘, ’e’, ’h’, ’t’, ’ ‘, ’r’, ’e’, ’v’, ’o’, ’ ‘, ’s’, ’p’, ’m’, ’u’, ’j’, ’ ‘, ’x’, ’o’, ’f’, ’ ‘, ’n’, ’w’, ’o’, ’r’, ’b’, ’ ‘, ’k’, ’c’, ’I’, ’u’, ’q’, ’ ‘, ’e’, ’h’, ’T’]
````

Agora é preciso colocar o array em uma string para que possamos fazer mais algum trabalho nela. Devemos usar o `.join()` exatamente como usamos o .split(). Para isso, precisamos adicionar o mesmo argumento ao .join() que fizemos em .split():

```` javascript
function reverseWords(str) { 
    return str.split('').reverse().join('') 
} //Saída:‘.god yzal eht revo spmuj xof nworb kciuq ehT’
````

As palavras estão invertidas, mas agora estão nas posições erradas. Olhando para o objetivo, precisamos colocar “ehT” de volta no primeiro lugar e “.god” de volta ao último lugar. Para fazer isso, precisamos dividir a string de volta em uma matriz para que possamos invertê-la novamente. Desta vez vamos usar `.split(' ')`. Certifique-se de que haja um espaço entre as aspas, isso nos permite dividir nos espaços em vez de depois de cada caractere.

```` javascript
function reverseWords(str) { 
    return str.split('').reverse().join('').split(' ') 
} // Saída[ ‘.god’, ‘yzal’, ‘eht’, ‘revo’, ‘spmuj’, ‘xof’, ‘nworb’, ‘kciuq’, ‘ehT’ ]
````

Agora que dividimos a string em um array, podemos inverter a ordem das palavras. `.reverse()` funciona invertendo a ordem de cada item no array, então quando usarmos agora ele não irá mudar as letras em cada string, apenas irá inverter a posição do índice de cada string no array.

```` javascript
function reverseWords(str) { 
    return str.split('').reverse().join('').split(' ').reverse() 
} // Saída [ ‘ehT’, ‘kciuq’, ‘nworb’, ‘xof’, ‘spmuj’, ‘revo’, ‘eht’, ‘yzal’, ‘.god’ ]
````

A última coisa que precisamos fazer para concluir este desafio é converter esse array de volta em uma string, faremos isso usando `.join()` novamente. A última .split(‘ ‘)que usamos tínhamos um espaço entre as aspas, quando usarmos `.join(' ')` precisará ser igual.
```` javascript
function reverseWords(str) { 
return str.split('').reverse().join('').split(' ').reverse().join(' ') 
} //Saída ‘ehT kciuq nworb xof spmuj revo eht yzal .god’ 
````

</details>

---

