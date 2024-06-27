# Información de apunte

Este documento explora el capítulo 1.1 de "Nociones Básicas de Lógica", donde se introducen los fundamentos esenciales, como la Lógica Proposicional. El objetivo es proporcionar una base clara para evaluar y construir proposiciones de manera correcta y efectiva. Estos conceptos son cruciales no solo en el estudio de la lógica, sino también en su aplicación práctica en disciplinas como la informática/computación y las ciencias naturales/exactas.

Este apunte es la continuación de ***[Introducción a la Filosofía Básica](Introducción%20a%20la%20Filosofía%20Básica.md)***

## 1.1 El lenguaje lógico

### Introducción a la Lógica

La lógica es la disciplina que estudia los métodos y principios para distinguir entre razonamientos correctos e incorrectos. Sus objetivos principales son establecer las leyes del pensamiento válido y proporcionar métodos para evaluar argumentos.

**Tipos de lógica:**
- Lógica formal: Se enfoca en la estructura de los argumentos.
- Lógica informal: Se centra en el contenido y contexto de los argumentos.

**Componentes básicos:**
1. **Proposiciones**: Enunciados que pueden ser verdaderos o falsos.
2. **Argumentos**: Conjuntos de proposiciones donde una (conclusión) se infiere de las otras ([premisas](#Premisa)).

### Aplicaciones de la Lógica

La lógica se aplica en diversas ramas:
- **Filosofía**: Análisis de argumentos y clarificación de conceptos.
- **Matemáticas**: Base para demostraciones y teoremas.
- **Ciencias naturales**: Formulación y evaluación de hipótesis.
- ***Ciencias de la Computación***: Fundamental en programación, diseño de algoritmos, inteligencia artificial, sistemas, etc. 

### Conceptos Fundamentales

#### Proposiciones
**Definición**: Enunciados declarativos que pueden ser verdaderos o falsos.

**Tipos**:
- **Atómicas**: Proposiciones simples. Ejemplo: "Está lloviendo" ***(p)***
- **Moleculares**: Combinación de proposiciones atómicas mediante conectivas lógicas. Ejemplo: "Está lloviendo y hace frío" ***(p . q)***

**Nota**: El número de filas en una tabla de verdad para una proposición molecular se calcula como ***2^n***, donde ***n*** es el número de proposiciones atómicas.

#### Términos
Palabras o conjuntos de palabras que nombran aspectos de la realidad.

**Tipos**:
- **Descriptivos**: Mencionan aspectos de la realidad. Ejemplo: "agua", "temperatura"
- **Lógicos**: Enlazan términos o proposiciones. Ejemplo: "y", "o", "si...entonces"

### Variables lógicas
- ***p, q, r...***: Generalmente representan proposiciones atómicas.
- ***A, B, C...***: Representan fórmulas que pueden ser simples o complejas.

### Conectivas Lógicas

**Nota**: Los símbolos pueden variar según el autor o contexto, pero mantendremos el estándar utilizado en ***IPC (40) Cátedra Perot***.

1. **Conjunción (.)**: "Y"
   Ejemplo: *"Llueve y hace frío"* ***(p . q)***

2. **Disyunción (∨)**: "O"
   Ejemplo: *"Es día o es noche"* ***(p ∨ q)***

3. **Condicional (=>)**: "Si...entonces"
   Ejemplo: *"Si llueve, entonces la calle está mojada"* ***(p => q)***

4. **Negación (-)**: "NO"
   Ejemplo: *"No llueve"* ***(-p)***

5. **Bicondicional (<=>)**: "si y solo si"
   Ejemplo: *"La figura es un cuadrado si y solo si tiene cuatro lados iguales y cuatro ángulos rectos"* ***(p <=> q)***

### Tablas de verdad

Son herramientas que muestran todas las posibles combinaciones de valores de verdad para las proposiciones atómicas y cómo afectan a la proposición molecular. Ayudan a determinar bajo qué condiciones una proposición compleja es verdadera o falsa.
***[(Ver tablas de verdad)](Tablas%20de%20verdad.md)***

### Fórmulas bien formadas

Reglas para construir expresiones válidas en el lenguaje lógico:
1. Toda proposición atómica ***(p, q, r...)*** es una fórmula bien formada.
2. Si ***A*** y ***B*** son fórmulas, entonces ***A ∨ B, A . B, A => B, -A, y A <=> B*** también lo son.

Ejemplo simple: 
- ***p*** es una fórmula bien formada
- Si ***p*** y ***q*** son fórmulas, entonces ***(p . q)*** también lo es

### Importancia en la Ciencia

La lógica es crucial en el método científico y particularmente en ***Ciencias de la Computación***:
- Proporciona la base para el razonamiento formal en programación.
- Es esencial en el diseño y análisis de algoritmos.
- Fundamental en la verificación y validación de sistemas de software.
- Base para lenguajes de programación lógica.
- Crucial en el desarrollo de sistemas como inteligencia artificial y aprendizaje automático.
(Estos son algunos de la infinidad de ejemplos que existen...)

### Recursos utiles

Si los conceptos mencionados no quedaron claros, recomiendo ver el siguiente [***Curso de Logica Proposicional*** ](https://www.youtube.com/playlist?list=PLeySRPnY35dHBYcVHPisjBCVHBa954rMZ)

### Definiciones

#### Inferencia
Acto o proceso de derivar conclusiones lógicas a partir de [premisas](#Premisa.) que se conoce o asumen como ciertas. ([mas info](https://concepto.de/inferencia/))

#### Premisa
**[Proposiciones](https://concepto.de/proposicion/) iniciales de un [argumento](https://concepto.de/argumento/)**, a partir de las cuales es posible llegar a una conclusión. ([mas info](https://concepto.de/premisa/))

(Estas definiciones de profundizaran en [***Tipos de razonamiento***]())

[BBeej/Code4Exactas-UBA](https://github.com/BBeej/Code4Exactas-UBA)
