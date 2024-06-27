# Información de apunte

Este es un documento complementario de ***[El lenguaje lógico](El%20lenguaje%20lógico.md)***.

## Tablas de verdad

Una **tabla de verdad**, o **tabla de valores de verdades**, es una tabla que muestra el [valor de verdad](https://es.wikipedia.org/wiki/Valor_de_verdad "Valor de verdad") de una [proposición](https://es.wikipedia.org/wiki/Proposici%C3%B3n "Proposición") compuesta, para cada combinación de verdad que se pueda asignar. [Fuente original](https://es.wikipedia.org/wiki/Tabla_de_verdad)
​
### Estructura Base

En esta estructura base, tenemos dos proposiciones (***A*** y ***B***). Pueden ser *proposiciones complejas*, pero para simplificar, también podríamos considerarlas como *proposiciones simples* (***p*** y ***q***) (*Es valido para ambos casos*). Los resultados de la tabla de verdad (***X***) depende del *conector lógico* (***C***) que se utilice para combinar (***A*** y ***B***).

| A   | B   | A {C} B |
| --- | --- | :-----: |
| V   | V   |   {X}   |
| V   | F   |   {X}   |
| F   | V   |   {X}   |
| F   | F   |   {X}   |

**No olvidar lo fundamental para todas las tablas!**
- Patrón de la primera **columna** (***A***): **[VVFF]**
- Patrón de la segunda **columna** (***B***): **[VFVF]**
- El número de **filas** en una tabla de verdad para una proposición molecular se calcula como ***2^n***, donde ***n*** es el número de proposiciones atómicas.
### Tablas de verdad *(Según conectores lógicos)*

A continuación todas las tablas de verdad según sus respectivos conectores lógicos.
El formato será: {Conector Lógico} seguido de sus notaciones populares -> (N1), (N2), ("N3" o "N4"), (N...): [Tabla de verdad]

**Conjunción: ("Y" o "AND"),  ("&" o "&&"), ( . ), (∧)**:

(***A*** ∧ ***B***) es verdadera solo si tanto ***A*** como ***B*** son verdaderas.

| A   | B   | A ∧ B |
| --- | --- | :---: |
| V   | V   |   V   |
| V   | F   |   F   |
| F   | V   |   F   |
| F   | F   |   F   |

**Disyunción ("O" u "OR"), (" | " o "||"), (+), (∨)**:

(***A*** ∨ ***B***) es verdadera si al menos una de las proposiciones ***A*** o ***B*** es verdadera.

| A   | B   | A ∨ B |
| --- | --- | :---: |
| V   | V   |   V   |
| V   | F   |   V   |
| F   | V   |   V   |
| F   | F   |   F   |

**Condicional, Implicación o 'Si...entonces' ("→" o "=>")**:

(***A*** → ***B***) es falsa solo si ***A*** es verdadera y ***B*** es falsa; en cualquier otro caso es verdadera.

| A   | B   | A → B |
| --- | --- | :---: |
| V   | V   |   V   |
| V   | F   |   F   |
| F   | V   |   V   |
| F   | F   |   V   |

**Bicondicional o 'si y solo si' ("<=>" o "↔")**:

(***A*** ↔ ***B***) es verdadera si ***A*** y ***B*** tienen el mismo valor de verdad.

| A   | B   | A ↔ B |
| --- | --- | :---: |
| V   | V   |   V   |
| V   | F   |   F   |
| F   | V   |   F   |
| F   | F   |   V   |

**Nota**: Este conector lógico no tiene una representación reservada en los lenguajes de programación, ya que su lógica es tan simple como hacer: `A == B` o `p == q`

**Negación o Complemento Lógico (NOT), ("~" o "-"), ( ! ), ( ¬ )**:

Este operador invierte el valor de verdad de una proposición. Si la proposición es verdadera, su negación es falsa y viceversa.

| A   | ¬A  |
| --- | --- |
| V   | F   |
| F   | V   |

### Estructura Base con Negación implementada

Para incluir la negación en nuestra tabla de verdad, agregamos una columna para ¬***A*** y otra para ¬***B***, no hace falta modificar los resultados de la tabla si implementamos estas columnas con sus debidos patrones pero invertidos.

| A   | B   | ¬A  | ¬B  | A {C} B |
| --- | --- | --- | --- | :-----: |
| V   | V   | F   | F   |   {X}   |
| V   | F   | F   | V   |   {X}   |
| F   | V   | V   | F   |   {X}   |
| F   | F   | V   | V   |   {X}   |

Patrones normales como vimos previamente:
- Patrón de la primera **columna** (***A***): **[VVFF]**
- Patrón de la segunda **columna** (***B***): **[VFVF]**

Patrones invertidos para Negación:
- Patrón de la tercera **columna** (¬***A***): **[FFVV]**
- Patrón de la cuarta **columna** (¬***B***): **[FVFV]**

### Conectores Lógicos con Negación

**Conjunción (AND, ∧) con Negación**:

| A   | B   | ¬A  | ¬B  | A ∧ B |
| --- | --- | --- | --- | :---: |
| V   | V   | F   | F   |   V   |
| V   | F   | F   | V   |   F   |
| F   | V   | V   | F   |   F   |
| F   | F   | V   | V   |   F   |

**Disyunción (OR, ∨) con Negación**:

| A   | B   | ¬A  | ¬B  | A ∨ B |
| --- | --- | --- | --- | :---: |
| V   | V   | F   | F   |   V   |
| V   | F   | F   | V   |   V   |
| F   | V   | V   | F   |   V   |
| F   | F   | V   | V   |   F   |

**Implicación (→) con Negación**:

| A   | B   | ¬A  | ¬B  | A → B |
| --- | --- | --- | --- | :---: |
| V   | V   | F   | F   |   V   |
| V   | F   | F   | V   |   F   |
| F   | V   | V   | F   |   V   |
| F   | F   | V   | V   |   V   |

**Bicondicional (↔) con Negación**:

| A   | B   | ¬A  | ¬B  | A ↔ B |
| --- | --- | --- | --- | :---: |
| V   | V   | F   | F   |   V   |
| V   | F   | F   | V   |   F   |
| F   | V   | V   | F   |   F   |
| F   | F   | V   | V   |   V   |

### Recursos utiles

Ver tablas de verdad en: [***Curso de Logica Proposicional*** ](https://www.youtube.com/playlist?list=PLeySRPnY35dHBYcVHPisjBCVHBa954rMZ)

[BBeej/Code4Exactas-UBA](https://github.com/BBeej/Code4Exactas-UBA)
