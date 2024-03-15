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
