#### Fluxograma

```mermaid
flowchart TD
A([INICIO]) --> B{{"Digite um numero inteiro nao-negativo:"}}
B --> C[/n/]
C --> D{n >= 0}
D --TRUE--> E[fator = 1]
D --FALSE--> J{{"O valor deve ser maior ou igual a zero!"}}
J --> I([FIM])
E --> F[[i=1 ATÉ n PASSO 1]]
F --"i > n"--> H{{O fatorial de, n, é:, fator}}
F --"i=1,2,..n"--> G[fator = fator * i]
G --LOOP--> F
H --> I
```

#### Pseudocódigo (2 pontos)

```java
ALGORITMO CalcFatorial
DECLARE n: INTEIRO

INICIO

    // Solicita que o usuário digite um número inteiro não negativo
    ESCREVA "Digite um número inteiro não negativo:"

    // Armazena o valor inserido pelo usuário na variável "n"
    LEIA n

    // Verifica se o valor inserido pelo usuário é maior ou igual a zero
    SE n >= 0 ENTAO

        // Inicializa a variável "fator" como 1 para calcular o fatorial
        fator <- 1

        // Loop contado (for) para calcular o fatorial de "n"
        PARA i DE 1 ATÉ n PASSO 1 FAÇA

            // Calcula o fatorial multiplicando o fator pelo valor atual de "i"
            fator <- fator * i

        FIM_PARA

        // Exibe o fatorial de "n"
        ESCREVA "O fatorial de ", n, " é:", fator

    // Se o valor inserido pelo usuário não for maior ou igual a zero
    SENAO
        // Informa que o valor deve ser maior ou igual a zero
        ESCREVA "O valor deve ser maior ou igual a zero!"

    FIM_SE

FIM
```

#### Tabela de testes

| n  | fator | i  | fator = fator * i | saída               |
| -- | --    | -- | --                | --                  |
| 3  | 1     | 1  | 1*1 = 1           |                     |
| 3  | 1     | 2  | 1*2 = 2           |                     |
| 3  | 2     | 3  | 2*3 = 6           | O fatorial de 3 é 6 |
