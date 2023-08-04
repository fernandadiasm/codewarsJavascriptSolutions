# CodeWars JavaScript Solutions

---

## Volume of a Cuboid


**Descrição**

Bob precisa de uma maneira rápida de calcular o volume de um paralelepípedo com três valores: o `length`, `width` e `height` do paralelepípedo. Escreva uma função para ajudar Bob com esse cálculo.

---

### Código dado

```` JavaScript
class Kata {
  static getVolumeOfCuboid(length, width, height) {
    // your code here
  }
}
````

---
### Minha Solução

```` JavaScript
class Kata {
  static getVolumeOfCuboid(length, width, height) {
        const volume = length * width * height;
    return volume;
  }
}
```` 

<details>
<summary>Explicação</summary>

A variável volume calcula o volume do paralelepípedo multiplicando o comprimento, largura e altura e armazena seu resultado. Por fim, usando o return, a variável retornará o valor do volume calculado.

</details>

---

[Exercício no CodeWars.com](https://www.codewars.com/kata/58261acb22be6e2ed800003a/train/javascript)