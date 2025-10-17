#  Calculadora Científica en Kotlin

Una **calculadora científica orientada a objetos** escrita en **Kotlin**, diseñada para demostrar el uso de:
- **Herencia**
- **Polimorfismo (sobrecarga de operadores)**
- **Encapsulamiento**
- **Análisis de expresiones con precedencia de operadores (PEMDAS)**

---

##  Características

###  Calculadora Base
La clase base `Calculator` soporta:
- Suma `sum(a, b)`
- Resta `sub(a, b)`
- Multiplicación `mul(a, b)`
- División `div(a, b)` *(con verificación de división por cero)*
- Operaciones de memoria:
  - `Mplus(value)`
  - `Mminus(value)`
  - `MR()` *(recuperar memoria)*
  - `clearMemory()` *(limpiar memoria)*

---

### Calculadora Científica
`ScientificCalculator` **hereda** de `Calculator` y amplía su funcionalidad con:

####  Operaciones Matemáticas
- `pow(base, exponent)`
- `sqrt(value, n)` – calcula la raíz n-ésima, genera error para entradas negativas o grado de raíz cero

####  Funciones Logarítmicas
- `log10(value)` – logaritmo base 10
- `ln(value)` – logaritmo natural (base e)

####  Funciones Trigonométricas
- `sinDeg(angle)`, `cosDeg(angle)`, `tanDeg(angle)`
- `sinRad(angle)`, `cosRad(angle)`, `tanRad(angle)`
- `toDeg(radians)`, `toRad(degrees)`

---

###  Sobrecarga de Operadores
Permite operaciones matemáticas intuitivas mediante la **sobrecarga de operadores** en Kotlin:

```kotlin
val c1 = ScientificCalculator()
val c2 = ScientificCalculator()
val result = c1 + c2  // usa sobrecarga de operadores
```
---

## Conceptos Demostrados
- **Herencia:** `ScientificCalculator` extiende `Calculator`.  
- **Polimorfismo:** Se implementa la sobrecarga de operadores y funciones personalizadas.  
- **Encapsulamiento:** Uso de variables privadas y acceso mediante métodos públicos.  
- **Análisis de expresiones:** Se manejan expresiones con jerarquía de operadores (PEMDAS).

## Manera de ejecucion

- **Acceda al siguiente link:** https://pl.kotl.in/4XJNVzrox?theme=darcula
