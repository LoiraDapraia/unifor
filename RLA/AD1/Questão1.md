#### Fluxograma

```mermaid
flowchart TD
A([INICIO]) --> B{{"Digite o valor da a:"}}
B --> C[\a\]
C --> D{{"Digite o valor da b:"}}
D --> E[\b\]
E --> F[aux = a]
F --> G[a = b]
G --> H[b = aux]
H --> I{{"a =", a}}
I --> J{{"b =", b}}
```

#### Pseudocódigo (1 ponto)

```java
ALGORTIMO TrocaValores
DECLARE a,b,axu: REAL

INICIO

    // Solicita que o usuário insira o valor de a
    ESCREVA "Digite o valor da a:"

    // Armazena o valor inserido pelo usuário na variável "a"
    LEIA a

    // Solicita que o usuário insira o valor de b
    ESCREVA "Digite o valor da b:"

    // Armazena o valor inserido pelo usuário na variável "b"
    LEIA b

    // Troca os valores de a e b usando uma variável auxiliar
    aux <- a 
    a <- b
    b <- aux

    // Exibe os novos valores de a e b após a troca
    ESCREVA "a=", a
    ESCREVA "b=", b

FIM
```

#### Tabela de testes

| a  | b  | aux | a  | b  | saída 1 | saída 2 | 
| -- | -- | --  | -- | -- | --      | --      | 
| 0  | 1  | 0   | 1  | 0  | a = 1   | b = 0   |

