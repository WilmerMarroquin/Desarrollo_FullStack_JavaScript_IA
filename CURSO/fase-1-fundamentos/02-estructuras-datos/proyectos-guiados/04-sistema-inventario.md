[🏠 **Volver al Índice de Navegación**](../../../../NAVEGACION-DOCUMENTOS.md)

---

# 📦 Sistema de Inventario - Proyecto de Estructuras de Datos 🎮 Sistema de Inventario - Proyecto de Estructuras de Datos

## 📝 **Descripción del Proyecto**
Crear un sistema de gestión de inventario para una tienda que maneje productos, categorías, proveedores y stock utilizando Map, Set y estructuras de datos avanzadas para optimizar búsquedas y relaciones.

---

## 🎯 **Objetivos de Aprendizaje**
- Dominar **Map y Set** para relaciones complejas
- Practicar **gestión de referencias** entre entidades
- Implementar **búsquedas optimizadas** con claves únicas
- Usar **WeakMap y WeakSet** para metadatos
- Trabajar con **estructuras relacionales** en JavaScript

---

## 🔧 **Funcionalidades Requeridas**

### ✅ **Gestión de Productos**
- ➕ **Agregar producto** con código, nombre, precio, stock
- ✏️ **Actualizar información** y cantidades
- ❌ **Eliminar producto** con validaciones
- 🔍 **Buscar productos** por código, nombre o categoría

### ✅ **Gestión de Categorías**
- 📁 **Crear categorías** con jerarquías
- 🏷️ **Asignar productos** a categorías múltiples
- 📊 **Estadísticas por categoría** (productos, valor total)
- 🔗 **Gestionar relaciones** padre-hijo entre categorías

### ✅ **Control de Stock y Movimientos**
- 📦 **Registrar entradas** de mercancía
- 🛒 **Procesar salidas** y ventas
- ⚠️ **Alertas de stock mínimo** automáticas
- 📈 **Historial de movimientos** por producto

### ✅ **Gestión de Proveedores**
- 🏢 **Registrar proveedores** con información completa
- 🔗 **Asociar productos** con proveedores
- 💰 **Calcular costos** por proveedor
- 📋 **Generar órdenes** de compra automáticas

---

## 📋 **Estructura Esperada**

```javascript
// Maps principales para datos relacionales
const productos = new Map();        // código → producto
const categorias = new Map();       // id → categoría
const proveedores = new Map();      // id → proveedor
const movimientos = new Map();      // id → movimiento

// Sets para relaciones muchos-a-muchos
const productosCategorias = new Map(); // producto → Set(categorías)
const categoriasProductos = new Map(); // categoría → Set(productos)
const proveedorProductos = new Map();  // proveedor → Set(productos)

// WeakMaps para metadatos
const metadatosProductos = new WeakMap();
const alertasStock = new WeakMap();

// Funciones de gestión de productos
function agregarProducto(codigo, datos) { /* tu código */ }
function actualizarProducto(codigo, cambios) { /* tu código */ }
function eliminarProducto(codigo) { /* tu código */ }
function buscarProducto(termino) { /* tu código */ }

// Funciones de categorías
function crearCategoria(id, nombre, padre = null) { /* tu código */ }
function asignarCategoria(codigoProducto, idCategoria) { /* tu código */ }
function obtenerProductosPorCategoria(idCategoria) { /* tu código */ }
function calcularValorCategoria(idCategoria) { /* tu código */ }

// Funciones de stock
function registrarEntrada(codigo, cantidad, proveedor) { /* tu código */ }
function registrarSalida(codigo, cantidad, motivo) { /* tu código */ }
function verificarStockMinimo() { /* tu código */ }
function obtenerHistorialMovimientos(codigo) { /* tu código */ }

// Funciones de proveedores
function registrarProveedor(id, datos) { /* tu código */ }
function asociarProveedor(codigoProducto, idProveedor) { /* tu código */ }
function calcularCostosProveedor(idProveedor) { /* tu código */ }
function generarOrdenCompra(idProveedor) { /* tu código */ }

// Función principal del sistema
function sistemaInventario() {
    // Inicializar datos de ejemplo
    // Mostrar dashboard principal
    // Procesar operaciones del usuario
}

// Ejecutar sistema
sistemaInventario();
```

---

## 🧪 **Casos de Prueba**

Asegúrate de que tu sistema maneje estos casos:

```javascript
// Gestión de productos
agregarProducto("PROD001", {
    nombre: "Laptop Gaming",
    precio: 1299.99,
    stock: 15,
    stockMinimo: 5
}) → Producto agregado exitosamente

buscarProducto("gaming") → Encuentra "Laptop Gaming"
actualizarProducto("PROD001", {precio: 1199.99}) → Precio actualizado
productos.get("PROD001").precio → 1199.99

// Gestión de categorías
crearCategoria("CAT001", "Electrónicos") → Categoría creada
crearCategoria("CAT002", "Computadoras", "CAT001") → Subcategoría creada
asignarCategoria("PROD001", "CAT002") → Producto asignado a categoría
obtenerProductosPorCategoria("CAT002") → Set con "PROD001"

// Control de stock
registrarEntrada("PROD001", 10, "PROV001") → Stock: 25, Movimiento registrado
registrarSalida("PROD001", 3, "Venta") → Stock: 22, Movimiento registrado
verificarStockMinimo() → Lista productos con stock bajo mínimo

// Gestión de proveedores
registrarProveedor("PROV001", {
    nombre: "TechSupply Co.",
    contacto: "tech@supply.com"
}) → Proveedor registrado

asociarProveedor("PROD001", "PROV001") → Asociación creada
calcularCostosProveedor("PROV001") → Total de productos de ese proveedor

// Consultas complejas
productos.size → Número total de productos
Array.from(categorias.keys()) → Lista de IDs de categorías
productosCategorias.get("PROD001") → Set de categorías del producto

// Casos especiales
agregarProducto("PROD001", {}) → "Error: Producto ya existe"
eliminarProducto("INEXISTENTE") → "Error: Producto no encontrado"
registrarSalida("PROD001", 100) → "Error: Stock insuficiente"
```

