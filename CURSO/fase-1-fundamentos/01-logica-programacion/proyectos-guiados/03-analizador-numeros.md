[🏠 **Volver al Índice de Navegación**](../../../../NAVEGACION-DOCUMENTOS.md)

---

# 📊 Analizador de Números - Proyecto de Lógica

## 📝 **Descripción del Proyecto**
Crear un programa que analice un conjunto de números ingresados por el usuario y calcule estadísticas básicas usando arrays, bucles y funciones matemáticas.

---

## 🎯 **Objetivos de Aprendizaje**
- Trabajar con **arrays** y métodos básicos
- Aplicar **bucles for** para procesamiento de datos
- Usar **funciones matemáticas** (Math.max, Math.min)
- Implementar **algoritmos de búsqueda y ordenamiento** básicos
- Calcular **estadísticas** usando lógica programática

---

## 🔧 **Funcionalidades Requeridas**

### ✅ **Entrada de Datos**
- Pedir al usuario **cuántos números** quiere ingresar
- **Recibir y validar** cada número
- **Almacenar** en un array

### ✅ **Análisis Básico**
- Calcular **suma total**
- Calcular **promedio** (media aritmética)
- Encontrar **número mayor**
- Encontrar **número menor**
- **Contar** cuántos números hay

### ✅ **Análisis Avanzado**
- Contar **números pares** e **impares**
- Encontrar **números positivos** y **negativos**
- Calcular **rango** (diferencia entre mayor y menor)
- **Ordenar** la lista de menor a mayor

---

## 📋 **Estructura Esperada**

```javascript
// Función para recopilar números del usuario
function recopilarNumeros() { /* tu código */ }

// Funciones de análisis
function calcularSuma(numeros) { /* tu código */ }
function calcularPromedio(numeros) { /* tu código */ }
function encontrarMayor(numeros) { /* tu código */ }
function encontrarMenor(numeros) { /* tu código */ }
function contarPares(numeros) { /* tu código */ }
function contarImpares(numeros) { /* tu código */ }

// Función que muestra todos los resultados
function mostrarAnalisis(numeros) { /* tu código */ }

// Función principal
function analizadorNumeros() {
    const numeros = recopilarNumeros();
    mostrarAnalisis(numeros);
}

// Ejecutar el programa
analizadorNumeros();
```

---

## 🧪 **Ejemplo de Funcionamiento**

```
📊 ANALIZADOR DE NÚMEROS

¿Cuántos números quieres analizar? 5

Ingresa el número 1: 10
Ingresa el número 2: -3
Ingresa el número 3: 7
Ingresa el número 4: 22
Ingresa el número 5: 8

📈 RESULTADOS DEL ANÁLISIS:
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

🔢 Números ingresados: [10, -3, 7, 22, 8]
📊 Cantidad total: 5 números

🧮 ESTADÍSTICAS BÁSICAS:
├─ Suma total: 44
├─ Promedio: 8.8
├─ Número mayor: 22
├─ Número menor: -3
└─ Rango: 25

🎭 CLASIFICACIÓN:
├─ Números pares: 3 (10, 22, 8)
├─ Números impares: 2 (-3, 7)
├─ Números positivos: 4
└─ Números negativos: 1

📋 Lista ordenada: [-3, 7, 8, 10, 22]
```

---

## 🧠 **Conceptos Clave a Aplicar**

### 📦 **Trabajo con Arrays**
```javascript
const numeros = [];
numeros.push(valor); // Agregar elemento
numeros.length;      // Cantidad de elementos
```

### 🔄 **Bucles para Análisis**
```javascript
for (let i = 0; i < numeros.length; i++) {
    // Procesar cada número
}
```

### 🧮 **Algoritmos de Búsqueda**
```javascript
function encontrarMayor(array) {
    let mayor = array[0];
    for (let i = 1; i < array.length; i++) {
        if (array[i] > mayor) {
            mayor = array[i];
        }
    }
    return mayor;
}
```

---

## ⏱️ **Tiempo Estimado**
**2-3 horas** (incluyendo todas las funcionalidades)

## 🎓 **Nivel de Dificultad**
🟡 **INTERMEDIO** - Combina múltiples conceptos

---

## 💡 **Pistas para Empezar**

1. **Comienza simple**: Recoge los números y guárdalos en un array
2. **Una función a la vez**: Implementa suma, promedio, etc. por separado
3. **Usa bucles for**: Para recorrer el array en cada análisis
4. **Valida las entradas**: Asegúrate de que sean números válidos
5. **Organiza la salida**: Haz que los resultados se vean bien formateados

---

## 🎯 **Desafío Extra (Opcional)**

- **Detectar números repetidos** y mostrar cuántas veces aparecen
- **Calcular la mediana** (valor del medio cuando están ordenados)
- **Permitir decimales** y manejar redondeo apropiado

---

**🚀 ¡Este proyecto te dará experiencia sólida con arrays, bucles y lógica matemática!**

---

[🔙 **Volver al Libro Principal**](../LOGICA-PROGRAMACION-LIBRO.md) | [🏠 **Índice General**](../../../../README.md) | [📚 **Navegación**](../../../../NAVEGACION-DOCUMENTOS.md) | [📝 **Ver Cheatsheet**](../CHEATSHEET-VISUAL.md)
