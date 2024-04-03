# UNIFOR
**Nome**: Juan Doth
**Disciplina**: Raciocínio logico algorítmico

##Questão 4
###Fluxograma
```mermaid
flowchart TD
A([Inicio]) --> B[/informar idade/]
B --> C{idade >= 5 e idade <= 7}
C -- sim --> D(Infantil A)
D --> Z([FIM])
C -- não --> E{ idade >= 11 e idade <= 13}
E -- sim --> F(Juvenil A)
F --> Z
E -- não --> G{idade >= 14 e idade <= 17}
G -- sim --> H(Juvenil B)
H --> Z
G -- não --> I{idade > 18}
I -- sim --> J(Adulto)
J --> Z
I -- não --> K(não tem categoria)
K --> Z
```
#### Pseudocódigo (1.0 ponto)

```
ALGORTIMO ClassificaCategoria
DECLARE idade: INTEIRO

INICIO

    // Insira seu comentário
    ESCREVA "Digite a idade do aluno:"

    // Insira seu comentário
    LEIA idade

    // Insira seu comentário
    ESCOLHA

        // Insira seu comentário
        CASO idade >=5 E idade <= 7

            // Insira seu comentário
            ESCREVA "Infantial A"

        // Insira seu comentário
        CASO idade >=8 E idade <= 10

            // Insira seu comentário
            ESCREVA "Infantial B"

        // Insira seu comentário
        CASO idade >=11 E idade <= 13

            // Insira seu comentário
            ESCREVA "Juvenil A"

        // Insira seu comentário
        CASO idade >=14 E idade <= 17

            // Insira seu comentário
            ESCREVA "Juvenil B"

        // Insira seu comentário
        CASO idade >=18

            // Insira seu comentário
            ESCREVA "Adulto"

    // Insira seu comentário
    SENAO

        // Insira seu comentário
        ESCREVA "Digite uma idade válida!"

    FIM_ESCOLHA

FIM
```

#### Teste de mesa (0.5 ponto)

| idade | idade >=8 E idade <= 10 | idade >=11 E idade <= 13 | idade >=14 E idade <= 17 | idade >=18 | saída                       | 
| --    | --                      | --                       | --                       | --         | --                          |
| 4     | False                   | False                    | False                    | False      | Digite uma idade válida!    |
| -4    | False                   | False                    | False                    | False      | Digite uma idade válida!    |
| 8     | True                    | False                    | False                    | False      | Infantial A                 |
| 11    | False                   | True                     | False                    | False      | Infantial B                 |
| 17    | False                   | False                    | True                     | False      | Infantial C                 |
| 21    | False                   | False                    | False                    | True       | Adulto                      |
