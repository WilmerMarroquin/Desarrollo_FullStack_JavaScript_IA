[🏠 **Volver al Índice de Navegación**](../../../NAVEGACION-DOCUMENTOS.md)

---

# 🎨 Generador de Patrones - Proyecto de Lógica 🎯 Generador de Patrones - Proyecto de Lógica

## 📝 **Descripción del Proyecto**
Crear un programa que genere diferentes patrones visuales usando bucles anidados, condicionales y lógica matemática para crear formas con asteriscos, números o letras.

---

## 🎯 **Objetivos de Aprendizaje**
- Dominar **bucles anidados** (for dentro de for)
- Aplicar **lógica matemática** para posicionamiento
- Usar **condicionales** para crear formas específicas
- Practicar **concatenación de strings**
- Desarrollar **pensamiento espacial** y algorítmico

---

## 🔧 **Funcionalidades Requeridas**

### ✅ **Patrones Básicos**
- **Cuadrado sólido** de asteriscos
- **Cuadrado hueco** (solo bordes)
- **Triángulo rectángulo** creciente
- **Triángulo rectángulo** decreciente

### ✅ **Patrones Avanzados**
- **Pirámide centrada** de asteriscos
- **Diamante** completo
- **Escalera** de números
- **Tablero de ajedrez** con caracteres alternos

### ✅ **Personalización**
- Permitir al usuario **elegir el tamaño**
- **Diferentes caracteres** (*, #, +, etc.)
- **Múltiples patrones** en un solo programa

---

## 📋 **Estructura Esperada**

```javascript
// Funciones para patrones básicos
function generarCuadrado(tamaño, caracter) { /* tu código */ }
function generarCuadradoHueco(tamaño, caracter) { /* tu código */ }
function generarTriangulo(tamaño, caracter) { /* tu código */ }

// Funciones para patrones avanzados
function generarPiramide(altura, caracter) { /* tu código */ }
function generarDiamante(tamaño, caracter) { /* tu código */ }
function generarEscalera(altura) { /* tu código */ }

// Función de menú
function mostrarMenu() { /* tu código */ }

// Función principal
function generadorPatrones() {
    // Mostrar opciones
    // Obtener selección del usuario
    // Ejecutar patrón seleccionado
}

// Iniciar programa
generadorPatrones();
```

---

## 🧪 **Ejemplos de Patrones**

### 🟦 **Cuadrado Sólido (5x5)**
```
* * * * *
* * * * *
* * * * *
* * * * *
* * * * *
```

### 🔲 **Cuadrado Hueco (5x5)**
```
* * * * *
*       *
*       *
*       *
* * * * *
```

### 🔺 **Triángulo Creciente**
```
*
* *
* * *
* * * *
* * * * *
```

### 🏔️ **Pirámide Centrada**
```
    *
   * *
  * * *
 * * * *
* * * * *
```

### 💎 **Diamante**
```
  *
 * *
* * *
 * *
  *
```

### 🪜 **Escalera de Números**
```
1
1 2
1 2 3
1 2 3 4
1 2 3 4 5
```

---

## 🧠 **Conceptos Clave a Aplicar**

### 🔄 **Bucles Anidados**
```javascript
for (let fila = 0; fila < altura; fila++) {
    for (let columna = 0; columna < ancho; columna++) {
        // Lógica para cada posición
    }
}
```

### 🧮 **Lógica de Posicionamiento**
```javascript
// Para pirámide centrada
const espacios = altura - fila - 1;
const asteriscos = fila + 1;
```

### 🎭 **Condicionales para Formas**
```javascript
// Para cuadrado hueco
if (fila === 0 || fila === altura-1 || columna === 0 || columna === ancho-1) {
    proceso += caracter;
} else {
    proceso += ' ';
}
```

---

## ⏱️ **Tiempo Estimado**
**2.5-3.5 horas** (todos los patrones)

## 🎓 **Nivel de Dificultad**
🟡 **INTERMEDIO** - Requiere lógica espacial

---

## 💡 **Pistas para Empezar**

1. **Empieza con cuadrado sólido**: Es el más simple (dos bucles anidados)
2. **Visualiza mentalmente**: Dibuja en papel antes de programar
3. **Usa console.log()**: Para imprimir cada línea del patrón
4. **Prueba con tamaños pequeños**: Más fácil de debuggear
5. **Un patrón a la vez**: No intentes hacer todos juntos

---

## 🎯 **Algoritmo General**

```javascript
function generarPatron(altura) {
    for (let fila = 0; fila < altura; fila++) {
        let linea = '';
        
        // Calcular espacios iniciales (si necesario)
        for (let espacio = 0; espacio < espaciosNecesarios; espacio++) {
            linea += ' ';
        }
        
        // Calcular caracteres principales
        for (let columna = 0; columna < caracteresEnFila; columna++) {
            linea += caracter;
        }
        
        console.log(linea);
    }
}
```

---

## 🎯 **Desafío Extra (Opcional)**

- **Patrón de números primos** en forma triangular
- **Espiral de números** hacia adentro
- **Patrón de letras** del alfabeto
- **Fractal simple** (triángulo de Sierpinski básico)

---

**🚀 ¡Este proyecto desarrollará tu habilidad para pensar en algoritmos complejos y visualizar lógica espacial!**

---

[🔙 **Volver al Libro Principal**](../LOGICA-PROGRAMACION-LIBRO.md) | [🏠 **Índice General**](../../../README.md) | [📚 **Navegación**](../../../NAVEGACION-DOCUMENTOS.md) | [📝 **Ver Cheatsheet**](../CHEATSHEET-VISUAL.md)
