[🏠 **Volver al Índice de Navegación**](../../../NAVEGACION-DOCUMENTOS.md)

---

# 🔄 Refactor App Moderna - Proyecto ES6+

## 📝 **Descripción del Proyecto**
Transformar una aplicación JavaScript ES5 (legacy) hacia JavaScript moderno ES6+ aplicando todas las características aprendidas.

---

## 🎯 **Objetivos de Aprendizaje**
- Aplicar **transformación ES5 → ES6+**
- Practicar **arrow functions** en contextos reales
- Implementar **destructuring** para código limpio
- Usar **clases ES6** en lugar de funciones constructor
- Organizar código con **módulos ES6**

---

## 🔧 **Funcionalidades Requeridas**

### ✅ **Transformaciones Básicas**
- ⚡ **Variables**: `var` → `const/let`
- 🏷️ **Propiedades**: Shorthand properties
- 📝 **Strings**: Template literals
- ➡️ **Funciones**: Arrow functions apropiadas

### ✅ **Transformaciones Avanzadas**
- 🏛️ **Clases**: Constructor functions → ES6 Classes
- 🎭 **Destructuring**: Parámetros y asignaciones
- ⚡ **Spread/Rest**: Inmutabilidad y parámetros
- 📦 **Módulos**: Import/Export

### ✅ **Código Base**
- 🔄 **Métodos de arrays**: `for` loops → `map`, `filter`
- 🧹 **Código limpio**: Eliminación de patrones anti-ES6

---

## 📋 **Código Base (ES5 Legacy)**

```javascript
// Archivo: task-manager-legacy.js
var TaskManager = function() {
    this.tasks = [];
    this.filter = 'all';
    this.idCounter = 1;
    this.subscribers = [];
};

TaskManager.prototype.addTask = function(text) {
    var task = {
        id: this.idCounter++,
        text: text,
        completed: false,
        createdAt: new Date(),
        priority: 'normal'
    };
    this.tasks.push(task);
    this.notifySubscribers('taskAdded', task);
    this.render();
};

TaskManager.prototype.removeTask = function(id) {
    for (var i = 0; i < this.tasks.length; i++) {
        if (this.tasks[i].id === id) {
            var removedTask = this.tasks.splice(i, 1)[0];
            this.notifySubscribers('taskRemoved', removedTask);
            break;
        }
    }
    this.render();
};

TaskManager.prototype.toggleTask = function(id) {
    for (var i = 0; i < this.tasks.length; i++) {
        if (this.tasks[i].id === id) {
            this.tasks[i].completed = !this.tasks[i].completed;
            this.notifySubscribers('taskToggled', this.tasks[i]);
            break;
        }
    }
    this.render();
};

TaskManager.prototype.getFilteredTasks = function() {
    var filtered = [];
    for (var i = 0; i < this.tasks.length; i++) {
        var task = this.tasks[i];
        if (this.filter === 'all') {
            filtered.push(task);
        } else if (this.filter === 'completed' && task.completed) {
            filtered.push(task);
        } else if (this.filter === 'pending' && !task.completed) {
            filtered.push(task);
        }
    }
    return filtered;
};

TaskManager.prototype.setFilter = function(filter) {
    this.filter = filter;
    this.render();
};

TaskManager.prototype.subscribe = function(callback) {
    this.subscribers.push(callback);
};

TaskManager.prototype.notifySubscribers = function(event, data) {
    for (var i = 0; i < this.subscribers.length; i++) {
        this.subscribers[i](event, data);
    }
};

TaskManager.prototype.render = function() {
    var container = document.getElementById('task-container');
    if (!container) return;
    
    container.innerHTML = '';
    var tasks = this.getFilteredTasks();
    
    for (var i = 0; i < tasks.length; i++) {
        var task = tasks[i];
        var taskElement = document.createElement('div');
        taskElement.className = 'task-item';
        taskElement.innerHTML = '<span>' + task.text + '</span>';
        container.appendChild(taskElement);
    }
};
```

## 🎯 **Resultado Esperado (ES6+ Moderno)**

