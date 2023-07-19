# CodeWars JavaScript Solutions

---

## Calculate average


**Descrição**

Escreva uma função que calcule a média dos números em uma determinada lista.

Nota: Arrays vazios devem retornar 0.

---

### Código dado

```` JavaScript
function findAverage(array) {
    return 0;
}
````

---
### Minha Solução

```` JavaScript
function findAverage(array) {
    const totalElements = array.length;
  
  if (totalElements === 0) {
    return 0;
  }
  
  const sum = array.reduce((accumulator, element) => accumulator + element, 0);
  return sum / totalElements;
}
````

<details>
<summary>Explicação</summary>

 Para calcular a média dos números em uma lista, é necessário somar todos os elementos do array e depois dividir pelo número de elementos. Se o array estiver vazio, a função deve retornar 0, conforme especificado.

 Na função `findAverage`, a lista de entrada é verificada para saber se está vazia (ou seja, o comprimento do array é igual a 0). Se estiver vazia, a função retorna 0 imediatamente. Caso contrário, a função usa o método `reduce()` para somar todos os elementos da lista e, em seguida, divide a soma pelo número total de elementos para obter a média. O resultado é retornado como o valor da média.

Exemplo de uso:

```` javascript
const listaDeNumeros = [10, 20, 30, 40, 50];
const media = findAverage(listaDeNumeros);
console.log(media); 
// Saída: 30 (a média dos números é (10 + 20 + 30 + 40 + 50) / 5 = 30)
````

</details>

---

[Exercício no CodeWars.com](https://www.codewars.com/kata/57a2013acf1fa5bfc4000921/train/javascript)