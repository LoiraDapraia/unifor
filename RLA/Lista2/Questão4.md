# UNIFOR
**Nome**: Juan Doth
**Disciplina**: Raciocínio logico algorítmico

##Questão 4
###Fluxograma
```mermaid
flowchart TD
A([Inicio]) --> B[/informar idade/]
B --> C{idade >= 5 e idade <= 7}
C -- sim --> D(Infantil A)
D --> Z([FIM])
C -- não --> E{ idade >= 11 e idade <= 13}
E -- sim --> F(Juvenil A)
F --> Z
E -- não --> G{idade >= 14 e idade <= 17}
G -- sim --> H(Juvenil B)
H --> Z
G -- não --> I{idade > 18}
I -- sim --> J(Adulto)
J --> Z
I -- não --> K(não tem categoria)
K --> Z
