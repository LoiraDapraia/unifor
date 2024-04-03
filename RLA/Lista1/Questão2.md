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
#### Pseudocódigo

```java
ALGORTIMO ReajusteSalario
DECLARE sal_atual, sal_reaj: REAL

INICIO

    // a pessoa deve digitar o seu salario atual
    ESCREVA "Digite seu salário atual:"

    // O algoritmo vai ler o seu salario
    LEIA sal_atual

    // Se o salario for menor ou igual a 500 a pessoa recebera um ajuste de 1.2
    SE sal_atual <= 500 ENTAO
        sal_reaj = sal_atual * 1.2

    // SENAO for maior ou igual a 500 receberar um ajuste de 1.1
    SENAO
        sal_reaj = sal_atual * 1.1

    FIM_SE

    // O algoritimo vai mostrar o novo salario
    ESCREVA "O novo salário é R$", sal_reaj

FIM
```

#### Tabela de testes 

| sal_atual | sal_atual >= 500 |sal_reaj       | saída                   | 
| --        | --               | --            | --                      | 
| 400       | False            | 400*1.2 = 480 | O novo salário é R$ 480 |
| 500       | True             | 500*1.2 = 600 | O novo salário é R$ 600 |
| 600       | True             | 600*1.1 = 660 | O novo salário é R$ 660 |
