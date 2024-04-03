# UNIFOR
**Nome**: Juan Doth
**Disciplina**: Raciocínio logico algorítmico

##Questão 1
###Fluxograma
```mermaid
flowchart TD
A([Inicio]) --> B[/Digite quatro números inteiros/]
B --> C(soma = número 1 + número 2 + número 3 + número 4)
C --> D([soma / 4])
D --> F[Mostrar Média]
F --> G([FIM])
```
#### Pseudocódigo (1.0 ponto)

```java
ALGORTIMO Media
DECLARE num1, num2, num3, num4: REAL

INICIO

    // Insira seu comentário
    ESCREVA "Digite o número 1:"

    // Insira seu comentário
    LEIA num1

    // Insira seu comentário
    ESCREVA "Digite o número 2:"

    // Insira seu comentário
    LEIA num2

    // Insira seu comentário
    ESCREVA "Digite o número 3:"

    // Insira seu comentário
    LEIA num3

    // Insira seu comentário
    ESCREVA "Digite o número 4:"

    // Insira seu comentário
    LEIA num4

    // Insira seu comentário
    media <- (num1 + num2 + num3 + num4)/4
    ESCREVA "A média é", media

FIM
```

#### Teste de mesa (0.5 ponto)

| num1 | num2 | num3 | num4 | saída | 
| --   | --   | --   | --   | --    | 
| 0.25 | 0.25 | 2.50 | 1.00 | 1.00  | 
