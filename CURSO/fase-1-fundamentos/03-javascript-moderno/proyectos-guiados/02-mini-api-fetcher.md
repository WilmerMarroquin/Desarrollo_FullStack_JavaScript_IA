[🏠 **Volver al Índice de Navegación**](../../../NAVEGACION-DOCUMENTOS.md)

---

# 🌐 Mini API Client - Proyecto ES6+

## 📝 **Descripción del Proyecto**
Crear un cliente de API usando async/await, clases ES6 y todas las características modernas de JavaScript para consumir datos externos.

---

## 🎯 **Objetivos de Aprendizaje**
- Aplicar **async/await** para operaciones asíncronas
- Practicar **clases ES6** para organización
- Implementar **destructuring** en respuestas API
- Usar **arrow functions** en contextos async
- Manejar **errores** con try/catch moderno

---

## 🔧 **Funcionalidades Requeridas**

### ✅ **Cliente API Básico**
- 🌐 **GET request** con async/await
- 📤 **POST request** para envío de datos
- 🛡️ **Error handling** elegante
- 🎭 **Destructuring** de respuestas JSON

### ✅ **Interfaz de Usuario**
- 📋 **Mostrar datos** obtenidos de API
- ➕ **Agregar elementos** mediante formulario
- 🔄 **Estados de carga** (loading, error, success)
- ⚡ **Event listeners** con arrow functions

### ✅ **Características ES6+**
- 🏛️ **Clases** para organizar el cliente
- 📦 **Módulos** para separar responsabilidades
- 🎨 **Template literals** para HTML dinámico
- ⚡ **Spread operator** para manejo de datos

---

## 📋 **Estructura Esperada**

```javascript
// Cliente API con ES6+
class APIClient {
    constructor(baseURL) {
        /* tu código */
    }
    
    async get(endpoint) {
        /* tu código con async/await */
    }
    
    async post(endpoint, data) {
        /* tu código con async/await */
    }
}

// Uso del cliente
const client = new APIClient('https://api.ejemplo.com');
const data = await client.get('/users');
```

---

## 🧪 **API Sugerida**

```javascript
// Usar JSONPlaceholder para pruebas
const API_BASE = 'https://jsonplaceholder.typicode.com';

// Endpoints disponibles:
// GET /users - Lista de usuarios
// GET /posts - Lista de posts  
// POST /users - Crear usuario
// POST /posts - Crear post
```

---

## ✅ **Criterios de Evaluación**

- [ ] **Async/await** implementado correctamente
- [ ] **Clases ES6** utilizadas para organización
- [ ] **Error handling** con try/catch
- [ ] **Destructuring** aplicado en respuestas
- [ ] **Arrow functions** en callbacks
- [ ] **Template literals** para strings dinámicos

---

[📁 **Proyecto Anterior**](./01-refactor-app-moderna.md) | [📁 **Siguiente Proyecto**](./03-generador-componentes.md) | [🏠 **Volver a Ejercicios**](../ejercicios-practicos/README-EJERCICIOS.md)
