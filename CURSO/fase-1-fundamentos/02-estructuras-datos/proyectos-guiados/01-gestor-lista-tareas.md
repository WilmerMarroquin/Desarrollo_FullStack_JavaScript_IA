[🏠 **Volver al Índice de Navegación**](../../../NAVEGACION-DOCUMENTOS.md)

---

# 📊 Gestor de Lista de Tareas - Proyecto de Estructuras de Datos

## 📝 **Descripción del Proyecto**
Crear un sistema de gestión de tareas que permita agregar, eliminar, marcar como completadas y organizar tareas utilizando arrays y métodos básicos de manipulación.

---

## 🎯 **Objetivos de Aprendizaje**
- Dominar **creación y manipulación de arrays**
- Practicar **métodos push, pop, splice, indexOf**
- Implementar **operaciones CRUD** (Create, Read, Update, Delete)
- Usar **bucles for y for...of** para iterar arrays
- Organizar datos con **objetos dentro de arrays**

---

## 🔧 **Funcionalidades Requeridas**

### ✅ **Gestión Básica**
- ➕ **Agregar tarea** nueva al final de la lista
- ❌ **Eliminar tarea** por índice o título
- ✅ **Marcar tarea como completada/pendiente**
- 📋 **Mostrar todas las tareas** con su estado

### ✅ **Operaciones de Lista**
- 🔢 **Contar tareas** (total, completadas, pendientes)
- 🔍 **Buscar tarea** por título o palabra clave
- 🧹 **Limpiar tareas completadas**
- 📊 **Mostrar estadísticas** del progreso

### ✅ **Funcionalidades Extra**
- 🔄 **Reordenar tareas** (mover arriba/abajo)
- ⭐ **Marcar tareas como importantes**
- 📅 **Filtrar por estado** (completadas, pendientes, importantes)

---

## 📋 **Estructura Esperada**

```javascript
// Array principal para almacenar tareas
let listaTareas = [];

// Funciones básicas de gestión
function agregarTarea(titulo, importante = false) { /* tu código */ }
function eliminarTarea(indice) { /* tu código */ }
function marcarCompletada(indice) { /* tu código */ }
function mostrarTareas() { /* tu código */ }

// Funciones de búsqueda y filtrado
function buscarTarea(termino) { /* tu código */ }
function filtrarPorEstado(estado) { /* tu código */ }
function contarTareas() { /* tu código */ }

// Funciones de utilidad
function limpiarCompletadas() { /* tu código */ }
function moverTarea(indiceOrigen, indiceDestino) { /* tu código */ }

// Función principal que maneja el menú
function gestorTareas() {
    // Mostrar menú de opciones
    // Capturar elección del usuario
    // Ejecutar función correspondiente
}

// Ejecutar el gestor
gestorTareas();
```

---

## 🧪 **Casos de Prueba**

Asegúrate de que tu gestor maneje estos casos:

```javascript
// Operaciones básicas
agregarTarea("Estudiar JavaScript") → Tarea agregada en índice 0
agregarTarea("Hacer ejercicio", true) → Tarea importante agregada
mostrarTareas() → Lista todas las tareas con estado

// Gestión de tareas
marcarCompletada(0) → "Estudiar JavaScript" marcada como ✅
eliminarTarea(1) → "Hacer ejercicio" eliminada de la lista
contarTareas() → {total: 1, completadas: 1, pendientes: 0}

// Búsqueda y filtrado
buscarTarea("JavaScript") → Encuentra la tarea con "JavaScript"
filtrarPorEstado("completadas") → Muestra solo tareas ✅
limpiarCompletadas() → Elimina todas las tareas completadas

// Casos especiales
eliminarTarea(99) → "Error: Índice inválido"
agregarTarea("") → "Error: El título no puede estar vacío"
```

---

## 💾 **Estructura de Datos Sugerida**

```javascript
// Cada tarea será un objeto con esta estructura:
const tareaEjemplo = {
    id: 1,                    // Identificador único
    titulo: "Estudiar Arrays", // Texto de la tarea
    completada: false,        // Estado de completado
    importante: false,        // Marcada como importante
    fechaCreacion: new Date() // Cuándo se creó
};

// El array principal contendrá objetos como este:
let listaTareas = [tareaEjemplo];
```

---

## ⏱️ **Tiempo Estimado**
**1.5-2.5 horas** (dependiendo de tu nivel)

## 🎓 **Nivel de Dificultad**
🟢 **BÁSICO** - Ideal para empezar con arrays y objetos

---

## 💡 **Pistas para Empezar**

1. **Empieza con array simple**: Primero usa strings, luego evoluciona a objetos
2. **Una función a la vez**: Implementa `agregarTarea()` primero y pruébala
3. **Usa console.log()**: Para verificar que tu array se modifica correctamente
4. **Maneja índices**: Siempre valida que el índice exista antes de usarlo
5. **Piensa en la experiencia**: ¿Cómo te gustaría que se vea el menú?

---

## 🎯 **Conceptos Clave que Practicarás**

- **Array.push()** - Agregar elementos al final
- **Array.splice()** - Eliminar elementos por índice
- **Array.indexOf()** - Encontrar posición de elemento
- **Array.filter()** - Filtrar elementos por condición
- **Array.length** - Obtener tamaño del array
- **for...of** - Iterar sobre elementos
- **Objetos básicos** - Propiedades y valores

---

**🚀 ¡Cuando termines, tendrás un gestor de tareas funcional y habrás dominado los fundamentos de arrays en JavaScript!**

---

[🔙 **Volver al Libro Principal**](../ESTRUCTURAS-DATOS-LIBRO.md) | [🏠 **Índice General**](../../../README.md) | [📚 **Navegación**](../../../NAVEGACION-DOCUMENTOS.md) | [📝 **Ver Cheatsheet**](../CHEATSHEET-VISUAL.md)
