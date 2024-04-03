# UNIFOR
**Nome**: Juan Doth
**Disciplina**: Raciocínio logico algorítmico

##Questão 2
###Fluxograma
```mermaid
flowchart TD
A([Inicio]) --> B[/informe idade/]
B --> C[Avaliar A Idade]
C --> D{Idade > 18}
D --NÃO -->E[NÃO APTO]
E --> F[Calcular anos necessários para tornar-se apto a obter a CNH]
D --SIM --> G[APTO]
G --> Z([FIM])
F --> Z
```
#### Pseudocódigo 

```java
ALGORTIMO AptoCNH
DECLARE idade, anos_apto: INTEIRO

```plaintext
INICIO

    // Solicita que o usuário insira sua idade
    ESCREVA "Digite a sua idade:"

    // Lê a idade inserida pelo usuário
    LEIA idade

    // Verifica se a idade é menor que zero
    SE idade < 0 ENTAO
        // Informa que a idade deve ser maior que zero
        ESCREVA "A idade deve ser maior que zero!"

    // Se a idade não for menor que zero
    SENAO

        // Verifica se a idade é maior ou igual a 18
        SE idade >= 18 ENTAO
            // Informa que o candidato está apto a tirar a CNH
            ESCREVA "O candidato está apto a tirar a CNH!"

        // Caso contrário
        SENAO

            // Calcula quantos anos faltam para o candidato estar apto
            anos_apto <- 18 - idade

            // Informa quantos anos faltam para o candidato estar apto
            ESCREVA "Faltam", anos_apto, "ano(s) para o candidato estar apto!"

        FIM_SE

    FIM_SE

FIM
```

Comentários adicionados para explicar cada parte do pseudocódigo.
```

#### Tabela de testes 

| idade | idade < 0 | idade >= 18 | anos_apto | saída                                         | 
| --    | --        | --          | --        | --                                            | 
| -1    | True      |             |           |                                               |
| 0     | False     | False       | 18-0 = 18 | Faltam 18 ano(s) para o candidato estar apto! |
| 17    | False     | False       | 18-17 = 1 | Faltam 1 ano(s) para o candidato estar apto!  |
| 18    | False     | True        |           | O candidato está apto a tirar a CNH!          |
