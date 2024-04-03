# UNIFOR
**Nome**: Juan Doth
**Disciplina**: Raciocínio logico algorítmico

##EXERCÍCIO 3
###Fluxograma
```mermaid
flowchart TD
A([INICIO]) --> B{{digite um número:}}
B --> C[/Número/]
C --> D{Número > 0}
D --NÃO--> E[O número não é positivo!]
D --SIM--> F[R= Número % 2]
E --> Z([FIM])
F --> G{R == 0}
G --Não --> H{{O número é impar!}}
G --SIM--> I{{ O Número é par}}
H --> Z
I --> Z
```
#### Pseudocódigo
```java
ALGORTIMO verifica_par_impar
DECLARE numero, resto: INTEIRO

INICIO

    // Solicita que o usuário insira um número
    ESCREVA "Digite um número: "
    
    // Lê o número inserido pelo usuário
    LEIA numero
    
    // Verifica se o número é maior ou igual a zero
    SE numero >= 0 ENTAO

        // Calcula o resto da divisão do número por 2
        resto <- numero % 2

        // Verifica se o resto da divisão é igual a zero (ou seja, se o número é par)
        SE resto == 0 ENTAO
            // Se o número é par, exibe essa informação
            ESCREVA "O número é par!"

        // Se o resto da divisão não é zero, o número é ímpar
        SENAO
            // Exibe essa informação
            ESCREVA "O número é ímpar!"

        FIM_SE

    // Se o número não for positivo (menor que zero), exibe uma mensagem de erro
    SENAO             
        ESCREVA "O número deve ser positivo!"

    FIM_SE

FIM
```


#### Tabela de testes
| numero | numero >= 0 | resto | resto == 0 | Saída |
| -- | -- | -- | -- | -- | 
| -1 | F |   |   | "O número deve ser postivo!" |
| 0  | V | 0 | V | "O número é par!" |
| 13 | V | 1 | F | "O número é impar!" |
| 30 | V | 0 | V | "O número é par!" |
