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
###Pseudocódigo
```
1 ALGORITMO Verificar_media_Aritmética
2   DECLARE Nota 1 e Nota 2
3  ESCREVA informe a Nota 1 e Nota 2
4 LEIA Nota 1 e Nota 2
5   DECLARE Nota Final 
6    SE Nota Final > 5 ENTAO
7     ESCREVA "APROVADO"
8   SENAO
9    ESCREVA "REPROVADO"
10 FIM_ALGORITMO
```
