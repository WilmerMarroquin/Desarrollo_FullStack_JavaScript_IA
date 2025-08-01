[🏠 **Volver al Índice de Navegación**](../../../../NAVEGACION-DOCUMENTOS.md)

---

# 🌐 **PROYECTO GUIADO 2: Mini API Client**

## Cliente de API con JavaScript Moderno

> **🚀 "Construye un cliente de API profesional usando async/await, destructuring y módulos ES6. Conecta tu app con el mundo."**

---

## 📋 **Descripción del Proyecto**

### 🎯 **Objetivo Principal**
Crear un cliente de API completo que consuma datos de servicios externos usando todas las características modernas de JavaScript ES6+.

### 🎨 **Lo que Aprenderás**
- **🔄 Async/Await** para operaciones asíncronas
- **📡 Fetch API** moderna
- **🎭 Destructuring** en respuestas API
- **� Módulos** para organizar cliente
- **⚡ Arrow functions** en contextos async
- **🛡️ Error handling** profesional

### ⏱️ **Tiempo Estimado**
**60-90 minutos** (construir desde cero)

---

## 🏗️ **Código Base del Proyecto**

### 📁 **Estructura del Cliente API**

```javascript
// === api-client.js ===
class APIClient {
    constructor(baseURL) {
        this.baseURL = baseURL;
        this.headers = {
            'Content-Type': 'application/json'
        };
    }
    
    // GET request con async/await
    async get(endpoint) {
        try {
            const response = await fetch(`${this.baseURL}${endpoint}`, {
                method: 'GET',
                headers: this.headers
            });
            
            if (!response.ok) {
                throw new Error(`HTTP error! status: ${response.status}`);
            }
            
            return await response.json();
        } catch (error) {
            console.error('GET Error:', error);
            throw error;
        }
    }
    
    // POST request con datos
    async post(endpoint, data) {
        try {
            const response = await fetch(`${this.baseURL}${endpoint}`, {
                method: 'POST',
                headers: this.headers,
                body: JSON.stringify(data)
            });
            
            if (!response.ok) {
                throw new Error(`HTTP error! status: ${response.status}`);
            }
            
            return await response.json();
        } catch (error) {
            console.error('POST Error:', error);
            throw error;
        }
    }
}
```

### 🎯 **Implementación de la App**

```javascript
// === app.js ===
import { APIClient } from './api-client.js';

class UserApp {
    constructor() {
        this.api = new APIClient('https://jsonplaceholder.typicode.com');
        this.users = [];
        this.init();
    }
    
    init = () => {
        this.setupEventListeners();
        this.loadUsers();
    }
    
    setupEventListeners = () => {
        document.getElementById('load-users').addEventListener('click', this.loadUsers);
        document.getElementById('add-user').addEventListener('click', this.addUser);
    }
    
    loadUsers = async () => {
        try {
            const users = await this.api.get('/users');
            this.users = users;
            this.renderUsers();
        } catch (error) {
            this.showError('Error loading users');
        }
    }
    
    addUser = async () => {
        const { name, email } = this.getUserInput();
        
        if (!name || !email) {
            this.showError('Name and email are required');
            return;
        }
        
        try {
            const newUser = await this.api.post('/users', { name, email });
            this.users = [...this.users, newUser];
            this.renderUsers();
            this.clearForm();
        } catch (error) {
            this.showError('Error adding user');
        }
    }
    
    getUserInput = () => {
        const name = document.getElementById('name').value;
        const email = document.getElementById('email').value;
        return { name, email };
    }
    
    renderUsers = () => {
        const container = document.getElementById('users-container');
        
        container.innerHTML = this.users.map(({ id, name, email }) => `
            <div class="user-card">
                <h3>${name}</h3>
                <p>${email}</p>
                <span>ID: ${id}</span>
            </div>
        `).join('');
    }
    
    showError = (message) => {
        const errorDiv = document.getElementById('error-message');
        errorDiv.textContent = message;
        errorDiv.style.display = 'block';
        
        setTimeout(() => {
            errorDiv.style.display = 'none';
        }, 3000);
    }
    
    clearForm = () => {
        document.getElementById('name').value = '';
        document.getElementById('email').value = '';
    }
}

// Inicializar la app
new UserApp();
```

---

## 🎯 **Pasos de Construcción**

### **📍 PASO 1: Setup del Cliente API (20 min)**

#### 🎯 Tareas:
1. **Clase base**: Constructor con baseURL
2. **Headers config**: Content-Type y auth
3. **Método GET**: Con async/await
4. **Error handling**: Try/catch profesional

### **📍 PASO 2: Métodos HTTP (20 min)**

#### 🎯 Tareas:
1. **POST method**: Envío de datos
2. **PUT method**: Actualización
3. **DELETE method**: Eliminación
4. **Response parsing**: JSON automático

### **📍 PASO 3: UI Integration (25 min)**

#### 🎯 Tareas:
1. **Event listeners**: Clicks y forms
2. **Async handlers**: Para UI events
3. **Destructuring**: En form data
4. **Template literals**: Para render

### **📍 PASO 4: Error Handling UX (15 min)**

#### 🎯 Tareas:
1. **Loading states**: Indicadores visuales
2. **Error messages**: User-friendly
3. **Retry logic**: Para fallos de red

---

## 🧪 **Características Modernas Usadas**

### ✅ **ES6+ Features**

- [ ] **Classes**: Para organización
- [ ] **Async/Await**: Operaciones asíncronas
- [ ] **Arrow Functions**: Event handlers
- [ ] **Destructuring**: Form data y responses
- [ ] **Template Literals**: String interpolation
- [ ] **Spread Operator**: Array updates
- [ ] **Modules**: Import/Export
- [ ] **Default Parameters**: Configuración flexible

---

**🌐 ¿Listo para conectar con APIs?**

[📁 **Proyecto 1: Refactor App**](./01-refactor-app-moderna.md) | [🏠 **Volver a Ejercicios**](../ejercicios-practicos/README-EJERCICIOS.md) | [📚 **Navegación**](../../../../NAVEGACION-DOCUMENTOS.md)
