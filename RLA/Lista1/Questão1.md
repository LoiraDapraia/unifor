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

    // a pessoa inserir um numero
    ESCREVA "Digite um número: "
    
    // a maquina vai ler o numero
    LEIA numero
    
    // se o numero for mairo que 0 
    SE numero >= 0 ENTAO

        // Insira seu comentário
        resto <- numero % 2

        // se o resto for igual a 0 a maquina escrevera o numero é par
        SE resto == 0 ENTAO
            ESCREVA "O número é par!"

        // senao ira escrever que é impar
        SENAO
          ESCREVA "O número é impar!"

        FIM_SE

    // se o numero não for positivo ira voltar para o escreva o numero
    SENAO             
        ESCREVA "O número deve ser postivo!"

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
