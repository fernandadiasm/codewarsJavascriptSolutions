# CodeWars JavaScript Solutions

---

## Area or Perimeter


**Descrição**
Você recebe o lengthe widthde um polígono de 4 lados. O polígono pode ser um retângulo ou um quadrado.
Se for um quadrado, retorne sua área. Se for um retângulo, retorne seu perímetro.

Exemplo(Entrada1, Entrada2 --> Saída):

```
6, 10 --> 32
3, 3 --> 9
```

Observação: para os propósitos deste kata, você assumirá que é um quadrado se seus lengthe widthforem iguais, caso contrário, é um retângulo.

---

### Código dado

```` JavaScript
const areaOrPerimeter = function(l , w) {
  // Return your answer
};
````

---
### Minha Solução

```` JavaScript
const areaOrPerimeter = function(l , w) {
  if (l === w) {
    return l * w; //area do quadrado
  } else {
    return 2 * (l + w) //perimetro de um retângulo
  }
};
```` 

<details>
<summary>Explicação</summary>



</details>

---

[Exercício no CodeWars.com](https://www.codewars.com/kata/5ab6538b379d20ad880000ab/train/javascript)