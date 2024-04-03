#### Fluxograma

```mermaid
flowchart TD
A([INICIO]) --> B{{"Digite o número de termos da série S:"}}
B --> C[/n/]
C --> D[S = 0]
D --> E[[i=0 ATE n-1 PASSO 1]]
E --"i > n-1"--> J{{"Soma da série S é ", S}}
J --> K([FIM])
E --"i=0,1,2,..,n-1"--> F[numerador = 2 * i + 1]
F --> G[denominador = 2 * i + 2]
G --> H[termo = numerador / denominador]
H --> I[S += termo]
I --LOOP--> E
```

#### Pseudocódigo (1 ponto)

```java
Algoritmo SomaSerie
DECLARE n,numerador,denominador: INTEIRO; termo, S: REAL

INICIO

    // Solicita que o usuário digite o número de termos da série S
    ESCREVA "Digite o número de termos da série S:"

    // Armazena o valor inserido pelo usuário na variável "n"
    LEIA n

    // Inicializa a variável "S" com zero para armazenar a soma da série
    S <- 0

    // Loop contado (for) para iterar sobre os termos da série
    PARA i DE 0 ATÉ n-1 PASSO 1 FAÇA

        // Calcula o numerador do termo atual da série
        numerador = 2 * i + 1

        // Calcula o denominador do termo atual da série
        denominador <- 2 * i + 2

        // Calcula o termo atual da série dividindo o numerador pelo denominador
        termo = numerador / denominador

        // Adiciona o termo atual à soma da série
        S += termo

    FIM_PARA

    // Exibe a soma da série S
    ESCREVA "A soma da série S é ", S

FIM
```

#### Tabela de testes (0.25 ponto)

| it | n  | S  | i | numerador | denominador | termo | S += termo     | saída                  |
| -- | -- | -- |-- | --        | --          | --    | --             | --                     |
|    | 0  | 0  |   |           |             |       |                |                        |
| 1  | 4  | 0  | 0 | 2*0+1 = 1 | 2*0+2 = 2   | 1/2   | 0+1/2 = 1/2    |                        |
| 2  | 4  | 0  | 1 | 2*1+1 = 1 | 2*1+2 = 2   | 3/4   | 1/2+3/4 = 1.25 |                        |
| 3  | 4  | 0  | 2 | 2*2+1 = 1 | 2*2+2 = 2   | 5/6   | 0+1/2 = 2.08   |                        |
| 4  | 4  | 0  | 3 | 2*3+1 = 1 | 2*3+2 = 2   | 7/8   | 0+1/2 = 2.96   | Soma da série S é 2.96 |
