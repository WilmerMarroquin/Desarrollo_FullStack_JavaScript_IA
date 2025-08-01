[🏠 **Volver al Índice de Navegación**](../../../NAVEGACION-DOCUMENTOS.md)

---

# 📈 Analizador de Datos - Proyecto de Estructuras de Datos

## 📝 **Descripción del Proyecto**
Crear un sistema de análisis de datos que procese información numérica utilizando métodos funcionales avanzados para calcular estadísticas, generar reportes y visualizar tendencias de manera programática.

---

## 🎯 **Objetivos de Aprendizaje**
- Dominar **métodos funcionales** (map, filter, reduce)
- Practicar **agregaciones y cálculos** estadísticos
- Implementar **transformación de datos** complejos
- Usar **encadenamiento de métodos** (method chaining)
- Trabajar con **números, fechas y análisis** matemático

---

## 🔧 **Funcionalidades Requeridas**

### ✅ **Análisis Estadístico**
- 📊 **Calcular promedio, mediana, moda** de datasets
- 📈 **Encontrar máximo y mínimo** con detalles
- 📉 **Calcular desviación estándar** y varianza
- 🔢 **Contar frecuencias** de valores únicos

### ✅ **Procesamiento de Datos**
- 🔄 **Transformar arrays** (normalizar, escalar, formatear)
- 🎯 **Filtrar por rangos** y condiciones múltiples
- 📋 **Agrupar datos** por categorías o criterios
- 🧮 **Operaciones matemáticas** en batch

### ✅ **Reportes y Análisis**
- 📑 **Generar reportes** estadísticos detallados
- 📅 **Análisis temporal** (por meses, años, períodos)
- 🏆 **Top N elementos** (mayores, menores, frecuentes)
- 📊 **Comparar datasets** múltiples

---

## 📋 **Estructura Esperada**

```javascript
// Arrays de datos para análisis
let datosVentas = [];
let datosTemperaturas = [];
let datosCalificaciones = [];

// Funciones estadísticas básicas
function calcularPromedio(datos) { /* tu código */ }
function calcularMediana(datos) { /* tu código */ }
function calcularModa(datos) { /* tu código */ }
function encontrarExtremos(datos) { /* tu código */ }

// Funciones estadísticas avanzadas
function calcularDesviacionEstandar(datos) { /* tu código */ }
function calcularVarianza(datos) { /* tu código */ }
function contarFrecuencias(datos) { /* tu código */ }
function calcularPercentiles(datos, percentil) { /* tu código */ }

// Funciones de transformación
function normalizarDatos(datos) { /* tu código */ }
function escalarDatos(datos, min, max) { /* tu código */ }
function filtrarPorRango(datos, minimo, maximo) { /* tu código */ }
function agruparPorCriterio(datos, criterio) { /* tu código */ }

// Funciones de análisis
function generarReporte(datos, titulo) { /* tu código */ }
function compararDatasets(datos1, datos2) { /* tu código */ }
function analizarTendencias(datos) { /* tu código */ }
function obtenerTopN(datos, n, orden) { /* tu código */ }

// Función principal del analizador
function analizadorDatos() {
    // Cargar datos de ejemplo
    // Mostrar menú de análisis
    // Procesar selección del usuario
    // Mostrar resultados detallados
}

// Ejecutar analizador
analizadorDatos();
```

---

## 🧪 **Casos de Prueba**

Asegúrate de que tu analizador maneje estos casos:

```javascript
// Datos de ejemplo para pruebas
const ventasMensuales = [1200, 1500, 1800, 1300, 2100, 1900, 2300, 2000, 1700, 2200, 2500, 2800];
const temperaturas = [18.5, 22.1, 25.3, 19.8, 21.4, 26.7, 23.2, 20.9, 24.1, 22.8];
const calificaciones = [85, 92, 78, 94, 87, 91, 82, 88, 95, 79, 86, 93];

// Estadísticas básicas
calcularPromedio(ventasMensuales) → 1925
calcularMediana(temperaturas) → 22.15
calcularModa(calificaciones) → "No hay moda" (todos únicos)
encontrarExtremos(ventasMensuales) → {min: 1200, max: 2800, rango: 1600}

// Estadísticas avanzadas
calcularDesviacionEstandar(temperaturas) → 2.89 (aproximado)
contarFrecuencias([1,2,2,3,3,3]) → {1: 1, 2: 2, 3: 3}
calcularPercentiles(calificaciones, 90) → 94.1

// Transformaciones
normalizarDatos([10, 20, 30]) → [0, 0.5, 1]
escalarDatos([1, 2, 3], 0, 100) → [0, 50, 100]
filtrarPorRango(calificaciones, 85, 95) → [85, 92, 94, 87, 91, 88, 95, 86, 93]

// Análisis
obtenerTopN(ventasMensuales, 3, 'desc') → [2800, 2500, 2300]
analizarTendencias(ventasMensuales) → "Tendencia creciente: +133.33 por mes"

// Casos especiales
calcularPromedio([]) → "Error: Array vacío"
calcularMediana([1]) → 1 (un solo elemento)
normalizarDatos([5, 5, 5]) → "Error: Todos los valores son iguales"
```

