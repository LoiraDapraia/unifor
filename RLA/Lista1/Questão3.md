# UNIFOR
**Nome**: Juan Doth
**Disciplina**: Raciocínio logico algorítmico

##Questão 2
###Fluxograma
```mermaid
flowchart TD
A([Inicio]) --> B[/informe Nota 1 e Nota 2/]
B --> G[Calcular nota]
G --> C[Nota 1 + Nota 2/2]
C --> H[Nota Final]
H --> D{Nota Final > 5}
D --Não --> E[REPROVADO]
D --Sim --> F[APROVADO]
E --> Z([FIM])
F --> Z
```
