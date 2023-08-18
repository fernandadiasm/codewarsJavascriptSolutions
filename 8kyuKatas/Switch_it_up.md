# CodeWars JavaScript Solutions

---

## Switch it up!


**Descrição**

Quando receber um número entre 0-9, retorne-o por extenso.

```
Entrada: 1
Saída: "Um"
```

Se a sua linguagem for compatível, tente usar uma instrução switch.

---

### Código dado

```` JavaScript
function switchItUp(number){
//Write your own Code!
}
````

---
### Minha Solução

```` JavaScript
function switchItUp(number){
    switch (number) {
        case 0:
            return "Zero";
        case 1:
            return "One";
        case 2:
            return "Two";
        case 3:
            return "Three";
        case 4:
            return "Four";
        case 5:
            return "Five";
        case 6:
            return "Six";
        case 7:
            return "Seven";
        case 8:
            return "Eight";
        case 9:
            return "Nine";
        default:
            return "Number out of range (0-9)";
    }
}
```` 

<details>
<summary>Explicação</summary>

Nesta função, usei a instrução `switch` para comparar o número fornecido com os valores de 0 a 9. Dependendo do valor, retorna a string correspondente por extenso. Se o número estiver fora do intervalo (0-9), retorna uma mensagem de erro.

</details>

---

[Exercício no CodeWars.com](https://www.codewars.com/kata/5808dcb8f0ed42ae34000031/train/javascript)