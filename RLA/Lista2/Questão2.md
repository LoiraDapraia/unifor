# UNIFOR
**Nome**: Juan Doth
**Disciplina**: Raciocínio logico algorítmico

##Questão 2
###Fluxograma
```mermaid
flowchart TD
A([Inicio]) --> B[/digite uma temperatura em Celsius/]
B --> C[Transforme esse valor para fahrenheit]
C --> D(aplique o valor na formula)
D --> E[F = 9/5 * C + 32]
E --> F(Valor em fahrenheit )
F --> G([FIM])
```
#### Pseudocódigo (1.0 ponto)

```java
ALGORTIMO ConverteCelsiusFarenheit
DECLARE C, F: REAL

INICIO

    // Solicita que o usuário insira a temperatura em Celsius
    ESCREVA "Digite a temperatura em Celsius:"

    // Lê a temperatura em Celsius inserida pelo usuário
    LEIA C

    // Converte a temperatura de Celsius para Fahrenheit
    F <- (9/5) * C + 32

    // Mostra a temperatura convertida em Fahrenheit
    ESCREVA "A temperatura em Fahrenheit é", F, "graus"

FIM
```

#### Teste de mesa (0.5 ponto)

| C  | F  | saída                                  | 
| -- | -- | --                                     |
| 0  | 32 | A temperatura em Fahrenheit é 32 graus |
