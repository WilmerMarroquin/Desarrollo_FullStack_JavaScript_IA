[🏠 **Volver al Índice de Navegación**](../../../NAVEGACION-DOCUMENTOS.md)

---

# 📝 **CHEATSHEET VISUAL - JAVASCRIPT MODERNO (ES6+)**

## La Referencia Rápida Definitiva para Dominar ES6+

> **🎯 "Una imagen vale más que mil palabras, pero un buen ejemplo de código vale más que mil explicaciones. Esta es tu referencia visual para JavaScript moderno."**

---

## 🧭 **NAVEGACIÓN RÁPIDA**

### 📋 **ÍNDICE DEL CHEATSHEET**

| **🎯 SINTAXIS BÁSICA** | **⚡ FUNCIONES** | **📦 ESTRUCTURAS** | **🔄 ASÍNCRONO** |
|:----------------------:|:----------------:|:------------------:|:-----------------:|
| [Variables](#variables-let-const-var) | [Arrow Functions](#arrow-functions) | [Destructuring](#destructuring) | [Promises](#promises) |
| [Template Literals](#template-literals) | [Parámetros](#parámetros-por-defecto) | [Spread/Rest](#spread--rest) | [Async/Await](#asyncawait) |
| [Comparaciones](#comparaciones-es5-vs-es6) | [Scope](#scope-y-hoisting) | [Módulos](#módulos-es6) | [Fetch API](#fetch-api) |

---

## 🎯 **VARIABLES: let, const, var**

### 📊 **Comparación Visual**

```javascript
// ❌ ES5 - var (problemas de scope)
function ejemploVar() {
    if (true) {
        var nombre = 'Ana';
    }
    console.log(nombre); // 'Ana' - accesible fuera del bloque ❌
}

// ✅ ES6 - let y const (block scope)
function ejemploModerno() {
    if (true) {
        let nombre = 'Ana';
        const edad = 25;
    }
    console.log(nombre); // ❌ ReferenceError - no accesible
}
```

### 🔍 **Cuándo Usar Cada Una**

```javascript
// ✅ const - Para valores que NO cambian (preferir siempre)
const API_URL = 'https://api.miapp.com';
const usuarios = []; // El array puede mutar, la referencia no

// ✅ let - Para valores que SÍ cambian
let contador = 0;
let mensaje = '';

// ❌ var - EVITAR en código moderno
// Solo en casos muy específicos de compatibilidad
```

### 📈 **Hoisting Comparativo**

```javascript
// ❌ var - Se "eleva" y se inicializa con undefined
console.log(varVariable); // undefined (no error)
var varVariable = 'Hola';

// ✅ let/const - Se "elevan" pero NO se inicializan (Temporal Dead Zone)
console.log(letVariable); // ❌ ReferenceError
let letVariable = 'Hola';

console.log(constVariable); // ❌ ReferenceError  
const constVariable = 'Hola';
```

---

## ➡️ **ARROW FUNCTIONS**

### 🎯 **Sintaxis Comparativa**

```javascript
// ❌ ES5 - Función tradicional
function sumar(a, b) {
    return a + b;
}

// ✅ ES6 - Arrow function (explícita)
const sumar = (a, b) => {
    return a + b;
};

// ✅ ES6 - Arrow function (implícita)
const sumar = (a, b) => a + b;

// ✅ ES6 - Un parámetro (sin paréntesis)
const doble = x => x * 2;

// ✅ ES6 - Sin parámetros
const saludo = () => 'Hola mundo';
```

### 🎭 **Binding de 'this' - La Diferencia Clave**

```javascript
// ❌ ES5 - 'this' dinámico (problemático)
const objeto = {
    nombre: 'Ana',
    amigos: ['Luis', 'María'],
    
    mostrarAmigos: function() {
        this.amigos.forEach(function(amigo) {
            console.log(this.nombre + ' conoce a ' + amigo);
            // ❌ 'this' es undefined o window
        });
    }
};

// ✅ ES6 - Arrow function hereda 'this' léxico
const objeto = {
    nombre: 'Ana',
    amigos: ['Luis', 'María'],
    
    mostrarAmigos() {
        this.amigos.forEach(amigo => {
            console.log(`${this.nombre} conoce a ${amigo}`);
            // ✅ 'this' se refiere al objeto
        });
    }
};
```

### ⚠️ **Cuándo NO Usar Arrow Functions**

```javascript
// ❌ Como métodos de objeto (this no funciona como esperas)
const persona = {
    nombre: 'Ana',
    saludar: () => {
        console.log(`Hola, soy ${this.nombre}`); // ❌ this es undefined
    }
};

// ✅ Usar función tradicional para métodos
const persona = {
    nombre: 'Ana',
    saludar() {
        console.log(`Hola, soy ${this.nombre}`); // ✅ this es el objeto
    }
};

// ❌ Como constructores
const Persona = (nombre) => {
    this.nombre = nombre; // ❌ Error: Arrow functions no tienen 'this'
};

// ✅ Usar función tradicional o class
function Persona(nombre) {
    this.nombre = nombre; // ✅ Funciona
}
```

---

## 🎨 **TEMPLATE LITERALS**

### 📝 **Interpolación de Strings**

```javascript
// ❌ ES5 - Concatenación engorrosa
const nombre = 'Ana';
const edad = 25;
const mensaje = 'Hola, soy ' + nombre + ' y tengo ' + edad + ' años.';

// ✅ ES6 - Template literals elegantes
const mensaje = `Hola, soy ${nombre} y tengo ${edad} años.`;
```

### 🔢 **Expresiones y Cálculos**

```javascript
const precio = 99.99;
const cantidad = 3;

// ✅ Expresiones dentro de templates
const factura = `
    Producto: Laptop
    Precio unitario: $${precio}
    Cantidad: ${cantidad}
    Total: $${(precio * cantidad).toFixed(2)}
    IVA: $${(precio * cantidad * 0.21).toFixed(2)}
`;
```

### 📄 **Strings Multilínea**

```javascript
// ❌ ES5 - Strings multilínea complicadas
const html = '<div class="card">\n' +
             '  <h2>Título</h2>\n' +
             '  <p>Contenido</p>\n' +
             '</div>';

// ✅ ES6 - Template literals naturales
const html = `
    <div class="card">
        <h2>Título</h2>
        <p>Contenido</p>
    </div>
`;
```

### 🏷️ **Tagged Templates (Avanzado)**

```javascript
// ✅ Template personalizado para highlighting
function highlight(strings, ...values) {
    return strings.reduce((result, string, i) => {
        const value = values[i] ? `<mark>${values[i]}</mark>` : '';
        return result + string + value;
    }, '');
}

const busqueda = 'JavaScript';
const texto = highlight`Aprende ${busqueda} moderno con ES6+`;
// "Aprende <mark>JavaScript</mark> moderno con ES6+"
```

---

## 🎭 **DESTRUCTURING**

### 📦 **Arrays - Extracción Posicional**

```javascript
// ❌ ES5 - Acceso por índice
const colores = ['rojo', 'verde', 'azul'];
const primero = colores[0];
const segundo = colores[1];
const tercero = colores[2];

// ✅ ES6 - Destructuring de arrays
const [primero, segundo, tercero] = colores;

// ✅ Saltar elementos
const [primero, , tercero] = colores; // Omite 'verde'

// ✅ Valores por defecto
const [a, b, c, d = 'amarillo'] = colores; // d será 'amarillo'

// ✅ Rest en arrays
const [primero, ...resto] = colores; // resto = ['verde', 'azul']
```

### 🏗️ **Objetos - Extracción por Clave**

```javascript
// ❌ ES5 - Acceso por propiedades
const usuario = { nombre: 'Ana', edad: 25, email: 'ana@email.com' };
const nombre = usuario.nombre;
const edad = usuario.edad;
const email = usuario.email;

// ✅ ES6 - Destructuring de objetos
const { nombre, edad, email } = usuario;

// ✅ Renombrar variables
const { nombre: nombreCompleto, edad: años } = usuario;

// ✅ Valores por defecto
const { nombre, edad, activo = true } = usuario;

// ✅ Rest en objetos
const { nombre, ...datosContacto } = usuario; 
// datosContacto = { edad: 25, email: 'ana@email.com' }
```

### 🔧 **Destructuring en Parámetros**

```javascript
// ❌ ES5 - Acceder a propiedades dentro de función
function crearTarjeta(usuario) {
    var nombre = usuario.nombre;
    var email = usuario.email;
    return '<div>' + nombre + ' - ' + email + '</div>';
}

// ✅ ES6 - Destructuring en parámetros
function crearTarjeta({ nombre, email, activo = true }) {
    return `
        <div class="${activo ? 'active' : 'inactive'}">
            ${nombre} - ${email}
        </div>
    `;
}

// ✅ Arrays en parámetros
function mostrarCoordenadas([x, y, z = 0]) {
    console.log(`X: ${x}, Y: ${y}, Z: ${z}`);
}

mostrarCoordenadas([10, 20]); // X: 10, Y: 20, Z: 0
```

### 🔄 **Intercambio de Variables**

```javascript
// ❌ ES5 - Intercambio con variable temporal
let a = 1;
let b = 2;
let temp = a;
a = b;
b = temp;

// ✅ ES6 - Intercambio elegante
let a = 1;
let b = 2;
[a, b] = [b, a]; // a = 2, b = 1
```

---

## ⚡ **SPREAD (...) Y REST (...)**

### 📤 **Spread - Expandir Elementos**

```javascript
// ✅ Spread en Arrays
const numeros1 = [1, 2, 3];
const numeros2 = [4, 5, 6];

// Combinando arrays
const todos = [...numeros1, ...numeros2]; // [1, 2, 3, 4, 5, 6]

// Copiando arrays (shallow copy)
const copia = [...numeros1]; // [1, 2, 3]

// Añadiendo elementos
const masNumeros = [0, ...numeros1, 7, 8]; // [0, 1, 2, 3, 7, 8]
```

```javascript
// ✅ Spread en Objetos
const usuario = { nombre: 'Ana', edad: 25 };
const ubicacion = { ciudad: 'Madrid', pais: 'España' };

// Combinando objetos
const perfilCompleto = { ...usuario, ...ubicacion };
// { nombre: 'Ana', edad: 25, ciudad: 'Madrid', pais: 'España' }

// Copiando objetos (shallow copy)
const copiaUsuario = { ...usuario };

// Sobrescribiendo propiedades
const usuarioActualizado = { ...usuario, edad: 26, activo: true };
```

```javascript
// ✅ Spread en Llamadas a Funciones
function sumar(a, b, c) {
    return a + b + c;
}

const numeros = [1, 2, 3];

// ❌ ES5
const resultado = sumar.apply(null, numeros);

// ✅ ES6
const resultado = sumar(...numeros); // 6
```

### 📥 **Rest - Recoger Elementos**

```javascript
// ✅ Rest en Parámetros de Función
function sumarTodos(...numeros) {
    return numeros.reduce((total, num) => total + num, 0);
}

sumarTodos(1, 2, 3, 4, 5); // 15

// ✅ Mezclando parámetros normales con rest
function presentar(saludo, ...nombres) {
    return `${saludo} ${nombres.join(', ')}`;
}

presentar('Hola', 'Ana', 'Luis', 'María'); // "Hola Ana, Luis, María"
```

```javascript
// ✅ Rest en Destructuring
const [primero, segundo, ...resto] = [1, 2, 3, 4, 5];
// primero = 1, segundo = 2, resto = [3, 4, 5]

const { nombre, email, ...otrosDatos } = usuario;
// Separar propiedades específicas del resto
```

---

## 📦 **MÓDULOS ES6**

### 📤 **Exports - Exportando Funcionalidad**

```javascript
// ✅ Named Exports - utilities.js
export const PI = 3.14159;

export function calcularArea(radio) {
    return PI * radio * radio;
}

export class Calculadora {
    sumar(a, b) { return a + b; }
}

// ✅ Export todo junto
const API_URL = 'https://api.com';
function conectar() { /* ... */ }
class Usuario { /* ... */ }

export { API_URL, conectar, Usuario };
```

```javascript
// ✅ Default Export - user.js
export default class Usuario {
    constructor(nombre) {
        this.nombre = nombre;
    }
}

// ✅ Mezclando default y named exports
export const ROLES = ['admin', 'user'];
export function validarEmail(email) { /* ... */ }

export default class Usuario { /* ... */ }
```

### 📥 **Imports - Importando Funcionalidad**

```javascript
// ✅ Named Imports
import { calcularArea, PI, Calculadora } from './utilities.js';

// ✅ Renombrar imports
import { calcularArea as area, PI as pi } from './utilities.js';

// ✅ Import todo como namespace
import * as Utils from './utilities.js';
Utils.calcularArea(5);
Utils.PI;
```

```javascript
// ✅ Default Imports
import Usuario from './user.js';

// ✅ Mezclando default y named imports
import Usuario, { ROLES, validarEmail } from './user.js';

// ✅ Import dinámico (async)
async function cargarModulo() {
    const modulo = await import('./modulo-pesado.js');
    modulo.default();
}
```

### 🗂️ **Barrel Exports - Organizando Exports**

```javascript
// ✅ index.js - Punto de entrada único
export { Usuario, Admin } from './usuarios.js';
export { Producto, Categoria } from './productos.js';
export { validarEmail, formatearFecha } from './utilidades.js';

// ✅ Uso desde otro archivo
import { Usuario, Producto, validarEmail } from './modelos/index.js';
```

---

## 🔄 **PROMISES**

### 📋 **Sintaxis Básica**

```javascript
// ✅ Creando una Promise
const miPromesa = new Promise((resolve, reject) => {
    setTimeout(() => {
        const exito = Math.random() > 0.5;
        if (exito) {
            resolve('¡Operación exitosa!');
        } else {
            reject('Algo salió mal');
        }
    }, 1000);
});

// ✅ Consumiendo la Promise
miPromesa
    .then(resultado => {
        console.log(resultado); // '¡Operación exitosa!'
    })
    .catch(error => {
        console.error(error); // 'Algo salió mal'
    })
    .finally(() => {
        console.log('Operación completada');
    });
```

### 🔗 **Encadenamiento de Promises**

```javascript
// ✅ Chainig elegante
obtenerUsuario(1)
    .then(usuario => obtenerPedidos(usuario.id))
    .then(pedidos => calcularTotal(pedidos))
    .then(total => mostrarFactura(total))
    .catch(error => manejarError(error));

// ✅ Transformando datos en cada paso
fetch('/api/usuarios')
    .then(response => response.json())
    .then(usuarios => usuarios.filter(u => u.activo))
    .then(usuariosActivos => usuariosActivos.map(u => u.email))
    .then(emails => enviarNewsletter(emails))
    .catch(error => console.error('Error:', error));
```

### ⚡ **Promise Utilities**

```javascript
// ✅ Promise.all - Todas deben resolverse
const promesas = [
    fetch('/api/usuarios'),
    fetch('/api/productos'),
    fetch('/api/pedidos')
];

Promise.all(promesas)
    .then(responses => {
        console.log('Todas las APIs respondieron');
        // Procesar todas las respuestas
    })
    .catch(error => {
        console.error('Al menos una API falló:', error);
    });

// ✅ Promise.allSettled - Esperar todas, sin importar resultado
Promise.allSettled(promesas)
    .then(resultados => {
        resultados.forEach((resultado, index) => {
            if (resultado.status === 'fulfilled') {
                console.log(`API ${index} exitosa:`, resultado.value);
            } else {
                console.error(`API ${index} falló:`, resultado.reason);
            }
        });
    });

// ✅ Promise.race - La primera en resolverse
Promise.race([
    fetch('/api/servidor1'),
    fetch('/api/servidor2'),
    fetch('/api/servidor3')
])
.then(response => {
    console.log('El servidor más rápido respondió');
})
.catch(error => {
    console.error('Todos los servidores fallaron');
});
```

---

## ⚡ **ASYNC/AWAIT**

### 🎯 **Sintaxis Básica**

```javascript
// ❌ Con Promises (funcional pero verboso)
function obtenerDatos() {
    return fetch('/api/datos')
        .then(response => response.json())
        .then(datos => {
            console.log('Datos obtenidos:', datos);
            return datos;
        })
        .catch(error => {
            console.error('Error:', error);
            throw error;
        });
}

// ✅ Con async/await (limpio y legible)
async function obtenerDatos() {
    try {
        const response = await fetch('/api/datos');
        const datos = await response.json();
        console.log('Datos obtenidos:', datos);
        return datos;
    } catch (error) {
        console.error('Error:', error);
        throw error;
    }
}
```

### � **Operaciones Secuenciales y Paralelas**

```javascript
// ✅ Secuencial - Una después de otra
async function procesoSecuencial() {
    const usuario = await obtenerUsuario(1);     // 2s
    const pedidos = await obtenerPedidos(usuario.id); // 3s  
    const facturas = await obtenerFacturas(pedidos);  // 2s
    // Total: ~7 segundos
    return { usuario, pedidos, facturas };
}

// ✅ Paralelo - Todas a la vez
async function procesoParalelo() {
    const [usuario, configuracion, notificaciones] = await Promise.all([
        obtenerUsuario(1),        // 2s
        obtenerConfiguracion(),   // 1s
        obtenerNotificaciones()   // 3s
    ]);
    // Total: ~3 segundos (el más lento)
    return { usuario, configuracion, notificaciones };
}
```

### 🎭 **Patrones Avanzados**

```javascript
// ✅ Async en Array Methods
const urls = ['/api/datos1', '/api/datos2', '/api/datos3'];

// Secuencial (uno tras otro)
const resultadosSecuencial = [];
for (const url of urls) {
    const response = await fetch(url);
    const datos = await response.json();
    resultadosSecuencial.push(datos);
}

// Paralelo (todos a la vez)
const resultadosParalelo = await Promise.all(
    urls.map(async url => {
        const response = await fetch(url);
        return response.json();
    })
);

// ✅ Error handling avanzado
async function operacionCompleja() {
    let usuario, pedidos, facturas;
    
    try {
        usuario = await obtenerUsuario(1);
    } catch (error) {
        console.error('Error obteniendo usuario:', error);
        usuario = null;
    }
    
    try {
        pedidos = await obtenerPedidos(usuario?.id);
    } catch (error) {
        console.error('Error obteniendo pedidos:', error);
        pedidos = [];
    }
    
    return { usuario, pedidos };
}
```

---

## 🏛️ **CLASES ES6**

### 🏗️ **Sintaxis Básica**

```javascript
// ❌ ES5 - Función constructora
function Usuario(nombre, email) {
    this.nombre = nombre;
    this.email = email;
    this.activo = true;
}

Usuario.prototype.saludar = function() {
    return 'Hola, soy ' + this.nombre;
};

Usuario.crearAdmin = function(nombre, email) {
    var admin = new Usuario(nombre, email);
    admin.rol = 'admin';
    return admin;
};

// ✅ ES6 - Clase
class Usuario {
    constructor(nombre, email) {
        this.nombre = nombre;
        this.email = email;
        this.activo = true;
    }
    
    saludar() {
        return `Hola, soy ${this.nombre}`;
    }
    
    static crearAdmin(nombre, email) {
        const admin = new Usuario(nombre, email);
        admin.rol = 'admin';
        return admin;
    }
}
```

### 👨‍👩‍👧‍👦 **Herencia**

```javascript
// ✅ Herencia con extends y super
class Animal {
    constructor(nombre, especie) {
        this.nombre = nombre;
        this.especie = especie;
    }
    
    dormir() {
        return `${this.nombre} está durmiendo`;
    }
}

class Perro extends Animal {
    constructor(nombre, raza) {
        super(nombre, 'perro'); // Llamar constructor padre
        this.raza = raza;
    }
    
    ladrar() {
        return `${this.nombre} está ladrando!`;
    }
    
    // Sobrescribir método padre
    dormir() {
        return `${super.dormir()} en su cama de perro`;
    }
}

const firulais = new Perro('Firulais', 'Golden');
console.log(firulais.dormir()); // "Firulais está durmiendo en su cama de perro"
```

### 🎨 **Getters y Setters**

```javascript
class Rectangulo {
    constructor(ancho, alto) {
        this._ancho = ancho;
        this._alto = alto;
    }
    
    // Getter - se usa como propiedad
    get area() {
        return this._ancho * this._alto;
    }
    
    get perimetro() {
        return 2 * (this._ancho + this._alto);
    }
    
    // Setter - se usa como asignación
    set ancho(valor) {
        if (valor > 0) {
            this._ancho = valor;
        }
    }
    
    set alto(valor) {
        if (valor > 0) {
            this._alto = valor;
        }
    }
}

const rect = new Rectangulo(10, 5);
console.log(rect.area);      // 50 (usa getter)
rect.ancho = 15;             // Usa setter
console.log(rect.area);      // 75
```

---

## 🆚 **COMPARACIONES ES5 vs ES6+**

### 📊 **Tabla de Equivalencias Rápidas**

| **Concepto** | **❌ ES5** | **✅ ES6+** |
|--------------|------------|-------------|
| **Variables** | `var nombre = 'Ana';` | `const nombre = 'Ana';` |
| **Funciones** | `function suma(a,b) { return a+b; }` | `const suma = (a,b) => a+b;` |
| **Strings** | `'Hola ' + nombre + '!'` | \`Hola ${nombre}!\` |
| **Objetos** | `var n = obj.nombre; var e = obj.email;` | `const {nombre, email} = obj;` |
| **Arrays** | `var primero = arr[0];` | `const [primero] = arr;` |
| **Clases** | `function User() {}` | `class User {}` |
| **Módulos** | `var mod = require('mod');` | `import mod from 'mod';` |
| **Promesas** | `callback(err, data)` | `await fetch(url)` |

### 🎯 **Casos de Uso Principales**

```javascript
// 🎯 ANTES: Código ES5 típico
var usuarios = [];
var configuracion = { tema: 'claro', idioma: 'es' };

function buscarUsuario(nombre, callback) {
    setTimeout(function() {
        var encontrado = null;
        for (var i = 0; i < usuarios.length; i++) {
            if (usuarios[i].nombre === nombre) {
                encontrado = usuarios[i];
                break;
            }
        }
        callback(encontrado);
    }, 100);
}

function crearTarjetaUsuario(usuario) {
    var html = '<div class="tarjeta">' +
               '<h3>' + usuario.nombre + '</h3>' +
               '<p>' + usuario.email + '</p>' +
               '</div>';
    return html;
}

// 🎯 DESPUÉS: Código ES6+ moderno
const usuarios = [];
const configuracion = { tema: 'claro', idioma: 'es' };

const buscarUsuario = async (nombre) => {
    return new Promise(resolve => {
        setTimeout(() => {
            const encontrado = usuarios.find(u => u.nombre === nombre);
            resolve(encontrado);
        }, 100);
    });
};

const crearTarjetaUsuario = ({ nombre, email, activo = true }) => `
    <div class="tarjeta ${activo ? 'active' : 'inactive'}">
        <h3>${nombre}</h3>
        <p>${email}</p>
    </div>
`;
```

---

## 🎯 **EJERCICIOS RÁPIDOS**

### 🧪 **Refactoring Challenge**

**Convierte este código ES5 a ES6+:**

```javascript
// ❌ Código ES5 para refactorizar
function CrearLibreria(nombre) {
    this.nombre = nombre;
    this.libros = [];
}

CrearLibreria.prototype.agregarLibro = function(titulo, autor, año) {
    var libro = {
        titulo: titulo,
        autor: autor,
        año: año,
        id: this.libros.length + 1
    };
    this.libros.push(libro);
};

CrearLibreria.prototype.buscarLibro = function(titulo, callback) {
    var self = this;
    setTimeout(function() {
        var encontrado = null;
        for (var i = 0; i < self.libros.length; i++) {
            if (self.libros[i].titulo === titulo) {
                encontrado = self.libros[i];
                break;
            }
        }
        callback(encontrado);
    }, 100);
};

CrearLibreria.prototype.mostrarLibros = function() {
    var html = '';
    for (var i = 0; i < this.libros.length; i++) {
        var libro = this.libros[i];
        html += '<div>' + libro.titulo + ' - ' + libro.autor + '</div>';
    }
    return html;
};

// ✅ Tu versión ES6+ aquí:
// class Libreria {
//     // Tu código...
// }
```

### 🎮 **Mini Desafíos**

1. **Arrow Functions**: Convierte estas funciones a arrow functions:
```javascript
// Convertir a arrow functions:
function multiplicar(a, b) { return a * b; }
function saludar(nombre) { return 'Hola ' + nombre; }
function obtenerPares(numeros) {
    return numeros.filter(function(n) { return n % 2 === 0; });
}
```

2. **Destructuring**: Extrae las propiedades usando destructuring:
```javascript
const usuario = { 
    nombre: 'Ana', 
    edad: 25, 
    direccion: { ciudad: 'Madrid', pais: 'España' } 
};
// Extraer: nombre, edad, ciudad
```

3. **Template Literals**: Convierte estas concatenaciones:
```javascript
const producto = 'Laptop';
const precio = 999.99;
const descuento = 10;
// Crear: "Oferta especial: Laptop por solo $899.99 (10% descuento)"
```

---

## 🚀 **PRÓXIMOS PASOS**

### 📈 **Roadmap de Aprendizaje**

```javascript
const tuProgreso = {
    actual: "JavaScript ES6+ Básico ✅",
    siguiente: [
        "JavaScript Avanzado (Proxies, Generators)",
        "TypeScript para tipado estático",
        "Node.js para backend",
        "React/Vue/Angular para frontend"
    ],
    
    proyectosSugeridos: [
        "Refactorizar proyecto existente a ES6+",
        "Crear API REST con módulos ES6",
        "SPA con Vanilla JS moderno",
        "PWA con Service Workers"
    ]
};
```

### 🎯 **Checklist de Dominio**

- [ ] **Variables**: Uso correcto de let/const, evitar var
- [ ] **Arrow Functions**: Sintaxis y comportamiento de 'this'
- [ ] **Template Literals**: Interpolación y strings multilínea  
- [ ] **Destructuring**: Arrays, objetos y parámetros
- [ ] **Spread/Rest**: Operaciones con arrays y objetos
- [ ] **Módulos**: Import/export y organización
- [ ] **Promises**: Creación, consumo y encadenamiento
- [ ] **Async/Await**: Código asíncrono legible
- [ ] **Clases**: POO moderna con herencia

---

**🎯 ¿Listo para dominar JavaScript moderno?**

[🏠 **Volver al Libro Principal**](./JAVASCRIPT-MODERNO-LIBRO.md) | [🧪 **Ejercicios Prácticos**](./ejercicios-practicos/README-EJERCICIOS.md) | [📚 **Navegación**](../../../NAVEGACION-DOCUMENTOS.md)

---

*💡 **Tip Pro**: Imprime esta cheatsheet y tenla siempre a mano. La referencia visual acelera el aprendizaje y mejora la retención.*

[🔙 **Volver al Libro Principal**](JAVASCRIPT-MODERNO-LIBRO.md) | [🏠 **Índice General**](../../../README.md) | [📚 **Navegación**](../../../NAVEGACION-DOCUMENTOS.md) | [🧪 **Ejercicios Prácticos**](ejercicios-practicos/README-EJERCICIOS.md)
