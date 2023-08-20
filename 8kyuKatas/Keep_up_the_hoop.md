# CodeWars JavaScript Solutions

---

## Keep up the hoop


**Descrição**

Alex acabou de ganhar um novo bambolê, ele adora, mas se sente desanimado porque seu irmãozinho é melhor do que ele

Escreva um programa onde Alex possa inserir (n) quantas vezes o aro dá voltas e ele retornará uma mensagem encorajadora :)

Se Alex conseguir 10 ou mais argolas, retorne a string "Great, now move on to tricks".
Se ele não conseguir 10 aros, devolva a string "Keep at it until you get it".

---

### Código dado

```` JavaScript
function hoopCount (n) {
   //your code goes here    
}
````

---
### Minha Solução

```` JavaScript
function hoopCount(n) {
    if (n >= 10) {
        return "Great, now move on to tricks";
    } else {
        return "Keep at it until you get it";
    }
}
```` 

<details>
<summary>Explicação</summary>



</details>

---

[Exercício no CodeWars.com](https://www.codewars.com/kata/55cb632c1a5d7b3ad0000145/train/javascript)