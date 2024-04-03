# UNIFOR
**Nome**: Juan Doth
**Disciplina**: Raciocínio logico algorítmico

##Questão 2
###Fluxograma
```mermaid
flowchart TD
A([Inicio]) --> B[/informe Nota 1 e Nota 2/]
B --> G[Calcular nota]
G --> C[Nota 1 + Nota 2 /2]
C --> H[Nota Final]
H --> D{Nota Final > 5}
D --Não --> E[REPROVADO]
D --Sim --> F[APROVADO]
E --> Z([FIM])
F --> Z
```
#### Pseudocódigo (1 ponto)

```java
ALGORTIMO SituacaoAluno
DECLARE nota1, nota2, media: REAL

INICIO

    // Insira seu comentário
    ESCREVA "Digite a nota 1:"

    // Insira seu comentário
    LEIA nota1

    // Insira seu comentário
    ESCREVA "Digite a nota 2:"

    // Insira seu comentário
    LEIA nota2

    // Insira seu comentário
    SE nota1 >= 0 E nota2 >= 0 ENTAO

        // Insira seu comentário
        media =  (nota1 + nota2)/2

        // Insira seu comentário
        SE media >= 7 ENTAO
            ESCREVA "O aluno está aprovado!"

        // Insira seu comentário
        SENAO
            "O aluno está reprovado!"

        FIM_SE

    // Insira seu comentário
    SENAO
        ESCREVA "A nota deve ser maior que zero!"

    FIM_SE

FIM
```

#### Tabela de testes (1 ponto)

| nota1 | nota2 | nota1 >= 0 E nota2 >= 0 | media        | saĩda | 
| --    | --    | --                      | --           | --    | 
| -1    | 0     | False                   |              | A nota deve ser maior que zero! | 
| 0     | 0     | True                    | (0+0)/2 = 0  | O aluno está reprovado!|
| 4     | 8     | True                    | (4+8)/2 = 6  | O aluno está reprovado!|
| 4     | 10    | True                    | (4+10)/2 = 7 | O aluno está aprovado!|
