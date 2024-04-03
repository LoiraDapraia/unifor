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
ALGORTIMO ReajusteSalario
DECLARE sal_atual, sal_reaj: REAL

INICIO

    // para a pessoa escrever seu salario atual
    ESCREVA "Digite seu salário atual:"

    // o algoritimo vai ler o seu salario
    LEIA sal_atual

    // se for maior que 500 vai ter reajuste
    SE sal_atual <= 500 ENTAO
        sal_reaj = sal_atual * 1.2

    // se não vara o reajuste com outro valor
    SENAO
        sal_reaj = sal_atual * 1.1

    FIM_SE

    // apresentar o novo salario
    ESCREVA "O novo salário é R$", sal_reaj

FIM
```