---

## 💾 **Estructura de Datos Sugerida**

```javascript
// Para análisis más complejos, usa objetos con metadatos:
const datasetEjemplo = {
    id: "VENTAS_2024",
    titulo: "Ventas Mensuales 2024",
    descripcion: "Ventas en miles de euros por mes",
    fechaCreacion: new Date(),
    datos: [1200, 1500, 1800, 1300, 2100, 1900],
    metadatos: {
        unidad: "euros",
        frecuencia: "mensual",
        fuente: "Sistema de ventas"
    }
};

// Para datos temporales:
const datosTempo = [
    {fecha: "2024-01", valor: 1200, categoria: "Q1"},
    {fecha: "2024-02", valor: 1500, categoria: "Q1"},
    {fecha: "2024-03", valor: 1800, categoria: "Q1"}
];
```

---

## ⏱️ **Tiempo Estimado**
**2.5-3.5 horas** (dependiendo de tu nivel)

## 🎓 **Nivel de Dificultad**
🔴 **AVANZADO** - Requiere dominio de métodos funcionales y matemáticas

---

## 💡 **Pistas para Empezar**

1. **Empieza con reduce**: Es la base de muchos cálculos estadísticos
2. **Valida datos**: Siempre verifica que el array no esté vacío
3. **Usa sort()**: Para mediana y percentiles necesitas datos ordenados
4. **Encadena métodos**: `.filter().map().reduce()` es muy poderoso
5. **Maneja decimales**: Usa `toFixed()` para resultados legibles
6. **Crea datasets de prueba**: Genera datos realistas para probar

---

## 🎯 **Conceptos Clave que Practicarás**

- **Array.reduce()** - Agregaciones y cálculos acumulativos
- **Array.map()** - Transformaciones elemento por elemento
- **Array.filter()** - Filtrado por múltiples condiciones
- **Array.sort()** - Ordenamiento para cálculos estadísticos
- **Math object** - Funciones matemáticas avanzadas
- **Method chaining** - Encadenamiento de operaciones
- **Higher-order functions** - Funciones que reciben/retornan funciones
- **Data validation** - Verificación de tipos y rangos

---

## 🔍 **Algoritmos Estadísticos Sugeridos**

```javascript
// Ejemplos de implementaciones avanzadas que puedes intentar:

// Coeficiente de correlación entre dos datasets
function calcularCorrelacion(datos1, datos2) {
    if (datos1.length !== datos2.length) return null;
    
    const promedio1 = calcularPromedio(datos1);
    const promedio2 = calcularPromedio(datos2);
    
    const numerador = datos1.reduce((sum, val, i) => 
        sum + (val - promedio1) * (datos2[i] - promedio2), 0);
    
    const denominador = Math.sqrt(
        datos1.reduce((sum, val) => sum + Math.pow(val - promedio1, 2), 0) *
        datos2.reduce((sum, val) => sum + Math.pow(val - promedio2, 2), 0)
    );
    
    return numerador / denominador;
}

// Análisis de tendencia usando regresión lineal simple
function calcularTendencia(datos) {
    const n = datos.length;
    const x = Array.from({length: n}, (_, i) => i + 1);
    
    const sumX = x.reduce((a, b) => a + b, 0);
    const sumY = datos.reduce((a, b) => a + b, 0);
    const sumXY = x.reduce((sum, xi, i) => sum + xi * datos[i], 0);
    const sumXX = x.reduce((sum, xi) => sum + xi * xi, 0);
    
    const pendiente = (n * sumXY - sumX * sumY) / (n * sumXX - sumX * sumX);
    const intercepto = (sumY - pendiente * sumX) / n;
    
    return {pendiente, intercepto, tendencia: pendiente > 0 ? 'creciente' : 'decreciente'};
}
```

---

**🚀 ¡Cuando termines, tendrás un analizador de datos profesional y habrás dominado los métodos funcionales más poderosos de JavaScript!**

---

[🔙 **Volver al Libro Principal**](../ESTRUCTURAS-DATOS-LIBRO.md) | [🏠 **Índice General**](../../../README.md) | [📚 **Navegación**](../../../NAVEGACION-DOCUMENTOS.md) | [📝 **Ver Cheatsheet**](../CHEATSHEET-VISUAL.md)