```javascript
// Archivo: TaskManager.js
class TaskManager {
    constructor() {
        this.tasks = [];
        this.filter = 'all';
        this.idCounter = 1;
        this.subscribers = [];
    }
    
    addTask = (text, priority = 'normal') => {
        const task = {
            id: this.idCounter++,
            text,
            completed: false,
            createdAt: new Date(),
            priority
        };
        
        this.tasks = [...this.tasks, task];
        this.notifySubscribers('taskAdded', task);
        this.render();
    }
    
    removeTask = (id) => {
        const taskToRemove = this.tasks.find(task => task.id === id);
        this.tasks = this.tasks.filter(task => task.id !== id);
        
        if (taskToRemove) {
            this.notifySubscribers('taskRemoved', taskToRemove);
        }
        
        this.render();
    }
    
    toggleTask = (id) => {
        this.tasks = this.tasks.map(task => {
            if (task.id === id) {
                const toggledTask = { ...task, completed: !task.completed };
                this.notifySubscribers('taskToggled', toggledTask);
                return toggledTask;
            }
            return task;
        });
        
        this.render();
    }
    
    getFilteredTasks = () => {
        const { tasks, filter } = this;
        
        const filterMap = {
            completed: ({ completed }) => completed,
            pending: ({ completed }) => !completed,
            all: () => true
        };
        
        return tasks.filter(filterMap[filter] || filterMap.all);
    }
    
    setFilter = (filter) => {
        this.filter = filter;
        this.render();
    }
    
    subscribe = (callback) => {
        this.subscribers = [...this.subscribers, callback];
    }
    
    notifySubscribers = (event, data) => {
        this.subscribers.forEach(callback => callback(event, data));
    }
    
    render = () => {
        const container = document.getElementById('task-container');
        if (!container) return;
        
        const tasks = this.getFilteredTasks();
        
        container.innerHTML = tasks
            .map(({ id, text, completed, priority }) => `
                <div class="task-item ${completed ? 'completed' : ''} priority-${priority}">
                    <span>${text}</span>
                    <button onclick="taskManager.toggleTask(${id})">
                        ${completed ? '✓' : '○'}
                    </button>
                    <button onclick="taskManager.removeTask(${id})">🗑️</button>
                </div>
            `)
            .join('');
    }
    
    // Métodos adicionales ES6+
    getTaskStats = () => {
        const { tasks } = this;
        const completed = tasks.filter(({ completed }) => completed).length;
        const pending = tasks.length - completed;
        
        return { total: tasks.length, completed, pending };
    }
    
    exportTasks = () => JSON.stringify(this.tasks, null, 2);
    
    importTasks = (jsonData) => {
        try {
            const importedTasks = JSON.parse(jsonData);
            this.tasks = [...this.tasks, ...importedTasks];
            this.render();
        } catch (error) {
            console.error('Error importing tasks:', error);
        }
    }
}

export default TaskManager;
```

## 🔄 **Pasos de Transformación**

### **1. Variables y Declaraciones**
```javascript
// ES5 ❌
var TaskManager = function() {
    var tasks = [];
    var filter = 'all';
};

// ES6+ ✅
class TaskManager {
    constructor() {
        const tasks = [];
        let filter = 'all';
    }
}
```

### **2. Métodos y Arrow Functions**
```javascript
// ES5 ❌
TaskManager.prototype.addTask = function(text) {
    var self = this;
    setTimeout(function() {
        self.render();
    }, 100);
};

// ES6+ ✅
addTask = (text) => {
    setTimeout(() => {
        this.render();
    }, 100);
}
```

### **3. Destructuring y Spread**
```javascript
// ES5 ❌
TaskManager.prototype.updateTask = function(id, updates) {
    for (var i = 0; i < this.tasks.length; i++) {
        if (this.tasks[i].id === id) {
            this.tasks[i].text = updates.text || this.tasks[i].text;
            this.tasks[i].priority = updates.priority || this.tasks[i].priority;
        }
    }
};

// ES6+ ✅
updateTask = (id, updates) => {
    this.tasks = this.tasks.map(task => 
        task.id === id ? { ...task, ...updates } : task
    );
}
```

---

## 🧪 **Casos de Prueba Detallados**

```javascript
// 1. Verificar funcionalidad básica
const taskManager = new TaskManager();

// Agregar tareas
taskManager.addTask("Aprender ES6+", "high");
taskManager.addTask("Practicar arrow functions", "normal");
taskManager.addTask("Implementar destructuring", "low");

console.log(taskManager.getTaskStats());
// Esperado: { total: 3, completed: 0, pending: 3 }

// 2. Probar filtros
taskManager.toggleTask(1);
taskManager.setFilter('completed');
console.log(taskManager.getFilteredTasks().length); // Esperado: 1

// 3. Verificar eventos
taskManager.subscribe((event, data) => {
    console.log(`Evento: ${event}`, data);
});

taskManager.addTask("Nueva tarea"); // Debe disparar evento 'taskAdded'

// 4. Probar exportación/importación
const exportedData = taskManager.exportTasks();
const newManager = new TaskManager();
newManager.importTasks(exportedData);
```

## 🔧 **Características ES6+ Implementadas**

### **📦 Módulos ES6**
```javascript
// main.js
import TaskManager from './TaskManager.js';
import { validateTask, formatDate } from './utils.js';

const app = new TaskManager();
```

### **🎭 Destructuring Patterns**
```javascript
// Parámetros
const updateTask = ({ id, text, priority = 'normal' }) => {
    // lógica aquí
};

// Arrays
const [firstTask, ...restTasks] = tasks;

// Objetos anidados
const { task: { id, text }, metadata: { createdAt } } = response;
```

