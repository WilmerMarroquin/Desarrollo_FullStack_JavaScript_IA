[🏠 **Volver al Índice de Navegación**](../../../NAVEGACION-DOCUMENTOS.md)

---

# 🎨 Generador de Componentes - Proyecto ES6+

## 📝 **Descripción del Proyecto**
Crear un generador de componentes web reutilizables usando clases ES6, template literals y módulos para construir elementos HTML dinámicos.

---

## 🎯 **Objetivos de Aprendizaje**
- Aplicar **clases ES6** para crear componentes
- Practicar **template literals** avanzados
- Implementar **getters y setters** modernos
- Usar **spread operator** para propiedades
- Organizar código con **módulos ES6**

---

## 🔧 **Funcionalidades Requeridas**

### ✅ **Componentes Básicos**
- 🧱 **Card Component** con propiedades dinámicas
- 📝 **Form Component** con validación
- 📋 **List Component** con elementos iterables
- 🎛️ **Button Component** con eventos

### ✅ **Características Avanzadas**
- 🎨 **Styling dinámico** con CSS-in-JS
- 🔄 **State management** básico
- 📡 **Event handling** con arrow functions
- 🧩 **Composición** de componentes

### ✅ **Técnicas ES6+**
- 🏛️ **Classes** para estructura
- 📝 **Template literals** para HTML
- 🎭 **Destructuring** en parámetros
- ⚡ **Default parameters** para configuración

---

## 📋 **Estructura Esperada**

```javascript
// Componente base
class Component {
    constructor(props = {}) {
        /* tu código */
    }
    
    render() {
        /* tu código con template literals */
    }
    
    mount(selector) {
        /* tu código */
    }
}

// Componente específico
class Card extends Component {
    /* tu implementación */
}
```

---

## 🧪 **Componentes a Crear**

```javascript
// Ejemplos de uso esperado
const card = new Card({
    title: 'Mi Tarjeta',
    content: 'Contenido dinámico',
    image: 'imagen.jpg'
});

const form = new Form({
    fields: ['name', 'email'],
    validation: true
});
```

---

## ✅ **Criterios de Evaluación**

- [ ] **Clases ES6** implementadas correctamente
- [ ] **Template literals** usados para HTML
- [ ] **Destructuring** aplicado en parámetros
- [ ] **Arrow functions** en event handlers
- [ ] **Módulos** para organización
- [ ] **Reutilización** de componentes funcional

---

[📁 **Proyecto Anterior**](./02-mini-api-fetcher.md) | [📁 **Siguiente Proyecto**](./04-todo-app-moderna.md) | [🏠 **Volver a Ejercicios**](../ejercicios-practicos/README-EJERCICIOS.md)
