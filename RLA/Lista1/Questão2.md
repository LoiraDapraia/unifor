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

    // Solicita que a pessoa digite seu salário atual
    ESCREVA "Digite seu salário atual:"

    // O algoritmo vai ler o salário
    LEIA sal_atual

    // Verifica se o salário é menor ou igual a 500
    SE sal_atual <= 500 ENTAO
        // Se o salário for menor ou igual a 500, aplica um ajuste de 20%
        sal_reaj = sal_atual * 1.2

    // Se o salário for maior que 500
    SENAO
        // Aplica um ajuste de 10%
        sal_reaj = sal_atual * 1.1

    FIM_SE

    // O algoritmo vai mostrar o novo salário
    ESCREVA "O novo salário é R$", sal_reaj

FIM
```

#### Tabela de testes 

| sal_atual | sal_atual >= 500 |sal_reaj       | saída                   | 
| --        | --               | --            | --                      | 
| 400       | False            | 400*1.2 = 480 | O novo salário é R$ 480 |
| 500       | True             | 500*1.2 = 600 | O novo salário é R$ 600 |
| 600       | True             | 600*1.1 = 660 | O novo salário é R$ 660 |
