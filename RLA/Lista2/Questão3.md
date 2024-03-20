# UNIFOR
**Nome**: Juan Doth
**Disciplina**: Raciocínio logico algorítmico

##Questão 3
###Fluxograma
```mermaid
flowchart TD
A([Inicio]) --> B[/digite um número 1/]
B --> C[/Digite um operador, +, -, *, / /]
C -->D[/Digite um número 2/]
D -->E{Se for = +}
E -- sim -->F[N1+N2]
E -- não --> H{Se for = -}
F --> G(resultado)
G --> Z([FIM])
H -- sim --> I[N1 - N2]
I --> J(Resultado)
J --> Z
H -- não --> K{Se for = *}
K -- sim --> L[N1 * N2]
L --> M(Resultado)
M --> Z
K -- não --> N{Se for = /}
N --> O(N2 for = 0)
O -- sim -->P[não pode ser dividido]
O -- não --> Q[N1/N2]
Q --> R(Resultado)
R --> Z
```
