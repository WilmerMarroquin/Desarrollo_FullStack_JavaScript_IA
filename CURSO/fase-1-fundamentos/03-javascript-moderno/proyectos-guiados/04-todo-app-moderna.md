[🏠 **Volver al Índice de Navegación**](../../../NAVEGACION-DOCUMENTOS.md)

---

# 📝 Todo App Moderna - Proyecto ES6+

## 📝 **Descripción del Proyecto**
Construir una aplicación de tareas completa usando todas las características ES6+: clases, async/await, destructuring, módulos y local storage.

---

## 🎯 **Objetivos de Aprendizaje**
- Aplicar **destructuring** en operaciones CRUD
- Practicar **spread operator** para inmutabilidad
- Implementar **async/await** para storage
- Usar **array methods** funcionales
- Organizar con **módulos ES6**

---

## 🔧 **Funcionalidades Requeridas**

### ✅ **Gestión de Tareas**
- ➕ **Agregar tareas** con validación
- ✅ **Marcar completadas** con toggle
- ❌ **Eliminar tareas** con confirmación
- ✏️ **Editar tareas** inline

### ✅ **Filtros y Búsqueda**
- 🔍 **Buscar** por texto
- 📋 **Filtrar** por estado (all, active, completed)
- 📊 **Contadores** dinámicos
- 🧹 **Limpiar completadas**

### ✅ **Persistencia**
- 💾 **LocalStorage** con async/await
- 🔄 **Auto-save** en cada cambio
- 📱 **Responsive** design
- 🎨 **Theme switcher** (bonus)

---

## 📋 **Estructura Esperada**

```javascript
// App principal
class TodoApp {
    constructor() {
        /* tu código */
    }
    
    async loadTodos() {
        /* tu código con async/await */
    }
    
    addTodo = (text) => {
        /* tu código con spread operator */
    }
    
    toggleTodo = (id) => {
        /* tu código con map y destructuring */
    }
}

// Storage helper
class StorageManager {
    /* tu implementación */
}
```

---

## 🧪 **Datos de Ejemplo**

```javascript
// Estructura de datos esperada
const todoExample = {
    id: Date.now(),
    text: 'Aprender ES6+',
    completed: false,
    createdAt: new Date(),
    priority: 'medium'
};
```

---

## ✅ **Criterios de Evaluación**

- [ ] **CRUD completo** implementado
- [ ] **Destructuring** usado consistentemente
- [ ] **Spread operator** para inmutabilidad
- [ ] **Array methods** en lugar de loops
- [ ] **Async/await** para storage
- [ ] **Módulos** para organización
- [ ] **LocalStorage** funcional

---

[📁 **Proyecto Anterior**](./03-generador-componentes.md) | [📁 **Siguiente Proyecto**](./05-weather-app-es6.md) | [🏠 **Volver a Ejercicios**](../ejercicios-practicos/README-EJERCICIOS.md)
