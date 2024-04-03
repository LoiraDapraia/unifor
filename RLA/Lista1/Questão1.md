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
###Pseudocódigo
```
1 ALGORITIMO verifica_par_impar
2 DECLARE numero, resto NUMERICO
3 ESCREVA "Digite um número"
4 LEIA numero
5 SE numero > 0 ENTAO
6   resto = numero % 2
7   SE resto == 0 ENTAO
8     ESCREVA "O número é par!"
9   SENAO
10    ESCREVA "O número é impar!"
11 SENAO
12   ESCREVA " O número é positivo
13 FIM_ALGORITIMO


#### Tabela de testes (0,25 ponto)
| numero | numero >= 0 | resto | resto == 0 | Saída |
| -- | -- | -- | -- | -- | 
| -1 | F |   |   | "O número deve ser postivo!" |
| 0  | V | 0 | V | "O número é par!" |
| 13 | V | 1 | F | "O número é impar!" |
| 30 | V | 0 | V | "O número é par!" |
