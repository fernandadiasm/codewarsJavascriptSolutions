# CodeWars JavaScript Solutions

---

## Keep Hydrated!


**Descrição**

Nathan adora andar de bicicleta.

Como Nathan sabe que é importante se manter hidratado, ele bebe 0,5 litro de água por hora de pedalada.

Você recebe o tempo em horas e precisa retornar o número de litros que Nathan vai beber, arredondado para o menor valor.

### Exemplos
```
time = 3 ----> litres = 1

time = 6.7---> litres = 3

time = 11.8--> litres = 5
```


---

### Código dado

```JavaScript
function litres(time) {
  return 0;
}
```
---

### Minha Solução

```JavaScript
function litres(time) {
  return Math.floor( time / 2);
}
```

<details>
<summary>Explicação</summary>
Essa função, chamada litres, calcula a quantidade de litros de água consumida com base no tempo em horas. Ela faz o seguinte:

1. Divide o tempo fornecido por 2. Isso é feito pela expressão time / 2. Essa divisão por 2 é utilizada para representar o consumo médio de água por hora. Por exemplo, se uma pessoa consome 1 litro de água a cada 2 horas, a divisão por 2 é utilizada para calcular quantos litros ela consumiu no tempo especificado.

2. O resultado da divisão é arredondado para baixo para o número inteiro mais próximo. Isso é feito pela função Math.floor(). O arredondamento para baixo é usado para garantir que o resultado seja um número inteiro, representando a quantidade de litros consumidos, sem considerar frações.

3. O resultado final, que representa a quantidade de litros consumidos, é retornado pela função.

Por exemplo:

Se chamar litres(5), a função retornará 2, porque 5 dividido por 2 é igual a 2.5, e o arredondamento para baixo resulta em 2.

Se chamar litres(8), a função retornará 4, porque 8 dividido por 2 é igual a 4.

Essa função é útil quando se precisa calcular a quantidade aproximada de litros de água consumida com base em um determinado tempo. Ela assume que o consumo é constante e igual a 1 litro a cada 2 horas.
</details>

---

[Exercício no CodeWars.com](https://www.codewars.com/kata/582cb0224e56e068d800003c/train/javascript)