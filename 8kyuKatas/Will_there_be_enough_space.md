# CodeWars JavaScript Solutions

---

## Will there be enough space?

**Descrição**

A história:
Bob está trabalhando como motorista de ônibus. No entanto, ele se tornou extremamente popular entre os moradores da cidade. Com tantos passageiros querendo embarcar em seu ônibus, ele às vezes tem que enfrentar o problema de não haver espaço suficiente no ônibus! Ele quer que você escreva um programa simples dizendo a ele se ele conseguirá acomodar todos os passageiros.

**Visão geral da tarefa:**

Você tem que escrever uma função que aceite três parâmetros:

* **cap** - a quantidade de pessoas que o ônibus comporta, excluindo o motorista.

* **on** - o número de pessoas no ônibus excluindo o motorista.

* **wait** - o número de pessoas esperando para entrar no ônibus, excluindo o motorista.

* Se houver espaço suficiente, retorne 0, e se não houver, retorne o número de passageiros que ele não pode levar.

**Exemplos de uso:**

`````
cap = 10, on = 5, wait = 5 --> 0 # He can fit all 5 passengers
cap = 100, on = 60, wait = 50 --> 10 # He can't fit 10 of the 50 waiting
`````

---

### Código dado

````JavaScript
function enough(cap, on, wait) {
}
````

---

### Minha Solução

```` JavaScript
function enough(cap, on, wait) {
    const totalPassengers = on + wait;
  
  if (totalPassengers <= cap) {
    return 0;
  } else {
    return totalPassengers - cap;
  }
}
````

<details>
<summary>Explicação</summary>

A função enough recebe os mesmos três parâmetros: cap (capacidade do ônibus), on (número de passageiros no ônibus excluindo o motorista) e wait (número de pessoas esperando para entrar no ônibus excluindo o motorista). Em seguida, ela calcula o total de passageiros somando o número atual de passageiros (on) com o número de pessoas esperando (wait).

Após calcular o total de passageiros, a função verifica se ele é menor ou igual à capacidade do ônibus (cap). Se for, significa que há espaço suficiente, e a função retorna 0. Caso contrário, a função retorna a diferença entre o total de passageiros e a capacidade do ônibus, que representa o número de passageiros que não podem entrar.

</details>

---

[Exercício no CodeWars.com](https://www.codewars.com/kata/5875b200d520904a04000003/train/javascript)
