[🏠 **Volver al Índice de Navegación**](../../../../NAVEGACION-DOCUMENTOS.md)

---

# 🧮 Calculadora Básica - Proyecto de Lógica

## 📝 **Descripción del Proyecto**
Crear una calculadora que realice operaciones aritméticas básicas utilizando funciones, condicionales y validación de datos.

---

## 🎯 **Objetivos de Aprendizaje**
- Aplicar **declaración y uso de funciones**
- Practicar **operadores aritméticos**
- Implementar **validación de entrada**
- Usar **condicionales** para control de flujo
- Organizar código de forma **modular y reutilizable**

---

## 🔧 **Funcionalidades Requeridas**

### ✅ **Funciones Básicas**
- ➕ **Suma** de dos números
- ➖ **Resta** de dos números  
- ✖️ **Multiplicación** de dos números
- ➗ **División** de dos números (con validación división por cero)

### ✅ **Validaciones**
- Verificar que los inputs sean **números válidos**
- **Manejo de errores** para entradas inválidas
- **Mensajes informativos** para el usuario

### ✅ **Interfaz**
- **Menú interactivo** en consola
- **Entrada de datos** por prompt o parámetros
- **Salida clara** y formateada de resultados

---

## 📋 **Estructura Esperada**

```javascript
// Funciones puras para operaciones
function sumar(a, b) { /* tu código */ }
function restar(a, b) { /* tu código */ }
function multiplicar(a, b) { /* tu código */ }
function dividir(a, b) { /* tu código */ }

// Función de validación
function esNumeroValido(valor) { /* tu código */ }

// Función principal que organiza la lógica
function calculadora() { /* tu código */ }

// Ejecutar la calculadora
calculadora();
```

---

## 🧪 **Casos de Prueba**

Asegúrate de que tu calculadora maneje estos casos:

```javascript
// Operaciones válidas
sumar(5, 3) → 8
restar(10, 4) → 6
multiplicar(7, 6) → 42
dividir(15, 3) → 5

// Casos especiales
dividir(10, 0) → "Error: División por cero"
sumar("abc", 5) → "Error: Entrada inválida"
```

---

## ⏱️ **Tiempo Estimado**
**1-2 horas** (dependiendo de tu nivel)

## 🎓 **Nivel de Dificultad**
🟢 **BÁSICO** - Ideal para empezar con proyectos

---

## 💡 **Pistas para Empezar**

1. **Empieza simple**: Crea primero las funciones básicas sin validación
2. **Prueba cada función**: Usa `console.log()` para verificar que funcionan
3. **Añade validaciones**: Una vez que las operaciones funcionen
4. **Organiza el flujo**: Crea la función principal al final

---

**🚀 ¡Cuando termines, tendrás tu primera aplicación funcional usando lógica de programación!**

---

[🔙 **Volver al Libro Principal**](../LOGICA-PROGRAMACION-LIBRO.md) | [🏠 **Índice General**](../../../../README.md) | [📚 **Navegación**](../../../../NAVEGACION-DOCUMENTOS.md) | [📝 **Ver Cheatsheet**](../CHEATSHEET-VISUAL.md)