### **⚡ Spread y Rest Operators**
```javascript
// Inmutabilidad
const newTasks = [...existingTasks, newTask];

// Parámetros rest
const addMultipleTasks = (...taskTexts) => {
    taskTexts.forEach(text => this.addTask(text));
};

// Clonación profunda
const clonedTask = { ...task, metadata: { ...task.metadata } };
```

### **🔄 Array Methods Modernos**
```javascript
// Transformación de datos
const taskSummary = tasks
    .filter(({ completed }) => !completed)
    .map(({ text, priority }) => ({ text, priority }))
    .reduce((acc, task) => {
        acc[task.priority] = acc[task.priority] || [];
        acc[task.priority].push(task.text);
        return acc;
    }, {});

// Búsqueda avanzada
const findTaskByText = (searchText) => 
    tasks.find(({ text }) => 
        text.toLowerCase().includes(searchText.toLowerCase())
    );
```

## 🎨 **Mejoras de Sintaxis ES6+**

### **Template Literals**
```javascript
// ES5 ❌
var message = 'Tarea "' + task.text + '" creada el ' + task.createdAt.toDateString();

// ES6+ ✅
const message = `Tarea "${task.text}" creada el ${task.createdAt.toDateString()}`;
```

### **Object Shorthand**
```javascript
// ES5 ❌
var task = {
    id: id,
    text: text,
    completed: completed
};

// ES6+ ✅
const task = { id, text, completed };
```

### **Computed Property Names**
```javascript
// ES6+ ✅
const filterType = 'completed';
const filters = {
    [filterType]: tasks => tasks.filter(t => t.completed),
    [`not${filterType.charAt(0).toUpperCase() + filterType.slice(1)}`]: 
        tasks => tasks.filter(t => !t.completed)
};
```

## 🛡️ **Validaciones y Error Handling**

```javascript
class TaskManager {
    addTask = (text, priority = 'normal') => {
        // Validación de entrada
        if (!text || typeof text !== 'string') {
            throw new Error('El texto de la tarea es requerido y debe ser string');
        }
        
        if (!['low', 'normal', 'high'].includes(priority)) {
            throw new Error('Prioridad debe ser: low, normal o high');
        }
        
        try {
            const task = {
                id: this.idCounter++,
                text: text.trim(),
                completed: false,
                createdAt: new Date(),
                priority
            };
            
            this.tasks = [...this.tasks, task];
            this.notifySubscribers('taskAdded', task);
            this.render();
            
            return task;
        } catch (error) {
            console.error('Error agregando tarea:', error);
            throw error;
        }
    }
    
    // Validación de estado
    validateState = () => {
        const errors = [];
        
        if (!Array.isArray(this.tasks)) {
            errors.push('Tasks debe ser un array');
        }
        
        if (typeof this.idCounter !== 'number') {
            errors.push('idCounter debe ser un número');
        }
        
        return errors.length > 0 ? errors : null;
    }
}
```

## 🚀 **Funcionalidades Avanzadas**

### **Async/Await para Persistencia**
```javascript
class TaskManager {
    // Guardar en localStorage
    saveToStorage = async () => {
        try {
            const data = JSON.stringify(this.tasks);
            localStorage.setItem('tasks', data);
            return { success: true };
        } catch (error) {
            return { success: false, error: error.message };
        }
    }
    
    // Cargar desde localStorage
    loadFromStorage = async () => {
        try {
            const data = localStorage.getItem('tasks');
            if (data) {
                this.tasks = JSON.parse(data);
                this.render();
            }
            return { success: true };
        } catch (error) {
            console.error('Error cargando tareas:', error);
            return { success: false, error: error.message };
        }
    }
}
```

### **Proxy para Observar Cambios**
```javascript
class ReactiveTaskManager extends TaskManager {
    constructor() {
        super();
        
        // Proxy para reactividad
        return new Proxy(this, {
            set(target, property, value) {
                const oldValue = target[property];
                target[property] = value;
                
                if (property === 'tasks' && oldValue !== value) {
                    target.render();
                }
                
                return true;
            }
        });
    }
}
```

---

## ✅ **Criterios de Evaluación**

- [ ] **Variables** correctamente declaradas
- [ ] **Funciones** modernizadas apropiadamente  
- [ ] **Clases** implementadas correctamente
- [ ] **Métodos de arrays** utilizados
- [ ] **Sintaxis ES6+** aplicada consistentemente

---

[📁 **Siguiente Proyecto**](./02-mini-api-fetcher.md) | [🏠 **Volver a Ejercicios**](../ejercicios-practicos/README-EJERCICIOS.md) | [📚 **Navegación**](../../../NAVEGACION-DOCUMENTOS.md)
