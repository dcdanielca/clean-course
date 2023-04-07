# Conceptos claves

- **Deuda técnica:** Falta de calidad en el código, que genera una deuda que repercutirà en costos futuros.


- **Refactorización:** Es un proceso que tiene como objetivo mejorar el código sin alterar su comportamiento para que sea mas entendible y tolerable a cambios.

- **Clean code**: Código que sea fácil de leer y entender por otra persona (o tu mismo del futuro)

# Clean code

- Nombres de variables, clases, métodos, etc. Deben ser pronunciables.

- Ausencia de información técnica en nombres (por ejemplo Abstract, Interface, Mixin en el nombre)



## Recomendaciones de funciones

- Usar máximo 3 argumentos posicionales
- Simplicidad es fundamental
- Funciones de una sola línea sin causar complejidad
- Menos de 20 líneas
- Evitar el uso del "else"
- Priorizar uso de la condicional ternaria


# Principio DRY

Don't Repeat Yourself

- Simplemente es evitar tener duplicidad de código
- Simplifica pruebas
- Ayuda a centralizar procesos


# Estructura recomendada de una clase

1. Propiedades estáticas
2. Propiedades públicas de último

## Métodos

1. Empezar por constuctores estáticos
2. Luego el constructor
3. Métodos estáticos
4. Metodos privados
5. Resto de metodos ordenados de mayor a menor importancia
6. Gettters y Setters al final


# Code Smells STUPID

- **S**ingleton: patrón singleton (si bien tiene ventajas, tiene contras también, debe usarse con cuidado, tratar de no usarlo)
- **T**ight Coupling: alto acoplamiento. Lo ideal es tener bajo acoplamiento y buena cohesión. Alto acomplamiento provoca efecto domino al realizar algún cambio en código. La buena cohesión se refiere a que la clase solo hace lo que debería estar haciendo, no está cargado de gran variedad de funcionalidades (SRP)
- **U**nestability: Código no probable. Dificilmente testeable debido al alto acoplamiento, muchas dependencias no inyectadas, uso de singleton.
- **P**remature optimization: Optimizaciones prematuras, no anticiparnos a los requisitos que añaden complejidad accidental
- **I**ndescriptive naming: Nombres poco descriptivos
- **D**uplication: Duplicidad de código, no aplicar DRY


## Otros "code smells"

- **Inflación:** Métodos con muchas líneas de código o clases muy grandes.
- **Obsesión primitiva:** Abusar del uso de variables primitivas. Lo correcto sería reemplazar todas estas variables en algun módulo u objeto que mantenga más simple todo.
- **Lista larga de parámetros** 


# Principios SOLID

S – Single Responsibility Principle (SRP)
O – Open/Closed Principle (OCP)
L – Liskov Substitution Principle (LSP)
I – Interface Segregation Principle (ISP)
D – Dependency Inversion Principle (DIP)


