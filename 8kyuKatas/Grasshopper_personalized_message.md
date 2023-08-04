# CodeWars JavaScript Solutions

---

## Grasshopper - Personalized Message

**Descrição**

Crie uma função que dê uma saudação personalizada. Esta função recebe dois parâmetros: namee owner.

Use condicionais para retornar a mensagem apropriada:

````
caso ---> retornar
nome é igual a dono ---> 'Hello boss'
de outra forma ---> 'Hello guest'
````

---

### Código dado

```` JavaScript
function greet (name, owner) {
}
````

---

### Minha Solução

```` JavaScript
function greet (name, owner) {
      if (name === owner) {
        return 'Hello boss';
    } else {
        return 'Hello guest';
    }
}
````

<details>
<summary>Explicação</summary>

A função é definida usando a palavra-chave function, seguida do nome da função `greet`. Em seguida, estão os parâmetros entre parênteses (name e owner), que são as informações que a função espera receber como entrada.

Dentro da função, usei um if para fazer uma verificação condicional. A condição é dada por `name === owner`, que verifica se o valor da variável name é igual ao valor da variável owner. Se essa condição for verdadeira, o bloco de código dentro do if será executado, e a função retornará a string 'Olá chefe'. Caso contrário, o bloco de código dentro do else será executado, e a função retornará a string 'Olá convidado'.

Exemplo: 
```` javascript
let nomeUsuario = 'Alice';
let nomeDono = 'Bob';
console.log(great(nomeUsuario, nomeDono)); // Saída: 'Olá convidado'

nomeUsuario = 'Bob';
nomeDono = 'Bob';
console.log(great(nomeUsuario, nomeDono)); // Saída: 'Olá chefe'
````

</details>

---

[Exercício no CodeWars.com](https://www.codewars.com/kata/5772da22b89313a4d50012f7/train/javascript)
