# CodeWars JavaScript Solutions

---

## The Feast of Many Beasts


**Descrição**

Todos os animais estão em festa! Cada animal traz um prato. A regra é apenas uma: o prato deve começar e terminar com as mesmas letras do nome do animal. Por exemplo, a garça azul está trazendo alho naan e o chapim está trazendo bolo de chocolate.

Escreva uma função feastque receba o nome e o prato do animal como argumentos e retorne verdadeiro ou falso para indicar se o animal pode levar o prato para o banquete.

Suponha que beaste dishsejam sempre strings minúsculas e que cada uma tenha pelo menos duas letras. beaste dishpode conter hífens e espaços, mas estes não aparecerão no início ou no final da string. Eles não conterão numerais.

---

### Código dado

```` JavaScript
function feast(beast, dish) {
}
````

---
### Minha Solução

```` JavaScript
function feast(beast, dish) {
return beast[0] === dish[0] && beast[beast.length - 1] === dish[dish.length - 1]
}
```` 

<details>
<summary>Explicação</summary>

A função feast recebe dois argumentos: beast e dish, que são strings. O objetivo dessa função É uma função é comparar caracteres nas posições iniciais e finais das strings. Se ambas as condições forem verdadeiras, a função retorna true; caso contrário, ela retorna false.

1. **beast[0] === dish[0]**:  Verifica se o primeiro caractere (letra) da string beast é igual ao primeiro caractere da string dish.

2. **beast[beast.length - 1] === dish[dish.length - 1]**: Verifica se o último caractere (letra) da string beast é igual ao último caractere da string dish. Para fazer isso, a função usa `beast.length - 1` para acessar o último caractere da string beast e `dish.length - 1` para acessar o último caractere da string dish. Entendendo a lógica do passo dois:

* `beast.length`: Retorna o comprimento da string beast, que é o número total de caracteres na string. No contexto da sua função, isso é importante para saber quantos caracteres existem em beast.
**Retorna o comprimento da string beast, que é 6 no caso da palavra "animal".**

* `beast.length - 1`: Esta expressão calcula a posição do último caractere na string beast. Como as posições de caracteres em uma string são baseadas em zero (ou seja, o primeiro caractere está na posição 0, o segundo na posição 1 e assim por diante), subtrair 1 do comprimento da string nos dá a posição do último caractere. **Calcula a posição do último caractere, que é 6 - 1 = 5.**

* `beast[beast.length - 1]`: Agora que temos a posição do último caractere, podemos usar esta expressão para acessar o último caractere da string beast. O [beast.length - 1] indica que queremos o caractere na posição calculada anteriormente. **Acessa o caractere na posição 5 da string beast, que é o último caractere.**

Exemplo: 
``` javascript
const beast = "animal";
const ultimoCaractere = beast[beast.length - 1];
console.log(ultimoCaractere); // Isso irá imprimir "l", que é o último caractere da palavra "animal"
```

Obs: o mesmo se aplica á string `dish`.

3. Se ambas as condições acima forem verdadeiras (ou seja, a primeira e a última letra das duas strings forem iguais), a função retorna true, indicando que o "banquete" está completo.

4. Se qualquer uma das condições não for atendida (ou seja, a primeira letra ou a última letra das duas strings forem diferentes), a função retorna false, indicando que o "banquete" não está completo.


</details>

---

[Exercício no CodeWars.com](https://www.codewars.com/kata/5aa736a455f906981800360d/train/javascript)