---

## 💾 **Estructura de Datos Sugerida**

```javascript
// Estructura de producto
const productoEjemplo = {
    codigo: "PROD001",
    nombre: "Laptop Gaming",
    descripcion: "Laptop para gaming de alto rendimiento",
    precio: 1299.99,
    costo: 899.99,
    stock: 15,
    stockMinimo: 5,
    unidad: "pieza",
    fechaCreacion: new Date(),
    activo: true
};

// Estructura de categoría
const categoriaEjemplo = {
    id: "CAT001",
    nombre: "Electrónicos",
    descripcion: "Productos electrónicos diversos",
    padre: null,        // ID de categoría padre
    hijos: new Set(),   // IDs de subcategorías
    nivel: 0           // Profundidad en jerarquía
};

// Estructura de proveedor
const proveedorEjemplo = {
    id: "PROV001",
    nombre: "TechSupply Co.",
    contacto: "Juan Pérez",
    email: "tech@supply.com",
    telefono: "555-0123",
    direccion: "Calle Tech 123",
    activo: true
};

// Estructura de movimiento
const movimientoEjemplo = {
    id: "MOV001",
    codigoProducto: "PROD001",
    tipo: "entrada",    // "entrada" o "salida"
    cantidad: 10,
    precio: 899.99,     // Para entradas (costo)
    motivo: "Compra",   // "Compra", "Venta", "Ajuste", "Devolución"
    proveedor: "PROV001",
    fecha: new Date(),
    usuario: "admin"
};
```

---

## ⏱️ **Tiempo Estimado**
**3-4 horas** (dependiendo de tu nivel)

## 🎓 **Nivel de Dificultad**
🔴 **AVANZADO** - Requiere dominio de Map, Set y relaciones complejas

---

## 💡 **Pistas para Empezar**

1. **Entiende Map vs Object**: Map es mejor para claves dinámicas y relaciones
2. **Usa Set para unicidad**: Perfecto para relaciones muchos-a-muchos
3. **Diseña las relaciones**: Planifica cómo conectar productos, categorías y proveedores
4. **Genera IDs únicos**: Usa prefijos y contadores o timestamps
5. **Valida integridad**: Siempre verifica que las referencias existan
6. **Piensa en performance**: Map.get() es O(1), Array.find() es O(n)

---

## 🎯 **Conceptos Clave que Practicarás**

- **Map.set()/get()** - Almacenamiento clave-valor optimizado
- **Set.add()/has()** - Colecciones de valores únicos
- **Map.keys()/values()** - Iteración sobre Maps
- **WeakMap/WeakSet** - Referencias débiles para metadatos
- **Relaciones bidireccionales** - Mantener coherencia entre estructuras
- **Integridad referencial** - Validar que las relaciones sean válidas
- **Índices múltiples** - Diferentes formas de acceder a los mismos datos
- **Performance optimization** - Elegir la estructura correcta para cada caso

---

## 🔍 **Algoritmos Avanzados Sugeridos**

```javascript
// Ejemplos de implementaciones avanzadas que puedes intentar:

// Búsqueda de productos por múltiples criterios
function busquedaAvanzada(filtros) {
    let resultados = new Set(productos.keys());
    
    if (filtros.categoria) {
        const productosCategoria = categoriasProductos.get(filtros.categoria) || new Set();
        resultados = new Set([...resultados].filter(x => productosCategoria.has(x)));
    }
    
    if (filtros.proveedor) {
        const productosProveedor = proveedorProductos.get(filtros.proveedor) || new Set();
        resultados = new Set([...resultados].filter(x => productosProveedor.has(x)));
    }
    
    if (filtros.precioMin || filtros.precioMax) {
        resultados = new Set([...resultados].filter(codigo => {
            const producto = productos.get(codigo);
            return (!filtros.precioMin || producto.precio >= filtros.precioMin) &&
                   (!filtros.precioMax || producto.precio <= filtros.precioMax);
        }));
    }
    
    return Array.from(resultados).map(codigo => productos.get(codigo));
}

// Calcular valor total del inventario
function valorTotalInventario() {
    return Array.from(productos.values())
        .reduce((total, producto) => total + (producto.precio * producto.stock), 0);
}

// Obtener productos de una categoría y todas sus subcategorías
function obtenerProductosJerarquia(idCategoria) {
    const categoria = categorias.get(idCategoria);
    if (!categoria) return new Set();
    
    let todosProductos = new Set(categoriasProductos.get(idCategoria) || []);
    
    // Recursivamente obtener productos de subcategorías
    for (const hijoId of categoria.hijos) {
        const productosHijo = obtenerProductosJerarquia(hijoId);
        productosHijo.forEach(p => todosProductos.add(p));
    }
    
    return todosProductos;
}
```

---

**🚀 ¡Cuando termines, tendrás un sistema de inventario profesional y habrás dominado las estructuras de datos más avanzadas de JavaScript!**

---

[🔙 **Volver al Libro Principal**](../ESTRUCTURAS-DATOS-LIBRO.md) | [🏠 **Índice General**](../../../../README.md) | [📚 **Navegación**](../../../../NAVEGACION-DOCUMENTOS.md) | [📝 **Ver Cheatsheet**](../CHEATSHEET-VISUAL.md)
