[🏠 **Volver al Índice de Navegación**](../../../NAVEGACION-DOCUMENTOS.md)

---

# 📇 Libreta de Contactos - Proyecto de Estructuras de Datos 👥 Libreta de Contactos - Proyecto de Estructuras de Datos

## 📝 **Descripción del Proyecto**
Crear una libreta de contactos digital que permita almacenar, buscar, editar y organizar información de personas utilizando objetos complejos y métodos de búsqueda avanzados.

---

## 🎯 **Objetivos de Aprendizaje**
- Dominar **objetos con múltiples propiedades**
- Practicar **búsqueda y filtrado** en arrays de objetos
- Implementar **validación de datos** complejos
- Usar **métodos find, filter, some** para consultas
- Trabajar con **propiedades anidadas** y **destructuring**

---

## 🔧 **Funcionalidades Requeridas**

### ✅ **Gestión de Contactos**
- ➕ **Agregar contacto** con nombre, teléfono, email, dirección
- ✏️ **Editar información** de contacto existente
- ❌ **Eliminar contacto** por nombre o ID
- 📋 **Mostrar todos los contactos** organizadamente

### ✅ **Búsqueda y Filtrado**
- 🔍 **Buscar por nombre** (coincidencia parcial)
- 📞 **Buscar por teléfono** (número completo o parcial)
- 📧 **Buscar por email** o dominio
- 🏠 **Filtrar por ciudad** o código postal

### ✅ **Funcionalidades Avanzadas**
- 📊 **Estadísticas** (total contactos, ciudades, dominios email)
- 🔤 **Ordenar alfabéticamente** por nombre o apellido
- 📋 **Exportar contactos** a formato texto
- ✅ **Validar formato** de email y teléfono

---

## 📋 **Estructura Esperada**

```javascript
// Array principal para almacenar contactos
let libretaContactos = [];

// Funciones básicas de gestión
function agregarContacto(datos) { /* tu código */ }
function editarContacto(id, nuevosDatos) { /* tu código */ }
function eliminarContacto(id) { /* tu código */ }
function mostrarContactos() { /* tu código */ }

// Funciones de búsqueda
function buscarPorNombre(termino) { /* tu código */ }
function buscarPorTelefono(numero) { /* tu código */ }
function buscarPorEmail(email) { /* tu código */ }
function filtrarPorCiudad(ciudad) { /* tu código */ }

// Funciones de validación
function validarEmail(email) { /* tu código */ }
function validarTelefono(telefono) { /* tu código */ }
function validarContacto(datos) { /* tu código */ }

// Funciones de utilidad
function ordenarPorNombre() { /* tu código */ }
function obtenerEstadisticas() { /* tu código */ }
function exportarContactos() { /* tu código */ }

// Función principal del sistema
function libretaDigital() {
    // Mostrar menú de opciones
    // Procesar elección del usuario
    // Ejecutar función correspondiente
}

// Ejecutar la libreta
libretaDigital();
```

---

## 🧪 **Casos de Prueba**

Asegúrate de que tu libreta maneje estos casos:

```javascript
// Agregar contactos válidos
agregarContacto({
    nombre: "Ana García",
    telefono: "555-0123", 
    email: "ana@email.com",
    direccion: {ciudad: "Madrid", cp: "28001"}
}) → Contacto agregado con ID único

// Búsquedas efectivas
buscarPorNombre("Ana") → Encuentra "Ana García"
buscarPorNombre("gar") → Encuentra "Ana García" (parcial)
buscarPorTelefono("555") → Encuentra contactos con ese prefijo
buscarPorEmail("email.com") → Encuentra contactos de ese dominio

// Validaciones
validarEmail("ana@email.com") → true
validarEmail("email-inválido") → false
validarTelefono("555-0123") → true
validarTelefono("123") → false

// Filtrado y ordenamiento
filtrarPorCiudad("Madrid") → Solo contactos de Madrid
ordenarPorNombre() → Lista alfabética por nombre
obtenerEstadisticas() → {total: 5, ciudades: 3, dominios: 2}

// Casos especiales
agregarContacto({nombre: ""}) → "Error: Nombre requerido"
editarContacto(999, {}) → "Error: Contacto no encontrado"
eliminarContacto("ID-inexistente") → "Error: ID inválido"
```

---

## 💾 **Estructura de Datos Sugerida**

```javascript
// Cada contacto será un objeto con esta estructura:
const contactoEjemplo = {
    id: "CONT_001",           // ID único generado automáticamente
    nombre: "Ana García",     // Nombre completo
    telefono: "555-0123",     // Número de teléfono
    email: "ana@email.com",   // Correo electrónico
    direccion: {              // Objeto anidado para dirección
        calle: "Calle Mayor 123",
        ciudad: "Madrid",
        codigoPostal: "28001",
        pais: "España"
    },
    fechaCreacion: new Date(), // Cuándo se agregó
    notas: "Compañera de trabajo" // Información adicional
};

// El array principal contendrá objetos como este:
let libretaContactos = [contactoEjemplo];
```

---

## ⏱️ **Tiempo Estimado**
**2-3 horas** (dependiendo de tu nivel)

## 🎓 **Nivel de Dificultad**
🟡 **INTERMEDIO** - Requiere comodidad con objetos y arrays

---

## 💡 **Pistas para Empezar**

1. **Diseña la estructura**: Define primero cómo será tu objeto contacto
2. **Genera IDs únicos**: Usa `Date.now()` o un contador para IDs únicos
3. **Valida paso a paso**: Implementa validaciones simples primero
4. **Usa destructuring**: Para extraer propiedades de objetos fácilmente
5. **Piensa en la experiencia**: ¿Cómo mostrarías la información claramente?
6. **Maneja objetos anidados**: Practica acceso a `contacto.direccion.ciudad`

---

## 🎯 **Conceptos Clave que Practicarás**

- **Array.find()** - Encontrar un elemento específico
- **Array.filter()** - Filtrar múltiples elementos
- **Array.some()** - Verificar si algún elemento cumple condición
- **Array.sort()** - Ordenar arrays de objetos
- **Object.keys()** - Obtener propiedades de objeto
- **Destructuring** - Extraer propiedades elegantemente
- **Objetos anidados** - Propiedades dentro de propiedades
- **Validación de datos** - Verificar formatos y tipos

---

## 🔍 **Funciones de Búsqueda Sugeridas**

```javascript
// Ejemplos de implementaciones avanzadas que puedes intentar:

// Búsqueda inteligente (nombre, email, teléfono a la vez)
function busquedaGlobal(termino) {
    return libretaContactos.filter(contacto => 
        contacto.nombre.toLowerCase().includes(termino.toLowerCase()) ||
        contacto.email.toLowerCase().includes(termino.toLowerCase()) ||
        contacto.telefono.includes(termino)
    );
}

// Obtener dominios de email únicos
function obtenerDominiosEmail() {
    return [...new Set(
        libretaContactos.map(c => c.email.split('@')[1])
    )];
}
```

---

**🚀 ¡Cuando termines, tendrás una libreta digital completa y habrás dominado la manipulación avanzada de objetos y arrays!**

---

[🔙 **Volver al Libro Principal**](../ESTRUCTURAS-DATOS-LIBRO.md) | [🏠 **Índice General**](../../../README.md) | [📚 **Navegación**](../../../NAVEGACION-DOCUMENTOS.md) | [📝 **Ver Cheatsheet**](../CHEATSHEET-VISUAL.md)
