# UNIFOR
**Nome**: Juan Doth
**Disciplina**: Raciocínio logico algorítmico

##Questão 2
###Fluxograma
```mermaid
flowchart TD
A([Inicio]) --> B[/contar i como 0/]
B --> C{i <= 30}
C -- sim --> D{i % 3 == 0}
D -- sim --> F(mostrar i)
C -- não -->G([FIM])
D -- não --> H(Adicionar o contador i em 1)
F --> G
H --> G
```
#### Pseudocódigo (1.0 ponto)

```java
ALGORTIMO MultiploTres
DECLARE n: INTEIRO

INICIO

    // Solicita que o usuário digite a quantidade de números
    ESCREVA "Digite a quantidade de números:"

    // Armazena o valor inserido pelo usuário na variável "n"
    LEIA n

    // Loop contado (for) que itera sobre os valores de 'i' de 0 até n-1, incrementando 'i' em 3 a cada iteração
    PARA i DE 0 ATÉ n-1 PASSO 3 FAÇA

        // Exibe o valor de 'i' em cada iteração
        ESCREVA i

    FIM_PARA

FIM
```

#### Tabela de testes (0.5 ponto)

| it | n   | i  | saida | 
| -- | --  | -- | --    |    
| 1  | 7   | 0  | 0     |
| 2  | 7   | 3  | 3     |
| 3  | 7   | 6  | 6     |

