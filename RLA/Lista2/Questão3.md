# UNIFOR
**Nome**: Juan Doth
**Disciplina**: Raciocínio logico algorítmico

##Questão 3
###Fluxograma
```mermaid
flowchart TD
A([Inicio]) --> B[/digite um número 1/]
B --> C[/Digite um operador, +, -, *, / /]
C -->D[/Digite um número 2/]
D -->E{Se for = +}
E -- sim -->F[N1+N2]
E -- não --> H{Se for = -}
F --> G(resultado)
G --> Z([FIM])
H -- sim --> I[N1 - N2]
I --> J(Resultado)
J --> Z
H -- não --> K{Se for = *}
K -- sim --> L[N1 * N2]
L --> M(Resultado)
M --> Z
K -- não --> N{Se for = /}
N --> O(N2 for = 0)
O -- sim -->P[não pode ser dividido]
O -- não --> Q[N1/N2]
Q --> R(Resultado)
R --> Z
```
#### Pseudocódigo (1.0 ponto)

```java
ALGORITMO CalculadoraSimples
DECLARE op: INTEIRO; num1,num2,res: REAL

INICIO

    // Insira seu comentário
    ESCREVA "Operações válidas: 1(soma), 2(subtração), 3(multiplicação) e 4(divisão)"

    // Insira seu comentário
    ESCREVA "Digite uma operação:"

    // Insira seu comentário
    LEIA op

    // Insira seu comentário
    ESCREVA "Digite um número:"
    LEIA num1

    // Insira seu comentário
    ESCREVA "Digite outro número:"
    LEIA num2

    // Insira seu comentário
    ESCOLHA

        // Insira seu comentário
        CASO op == 1

            // Insira seu comentário
            res = num1 + num2

            // Insira seu comentário
            ESCREVA num1, "+", num2, "=", res

        // Insira seu comentário
        CASO op == 2

            // Insira seu comentário
            res = num1 - num2

            // Insira seu comentário
            ESCREVA num1, "-", num2, "=", res

        // Insira seu comentário
        CASO op == 3

            // Insira seu comentário
            res = num1 * num2

            // Insira seu comentário
            ESCREVA num1, "*", num2, "=", res

        // Insira seu comentário
        CASO op == 4

            // Insira seu comentário
            SE num2 != 0 ENTAO

                // Insira seu comentário
                res = num1 / num2

                // Insira seu comentário
                ESCREVA num1, "/", num2, "=", res

            // Insira seu comentário
            SENAO
                ESCREVA "Impossível dividir!"

            FIM_SE

    // Insira seu comentário
    SENAO
        ESCREVA "Operação inválida!"

    FIM_ESCOLHA

FIM
```

#### Teste de mesa (0.5 ponto)

| num1 | num2 | op | num2 != 0 | res | saída               | 
| --   | --   | -- | --        | --  | --                  |
| 1    | 0    | 1  |           | 1   | 1 + 0 = 1           |
| 1    | 0    | 2  |           | 1   | 1 - 0 = 1           |
| 1    | 0    | 3  |           | 0   | 1 * 0 = 0           |
| 1    | 0    | 4  | False     |     | Impossível dividir! |
| 1    | 2    | 4  | True      | 0.5 | 1 / 2 = 0,5         |
| 1    | 2    | 5  |           |     | Operação inválida!  |
