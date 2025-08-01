[🏠 **Volver al Índice de Navegación**](../../../../NAVEGACION-DOCUMENTOS.md)

---

# � **PROYECTO GUIADO 1: Refactor App Moderna**

## Transformando JavaScript Legacy a ES6+ Profesional

> **🎯 "Un proyecto real de refactoring donde llevarás una aplicación ES5 completa hacia JavaScript moderno ES6+. La transformación que todo desarrollador debe dominar."**

---

## 📋 **Descripción del Proyecto**

### 🎯 **Objetivo Principal**
Refactorizar una aplicación completa de gestión de tareas escrita en JavaScript ES5 (estilo 2014) hacia JavaScript moderno ES6+ (estilo 2024).

### 🎨 **Lo que Aprenderás**
- **🔄 Refactoring sistemático** ES5 → ES6+
- **⚡ Arrow functions** en contextos reales
- **🎭 Destructuring** para código más limpio
- **📦 Módulos ES6** para organización profesional
- **🔄 Promises/Async-Await** para manejo asíncrono
- **🏛️ Clases ES6** para POO moderna

### ⏱️ **Tiempo Estimado**
**90-120 minutos** (sesión única o dividida en 3 partes de 30-40 min)

---

## 🏗️ **Estructura del Proyecto**

### 📁 **Código de Partida (ES5 Legacy)**

```javascript
// === ANTES: app-legacy.js ===
// ❌ Aplicación ES5 con todos los antipatrones típicos

var TaskManager = function() {
    this.tasks = [];
    this.filter = 'all';
    this.idCounter = 1;
};

TaskManager.prototype.addTask = function(text) {
    var task = {
        id: this.idCounter++,
        text: text,
        completed: false,
        createdAt: new Date()
    };
    this.tasks.push(task);
    this.render();
};

TaskManager.prototype.toggleTask = function(id) {
    for (var i = 0; i < this.tasks.length; i++) {
        if (this.tasks[i].id === id) {
            this.tasks[i].completed = !this.tasks[i].completed;
            break;
        }
    }
    this.render();
};

TaskManager.prototype.deleteTask = function(id) {
    var newTasks = [];
    for (var i = 0; i < this.tasks.length; i++) {
        if (this.tasks[i].id !== id) {
            newTasks.push(this.tasks[i]);
        }
    }
    this.tasks = newTasks;
    this.render();
};
```

### 🎯 **Meta: Código Moderno (ES6+)**

```javascript
// === DESPUÉS: app-modern.js ===
// ✅ Aplicación ES6+ con todas las mejores prácticas

class TaskManager {
    constructor() {
        this.tasks = [];
        this.filter = 'all';
        this.idCounter = 1;
    }
    
    addTask = (text) => {
        const task = {
            id: this.idCounter++,
            text,
            completed: false,
            createdAt: new Date()
        };
        
        this.tasks = [...this.tasks, task];
        this.render();
    }
    
    toggleTask = (id) => {
        this.tasks = this.tasks.map(task => 
            task.id === id ? { ...task, completed: !task.completed } : task
        );
        this.render();
    }
    
    deleteTask = (id) => {
        this.tasks = this.tasks.filter(task => task.id !== id);
        this.render();
    }
}
```

---

## 🎯 **Pasos del Refactoring**

### **� PASO 1: Variables y Sintaxis Básica (20 min)**

#### 🎯 Tareas:
1. **var → const/let**: Cambiar todas las declaraciones
2. **Shorthand properties**: `{ text: text }` → `{ text }`
3. **Template literals**: Concatenación → backticks
4. **Arrow functions**: Callbacks simples

### **📍 PASO 2: Funciones y Métodos (25 min)**

#### 🎯 Tareas:
1. **Function → Class**: Convertir constructor
2. **Prototype methods → Class methods**: Modernizar métodos
3. **Arrow functions**: Para métodos que usan this
4. **Method shorthand**: Sintaxis concisa

### **📍 PASO 3: Manipulación de Datos (25 min)**

#### 🎯 Tareas:
1. **Destructuring**: Extraer propiedades elegantemente
2. **Spread operator**: Inmutabilidad en arrays/objetos
3. **Array methods**: map, filter en lugar de loops
4. **Object literal**: Métodos dinámicos

### **📍 PASO 4: Organización y Módulos (20 min)**

#### 🎯 Tareas:
1. **Separar en módulos**: TaskManager, UI, Utils
2. **Export/Import**: Organización profesional
3. **Constants**: Configuración centralizada

---

## 🧪 **Testing y Validación**

### ✅ **Checklist de Completación**

- [ ] **Variables**: Todas `var` convertidas a `const/let`
- [ ] **Functions**: Constructor → Class, métodos → arrow functions
- [ ] **Strings**: Concatenación → template literals
- [ ] **Objects**: Shorthand properties y métodos
- [ ] **Arrays**: Loops → métodos funcionales (map, filter)
- [ ] **Immutability**: Spread operator para updates
- [ ] **Destructuring**: Parámetros y asignaciones
- [ ] **Modules**: Separación en archivos ES6+

---

**🎯 ¿Listo para modernizar tu primer proyecto?**

[📁 **Proyecto 2: API Client**](./02-mini-api-fetcher.md) | [🏠 **Volver a Ejercicios**](../ejercicios-practicos/README-EJERCICIOS.md) | [📚 **Navegación**](../../../../NAVEGACION-DOCUMENTOS.md)
