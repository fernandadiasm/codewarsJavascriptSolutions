# CodeWars JavaScript Solutions

---

## No zeros for heros


**Descrição**

Números que terminam com zeros são chatos.

Eles podem ser divertidos em seu mundo, mas não aqui.

Livrar-se deles. Só os finais.

````
1450 -> 145
960000 -> 96
1050 -> 105
-1050 -> -105
````

Zero sozinho é bom, não se preocupe com isso. Pobre cara de qualquer maneira

---

### Código dado

```JavaScript
function noBoringZeros(n) {
  }
```

---
### Minha Solução

```JavaScript
function noBoringZeros(n) {
   if (n === 0) {
    return 0;
  }

  while (n % 10 === 0) {
    n = n / 10;
  }

  return n;
  }
```

<details>
<summary>Explicação</summary>

Nesta função, comecei com uma verificação especial para o caso em que o número é zero. Se o número for zero, simplesmente retorna zero, pois ele não tem zeros finais a serem removidos.

Em seguida, usei um loop while para dividir o número por 10 repetidamente enquanto o resto da divisão (numero % 10) for igual a zero. Isso remove os zeros finais do número até que chegue a um dígito diferente de zero no final.

Usando a função com alguns exemplos:

```` javascript
console.log(removerZerosFinais(1450));     // Output: 145
console.log(removerZerosFinais(960000));   // Output: 96
console.log(removerZerosFinais(1050));     // Output: 105
console.log(removerZerosFinais(-1050));    // Output: -105
console.log(removerZerosFinais(0));        // Output: 0
````

</details>

---

[Exercício no CodeWars.com](https://www.codewars.com/kata/570a6a46455d08ff8d001002/train/javascript)