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
#### Pseudocódigo (1.0 ponto)

```java
ALGORTIMO verifica_par_impar
DECLARE num, resto: INTEIRO

INICIO

	// Entrada do usuário de um número inteiro qualquer armezando na variável "num"
	ESCREVA "Digite um número: "

	// Armazena o valor de entrada na variável "num"
	LEIA num

	// Loop condicional (loop while) executa as instruções enquanto a condição "num < 0" for verdadeira
	ENQUANTO num < 0 FAÇA

		// Exibe a mensagem com a solicitação de um número ao usuário
		ESCREVA "Digite um número maior ou igual a zero:"

		// Um novo número é atribuido na variável "num"
		LEIA num

	FIM_ENQUANTO

	// Executa as instruções sob a condição "num >= 0" for verdadeira
	SE num >= 0 ENTAO

		// Calcula o resto da divisão de "num" por 2
		resto ← num % 2
               
		// Executa a instrução se o resto é igual a zero
		SE resto == 0 ENTAO
			ESCREVA "O número é par!"

		// Executa a instrução se o resto não for igual a zero
		SENAO
			ESCREVA "O número é impar!"

		FIM_SE

	// Executa a instrução se inteiro for negativo
	SENAO                               
		ESCREVA "O número deve ser postivo!"

	FIM_SE

FIM
```

#### Tabela de testes (0.5 ponto)

| num | num < 0 | num | resto | resto == 0 | saída             | 
| --  | --      | --  | --    | --         | --                | 
| -1  | True    | 0   | 0     | True       | O número é par!   |
| 1   | False   |     | 1     | False      | O número é impar! |
| 2   | False   |     | 0     | True       | O número é par!   |
