# UNIFOR
**Nome**: Juan Doth
**Disciplina**: Raciocínio logico algorítmico

##Questão 4
###Fluxograma
```mermaid
flowchart TD
A([Inicio]) --> B[/informar um número/]
B --> C{número >= 0}
C -- sim --> D{número % 2 == 0}
D -- sim --> E(O número é par)
D -- não --> F(O número é ímpar)
C -- não --> G[insira um número inteiro e positivo]
G --> Z([FIM])
E --> Z([FIM])
F --> Z([FIM])
```
