# pep8-cheatsheet

PEP 8 es una guía de estilo para escribir código Python, promoviendo la legibilidad y consistencia. Aquí están sus principales recomendaciones en pocas palabras:

1. **Indentación**: Usa 4 espacios por nivel de indentación, no tabulaciones.
2. **Longitud de línea**: Limita las líneas a un máximo de 79 caracteres.
3. **Líneas en blanco**: Usa líneas en blanco para separar funciones y clases, y dentro de funciones para indicar secciones lógicas.
4. **Importaciones**: Coloca todas las importaciones al comienzo del archivo, separadas en tres grupos: estándar, de terceros y locales.
5. **Espaciado**:
   - No uses espacios alrededor de operadores de asignación dentro de funciones.
   - Usa un espacio alrededor de operadores aritméticos y comparativos.
6. **Nombres de variables y funciones**: Usa `snake_case` para funciones y variables, `CamelCase` para clases, y `UPPERCASE` para constantes.
7. **Comentarios**: Escribe comentarios claros y concisos, y usa docstrings para describir funciones y módulos.
8. **Comillas**: Usa comillas simples o dobles de manera consistente para cadenas de texto.


Estas son algunas de las reglas clave. Para más detalles, consulta la [guía completa de PEP 8](https://peps.python.org/pep-0008/).

Ejemplos en Código
---

## Ejemplos de reglas PEP-8 más importantes

### 1. Indentación
Usa 4 espacios por nivel de indentación.

```python
# Correcto
def funcion_ejemplo():
    if True:
        print("Indentación correcta")
    else:
        print("Indentación correcta")

# Incorrecto (Usando tabulaciones o número incorrecto de espacios)
def funcion_ejemplo():
  if True:
      print("Indentación incorrecta")
```

### 2. Longitud de línea
Limita las líneas a un máximo de 79 caracteres.

```python
# Correcto
def funcion_con_linea_larga():
    texto = "Este es un ejemplo de cómo una línea debe ser dividida para cumplir con PEP-8."
    print(texto)

# Incorrecto (Línea demasiado larga)
def funcion_con_linea_larga(): print("Este es un ejemplo de una línea que es demasiado larga y no cumple con PEP-8.")
```

### 3. Espacios en blanco
Evita espacios en blanco innecesarios.

```python
# Correcto
def suma(a, b):
    return a + b

# Incorrecto (Espacio innecesario después de la coma y antes del paréntesis de cierre)
def suma(a , b ):
    return a + b
```

### 4. Nombres de variables y funciones
Usa `snake_case` para nombres de funciones y variables.

```python
# Correcto
nombre_usuario = "John"
def obtener_datos():
    pass

# Incorrecto (Usando camelCase)
nombreUsuario = "John"
def obtenerDatos():
    pass
```

### 5. Importaciones
Coloca todas las importaciones al principio del archivo.
Usa una importación por línea.

```python
# Correcto
import os
import sys

# Incorrecto (Múltiples importaciones en una línea)
import os, sys
```

### 6. Comentarios y Docstrings
Usa comentarios para explicar el porqué del código, no el qué.
Utiliza docstrings para describir el propósito de una función o módulo.

```python
# Correcto
def suma(a, b):
    """Devuelve la suma de a y b."""
    return a + b

# Incorrecto (Falta de docstring)
def suma(a, b):
    return a + b
```

### 7. Organización del Código
Coloca una línea en blanco entre funciones y clases.

```python
# Correcto
class Ejemplo:
    def __init__(self, valor):
        self.valor = valor

    def metodo(self):
        pass

def funcion_ejemplo():
    pass

# Incorrecto (Sin línea en blanco entre clase y función)
class Ejemplo:
    def __init__(self, valor):
        self.valor = valor
    def metodo(self):
        pass
def funcion_ejemplo():
    pass
```

### 8. Espaciado alrededor de operadores
Usa un único espacio antes y después de los operadores.

```python
# Correcto
x = 1 + 2
y = x * 3

# Incorrecto (Sin espacios alrededor de los operadores)
x=1+2
y=x*3
```

### 9. Usar constantes
Define constantes en mayúsculas y con guiones bajos.

```python
# Correcto
PI = 3.14159

# Incorrecto (Usando minúsculas)
pi = 3.14159
```

---

Estos ejemplos cubren algunas de las reglas más esenciales de PEP-8, ayudando a mantener tu código legible y bien estructurado.
