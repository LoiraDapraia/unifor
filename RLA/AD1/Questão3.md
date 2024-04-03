#### Fluxograma

```mermaid
flowchart TD
A([INICIO]) --> B{{"Digite a quantidade de números<br> (n >= 0):"}}
B --> C[\n\]
C --> D{n >= 0}
D --FALSE-->N{{"O valor deve ser maior ou igual a zero!"}}
N --> M([FIM])
D --TRUE--> E[/soma = 0/]
E --> F[i = 1]
F --> G{i <= n}
G --FALSE--> L{{"A soma dos numeros é , soma"}}
L --> M
G --TRUE--> H{{Digite um número: }}
H --> I[\num\]
I --> J[soma =+ num]
J --> K[i =+ 1]
K --LOOP--> G
```

#### Pseudocódigo (1 ponto)

```java
Algoritmo SomaNumeros
DECLARE n,i,soma: INTEIRO

INICIO

    // Solicita que o usuário insira a quantidade de números (n >= 0)
    ESCREVA "Digite a quantidade de números (n >= 0):"
    LEIA n

    // Verifica se o valor inserido pelo usuário é maior ou igual a zero
    SE n >= 0 ENTAO

        // Inicializa a variável "soma" com zero
        soma <- 0

        // Inicializa a variável "i" com algum valor inicial (possivelmente deveria ser 1)
        i <- i

        // Loop condicional (while) que executa enquanto "i" for menor ou igual a "n"
        ENQUANTO i <= n FAÇA

            // Solicita que o usuário insira um número
            ESCREVA "Digite um número:"

            // Armazena o número inserido pelo usuário na variável "num"
            LEIA num 

            // Adiciona o número à variável "soma"
            soma <- soma + num

            // Incrementa o contador "i" para avançar para a próxima iteração
            i <- i + 1

        FIM_ENQUANTO

    // Se o valor inserido pelo usuário não for maior ou igual a zero
    SENAO
        // Informa que o valor deve ser maior ou igual a zero
        ESCREVA "O valor deve ser maior ou igual a zero!"

    FIM_SE

    // Exibe a soma dos números inseridos pelo usuário
    ESCREVA "A soma dos números é ", soma

FIM
```

#### Tabela de testes

| it | n  | n >= 0 | soma | i  | i <= n | num | soma =+ num  | saída                   |
| -- | -- | --     | --   | -- | --     | --  | --           | --                      |
|    | -3 | False  |      |    |        |     |              | O valor deve ser ...    |
| 1  | 0  | True   | 0    | 1  | False  |     |              | A soma dos números é 0  |
| 1  | 3  | True   | 0    | 1  | True   | 5   | 0 + 5 = 5    |                         |
| 2  | 3  | True   | 5    | 2  | True   | 10  | 5 + 10 = 15  |                         |
| 3  | 3  | True   | 15   | 3  | True   | 20  | 15 + 20 = 35 |                         |
| 4  | 3  | True   | 35   | 4  | False  |     |              | A soma dos números é 35 |
