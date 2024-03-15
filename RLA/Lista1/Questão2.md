# UNIFOR
**Nome**: Juan Doth
**Disciplina**: Raciocínio logico algorítmico

##Questão 2
###Fluxograma
```mermaid
flowchart TD
A([Inicio]) --> C[/Informe o seu salario/]
C --> R[Salario]
R --> B{Salario = R$500}
B --Não --> E[Aumento de 10%]
B --Sim --> F[Aumento de 20%]
E --> G{{Calcular o novo salario}}
G --> Y[Novo Salario]
F --> G
Y --> Z([FIM])
```
###Pseudocódigo
```
1 ALGORITMO Informe_O_Salario 
2 DECLARE salario
3 ESCREVA informe o salario
4 LEIA salario 
5    SE salario for = R$ 500 ENTAO
6     ESCREVA Aumento de 20%
7   SENAO 
8     ESCREVA aumento de 10% ENTAO
7    ESCREVA calcular o novo salario ENTAO
8   ESCREVA novo salario 
9 FIM_ALGORITMO
```
