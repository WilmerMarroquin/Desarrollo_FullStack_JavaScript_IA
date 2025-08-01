[🏠 **Volver al Índice de Navegación**](../../../NAVEGACION-DOCUMENTOS.md)

---

# 📝 JavaScript Cheatsheet Visual

> **📝 "Un buen cheatsheet vale más que mil tutoriales cuando estás programando. Aquí tienes tu referencia rápida definitiva."**

## 🎨 **Guía de Uso del Cheatsheet**

```javascript
// 🎯 Cómo usar este cheatsheet:
const guiaUso = {
    purpose: "📋 Referencia rápida mientras programas",
    usage: "🔍 Busca por categoría o usa Ctrl+F para encontrar lo que necesitas",
    level: "📈 Desde principiante hasta avanzado",
    format: "💻 Código copiable y pegable directamente"
};

// 🌈 Leyenda de símbolos:
// ✅ Recomendado / Buena práctica
// ❌ Evitar / Mala práctica  
// 🔥 Moderno / ES6+
// ⚡ Optimización
// 🐛 Propenso a errores
// 💡 Tip importante
```

---

## 📊 **Variables y Tipos de Datos**

### 🏷️ **Declaración de Variables**

```javascript
// 🔥 MODERNO (ES6+) - Usa estos
const nombre = "Juan";           // ✅ Constante, no se puede reasignar
let edad = 25;                   // ✅ Variable que puede cambiar
let activo;                      // undefined inicialmente

// 🐛 LEGACY - Evitar en código nuevo
var antiguaVariable = "valor";   // ❌ Función scope, hoisting confuso

// 💡 Reglas de nombrado
const miVariable = "camelCase";          // ✅ Para variables y funciones
const MI_CONSTANTE = "MAYÚSCULAS";       // ✅ Para constantes globales
const _privada = "guión bajo";           // ✅ Para indicar "privado"
const $elemento = document.body;         // ✅ Para elementos DOM

// ❌ Nombres que evitar
const 123variable;     // Error: No puede empezar con número
const mi-variable;     // Error: Guiones no permitidos
const class;           // Error: Palabra reservada
```

### 🎭 **Tipos de Datos Primitivos**

```javascript
// 📝 String (Cadenas de texto)
const texto1 = "Comillas dobles";
const texto2 = 'Comillas simples';
const texto3 = `Template literal con ${variable}`;  // 🔥 ES6

// 🔢 Number (Números)
const entero = 42;
const decimal = 3.14159;
const negativo = -10;
const infinito = Infinity;
const noNumero = NaN;

// ✅ Boolean (Verdadero/Falso)
const verdadero = true;
const falso = false;

// 🚫 Null y Undefined
const nulo = null;          // Intencionalmente vacío
let indefinido;             // undefined automáticamente

// 🔣 Symbol (ES6) - Identificadores únicos
const simbolo = Symbol('id');

// 📊 BigInt (ES2020) - Números muy grandes
const numeroGigante = 123456789012345678901234567890n;
```

### 🧪 **Verificación de Tipos**

```javascript
// 🔍 Operador typeof
typeof "texto"      // "string"
typeof 42           // "number"
typeof true         // "boolean"
typeof undefined    // "undefined"
typeof null         // "object" 🐛 Bug histórico de JS
typeof {}           // "object"
typeof []           // "object" 🐛 Arrays son objetos
typeof function(){} // "function"

// ✅ Métodos más precisos
Array.isArray([1,2,3])           // true
Number.isInteger(42)             // true
Number.isNaN(NaN)                // true
Object.prototype.toString.call([]) // "[object Array]"

// 🎯 Función helper para tipos exactos
function tipoExacto(valor) {
    return Object.prototype.toString.call(valor).slice(8, -1).toLowerCase();
}

tipoExacto([1,2,3])    // "array"
tipoExacto(new Date()) // "date"
tipoExacto(/regex/)    // "regexp"
```

---

## ⚡ **Operadores**

### 🧮 **Operadores Aritméticos**

```javascript
// Básicos
5 + 3      // 8  - Suma
5 - 3      // 2  - Resta
5 * 3      // 15 - Multiplicación
5 / 3      // 1.666... - División
5 % 3      // 2  - Módulo (resto)
5 ** 3     // 125 - Exponenciación 🔥 ES2016

// Incremento/Decremento
let x = 5;
x++        // Post-incremento: usa x, luego suma 1
++x        // Pre-incremento: suma 1, luego usa x
x--        // Post-decremento
--x        // Pre-decremento

// Asignación combinada
x += 5     // x = x + 5
x -= 3     // x = x - 3
x *= 2     // x = x * 2
x /= 4     // x = x / 4
x %= 3     // x = x % 3
x **= 2    // x = x ** 2 🔥
```

### 🔍 **Operadores de Comparación**

```javascript
// 💡 Siempre usa === y !== (estrictos)
5 === 5    // true  ✅ Mismo valor y tipo
5 === "5"  // false ✅ Diferentes tipos

// 🐛 Evita == y != (conversión automática)
5 == "5"   // true  ❌ Conversión confusa
0 == false // true  ❌ Conversión confusa

// Relacionales
5 > 3      // true
5 < 3      // false
5 >= 5     // true
5 <= 3     // false

// 🎯 Comparación de strings (lexicográfica)
"abc" < "def"     // true
"ABC" < "abc"     // true (mayúsculas primero)
"10" < "2"        // true (¡string, no número!)
```

### 🔗 **Operadores Lógicos**

```javascript
// AND lógico - Todas deben ser true
true && true     // true
true && false    // false

// OR lógico - Al menos una debe ser true
true || false    // true
false || false   // false

// NOT lógico - Invierte el valor
!true           // false
!false          // true
!!valor         // Convierte a boolean

// 🔥 Operadores de asignación lógica (ES2021)
x ||= 5         // x = x || 5 (asigna si x es falsy)
x &&= 5         // x = x && 5 (asigna si x es truthy)
x ??= 5         // x = x ?? 5 (asigna si x es null/undefined)

// 🎯 Short-circuit evaluation
false && console.log("No se ejecuta");
true || console.log("No se ejecuta");
```

### 🔥 **Operadores Modernos**

```javascript
// Nullish Coalescing ?? (ES2020)
const nombre = usuario.nombre ?? "Anónimo";  // Solo null/undefined
const edad = usuario.edad ?? 0;

// Optional Chaining ?. (ES2020)
const email = usuario?.contacto?.email;      // No error si undefined
const metodo = objeto?.metodo?.();           // Llamada segura

// Spread Operator ... (ES6)
const arr1 = [1, 2, 3];
const arr2 = [...arr1, 4, 5];              // [1, 2, 3, 4, 5]
const obj1 = {a: 1};
const obj2 = {...obj1, b: 2};              // {a: 1, b: 2}

// Destructuring (ES6)
const [primer, segundo] = [10, 20];         // primer=10, segundo=20
const {nombre, edad} = persona;             // Extrae propiedades
```

---

## 🔄 **Estructuras de Control**

### 🌿 **Condicionales**

```javascript
// 🎯 if...else básico
if (condicion) {
    // código si true
} else if (otraCondicion) {
    // código si la segunda es true
} else {
    // código si todas son false
}

// 🔥 Operador ternario (condición ? true : false)
const resultado = edad >= 18 ? "Adulto" : "Menor";
const mensaje = usuario ? `Hola ${usuario}` : "Usuario no encontrado";

// 🎭 Switch optimizado
switch (dia) {
    case 'lunes':
    case 'martes':
    case 'miercoles':
        console.log("Inicio de semana");
        break;
    case 'jueves':
    case 'viernes':
        console.log("Fin de semana");
        break;
    default:
        console.log("Fin de semana");
}

// 🔥 Switch expressions (propuesta)
const tipo = valor => {
    switch (true) {
        case valor > 100: return "alto";
        case valor > 50:  return "medio";
        default:          return "bajo";
    }
};
```

### 🔁 **Bucles**

```javascript
// 🎯 for clásico - Para contadores
for (let i = 0; i < array.length; i++) {
    console.log(array[i]);
}

// 🔥 for...of - Para valores (ES6)
for (const elemento of array) {        // ✅ Mejor para arrays
    console.log(elemento);
}

for (const caracter of "texto") {      // ✅ Funciona con strings
    console.log(caracter);
}

// 🎭 for...in - Para claves (propiedades)
for (const clave in objeto) {          // ✅ Para objetos
    console.log(clave, objeto[clave]);
}

// ⚡ while - Mientras condición sea true
while (condicion) {
    // código que puede cambiar la condición
}

// 🎪 do...while - Ejecuta al menos una vez
do {
    // código
} while (condicion);

// 🚪 Control de flujo
for (let i = 0; i < 10; i++) {
    if (i === 3) continue;    // Salta a la siguiente iteración
    if (i === 7) break;       // Sale del bucle completamente
    console.log(i);           // 0,1,2,4,5,6
}
```

---

## 🏗️ **Funciones**

### 📦 **Declaración de Funciones**

```javascript
// 🎯 Function Declaration - Hoisted
function saludar(nombre) {
    return `Hola ${nombre}!`;
}

// 🔥 Function Expression - No hoisted
const saludar = function(nombre) {
    return `Hola ${nombre}!`;
};

// 🚀 Arrow Functions (ES6) - Sintaxis corta
const saludar = nombre => `Hola ${nombre}!`;
const sumar = (a, b) => a + b;
const procesar = datos => {
    // código complejo
    return resultado;
};

// 💡 Parámetros por defecto (ES6)
function crear(nombre = "Anónimo", edad = 0) {
    return {nombre, edad};
}

// 🎪 Rest Parameters (ES6)
function sumarTodos(...numeros) {
    return numeros.reduce((a, b) => a + b, 0);
}

// 🎯 Destructuring en parámetros
function presentar({nombre, edad, ciudad = "No especificada"}) {
    return `${nombre}, ${edad} años, de ${ciudad}`;
}
```

### 🎨 **Funciones Avanzadas**

```javascript
// 🏭 IIFE - Immediately Invoked Function Expression
(function() {
    console.log("Se ejecuta inmediatamente");
})();

// 🔥 IIFE con arrow function
(() => {
    console.log("IIFE moderno");
})();

// 🎭 Closures - Funciones que "recuerdan"
function contador() {
    let count = 0;
    return function() {
        return ++count;
    };
}
const miContador = contador();
miContador(); // 1
miContador(); // 2

// 🏗️ Función constructora (antes de ES6)
function Persona(nombre, edad) {
    this.nombre = nombre;
    this.edad = edad;
    this.saludar = function() {
        return `Hola, soy ${this.nombre}`;
    };
}

// 🔥 Class syntax (ES6) - Más limpio
class Persona {
    constructor(nombre, edad) {
        this.nombre = nombre;
        this.edad = edad;
    }
    
    saludar() {
        return `Hola, soy ${this.nombre}`;
    }
    
    static crear(datos) {
        return new Persona(datos.nombre, datos.edad);
    }
}
```

---

## 📋 **Arrays (Arreglos)**

### 🎯 **Creación y Básicos**

```javascript
// 📝 Creación
const numeros = [1, 2, 3, 4, 5];
const mixto = [1, "texto", true, null];
const vacio = [];
const conTamaño = new Array(5);              // [empty × 5]
const desde = Array.from("hello");          // ['h','e','l','l','o']
const rango = Array.from({length: 5}, (_, i) => i); // [0,1,2,3,4]

// 🔍 Propiedades básicas
numeros.length        // 5
numeros[0]           // 1 (primer elemento)
numeros[-1]          // undefined ❌ No funciona como Python
numeros.at(-1)       // 5 🔥 ES2022 - último elemento
```

### ⚡ **Métodos de Modificación**

```javascript
let frutas = ['manzana', 'banana'];

// 📎 Agregar elementos
frutas.push('naranja');              // Final: ['manzana', 'banana', 'naranja']
frutas.unshift('fresa');             // Inicio: ['fresa', 'manzana', 'banana', 'naranja']
frutas.splice(2, 0, 'uva');          // Posición 2: ['fresa', 'manzana', 'uva', 'banana', 'naranja']

// ✂️ Remover elementos
frutas.pop();                        // Último: ['fresa', 'manzana', 'uva', 'banana']
frutas.shift();                      // Primero: ['manzana', 'uva', 'banana']
frutas.splice(1, 1);                 // Posición 1, 1 elemento: ['manzana', 'banana']

// 🔄 Otros métodos de modificación
frutas.reverse();                    // Invierte: ['banana', 'manzana']
frutas.sort();                       // Ordena: ['banana', 'manzana'] (lexicográfico)
frutas.sort((a, b) => a.localeCompare(b)); // Orden correcto para strings
```

### 🎨 **Métodos Funcionales**

```javascript
const numeros = [1, 2, 3, 4, 5];

// 🗺️ map - Transforma cada elemento
const dobles = numeros.map(n => n * 2);           // [2, 4, 6, 8, 10]
const strings = numeros.map(n => `#${n}`);        // ['#1', '#2', '#3', '#4', '#5']

// 🔍 filter - Filtra elementos que cumplan condición
const pares = numeros.filter(n => n % 2 === 0);   // [2, 4]
const mayores = numeros.filter(n => n > 3);       // [4, 5]

// 🎯 find - Encuentra el primer elemento que cumpla
const encontrado = numeros.find(n => n > 3);      // 4
const persona = personas.find(p => p.id === 123);

// 📍 findIndex - Encuentra el índice del primer elemento
const indice = numeros.findIndex(n => n > 3);     // 3

// ✅ some - ¿Alguno cumple la condición?
const hayPares = numeros.some(n => n % 2 === 0);  // true

// 🎪 every - ¿Todos cumplen la condición?
const todosPares = numeros.every(n => n % 2 === 0); // false

// 🎭 reduce - Reduce a un solo valor
const suma = numeros.reduce((acc, n) => acc + n, 0);           // 15
const max = numeros.reduce((acc, n) => Math.max(acc, n));      // 5
const obj = numeros.reduce((acc, n) => ({...acc, [n]: n*2}), {}); // {1:2, 2:4, 3:6, 4:8, 5:10}

// 🔗 forEach - Ejecuta función para cada elemento
numeros.forEach((numero, indice) => {
    console.log(`${indice}: ${numero}`);
});
```

### 🎯 **Métodos de Búsqueda y Verificación**

```javascript
const frutas = ['manzana', 'banana', 'naranja', 'banana'];

// 🔍 Búsqueda
frutas.includes('banana');          // true
frutas.indexOf('banana');           // 1 (primer ocurrencia)
frutas.lastIndexOf('banana');       // 3 (última ocurrencia)

// ✂️ Extracción
frutas.slice(1, 3);                 // ['banana', 'naranja'] (no modifica original)
frutas.splice(1, 2);                // ['banana', 'naranja'] ❌ Modifica original

// 🔗 Unión
const mas = ['uva', 'pera'];
const todas = frutas.concat(mas);   // Nuevo array
const todas2 = [...frutas, ...mas]; // 🔥 ES6 más legible

// 🎯 Conversión
frutas.join(', ');                  // "manzana, banana, naranja, banana"
frutas.toString();                  // "manzana,banana,naranja,banana"
```

---

## 🗂️ **Objetos**

### 🏗️ **Creación y Básicos**

```javascript
// 📝 Creación literal
const persona = {
    nombre: "Ana",
    edad: 30,
    activo: true,
    direccion: {
        calle: "Principal 123",
        ciudad: "Madrid"
    }
};

// 🎯 Acceso a propiedades
persona.nombre              // "Ana"
persona['edad']             // 30
persona['prop-con-guion']   // Para propiedades con caracteres especiales

// 🔥 Computed property names (ES6)
const clave = 'dinamica';
const obj = {
    [clave]: 'valor',           // dinamica: 'valor'
    [`${clave}_2`]: 'valor2'    // dinamica_2: 'valor2'
};

// 🎨 Property shorthand (ES6)
const nombre = "Juan";
const edad = 25;
const persona2 = { nombre, edad };  // Equivale a { nombre: nombre, edad: edad }

// 🎭 Method shorthand (ES6)
const calculadora = {
    sumar(a, b) { return a + b; },      // Equivale a: sumar: function(a, b) { return a + b; }
    restar(a, b) { return a - b; }
};
```

### ⚡ **Métodos de Objeto**

```javascript
const persona = { nombre: "Ana", edad: 30, ciudad: "Madrid" };

// 🔑 Object.keys - Array de claves
Object.keys(persona);           // ['nombre', 'edad', 'ciudad']

// 💎 Object.values - Array de valores
Object.values(persona);         // ['Ana', 30, 'Madrid']

// 🎭 Object.entries - Array de [clave, valor]
Object.entries(persona);        // [['nombre', 'Ana'], ['edad', 30], ['ciudad', 'Madrid']]

// 🔄 Object.fromEntries - De entries a objeto (ES2019)
const entries = [['a', 1], ['b', 2]];
Object.fromEntries(entries);    // { a: 1, b: 2 }

// 🎯 Object.assign - Combinar objetos
const extra = { profesion: "Doctora" };
const completo = Object.assign({}, persona, extra);

// 🔥 Spread operator (ES6) - Más limpio
const completo2 = { ...persona, ...extra };

// ❄️ Object.freeze - Inmutable
Object.freeze(persona);         // No se puede modificar
persona.edad = 31;              // Silenciosamente ignorado (strict mode: error)

// 🔒 Object.seal - Solo modificar, no agregar/eliminar
Object.seal(persona);

// 🔍 Verificaciones
Object.isFrozen(persona);       // true
Object.isSealed(persona);       // true
persona.hasOwnProperty('nombre'); // true 🐛 Mejor usar Object.hasOwn
Object.hasOwn(persona, 'nombre'); // true 🔥 ES2022
```

### 🎨 **Destructuring de Objetos**

```javascript
const usuario = {
    id: 123,
    nombre: "María",
    email: "maria@email.com",
    perfil: {
        avatar: "avatar.jpg",
        bio: "Desarrolladora"
    }
};

// 🎯 Destructuring básico
const { nombre, email } = usuario;

// 🏷️ Renombrar variables
const { nombre: nombreUsuario, email: correo } = usuario;

// 💡 Valores por defecto
const { telefono = "No disponible" } = usuario;

// 🎭 Destructuring anidado
const { perfil: { avatar, bio } } = usuario;

// 🎪 Rest operator en objetos
const { nombre, ...resto } = usuario;  // resto contiene todo excepto nombre

// 🔄 En parámetros de función
function mostrarUsuario({ nombre, email, edad = "No especificada" }) {
    console.log(`${nombre} - ${email} - ${edad} años`);
}
```

---

## 🎭 **Strings (Cadenas)**

### 🔤 **Métodos de String**

```javascript
const texto = "  Hola Mundo JavaScript  ";

// 🎯 Información básica
texto.length                    // 25
texto.charAt(2)                 // "H" (carácter en posición 2)
texto.charCodeAt(2)             // 72 (código ASCII)

// 🔍 Búsqueda
texto.indexOf("Mundo")          // 7 (primera ocurrencia)
texto.lastIndexOf("a")          // 18 (última ocurrencia)
texto.includes("JavaScript")    // true 🔥 ES6
texto.startsWith("  Hola")      // true 🔥 ES6
texto.endsWith("  ")            // true 🔥 ES6

// ✂️ Extracción
texto.slice(2, 6)               // "Hola" (desde índice 2 hasta 6-1)
texto.substring(2, 6)           // "Hola" (similar a slice)
texto.substr(2, 4)              // "Hola" ❌ Deprecated

// 🎨 Transformación
texto.toLowerCase()             // "  hola mundo javascript  "
texto.toUpperCase()             // "  HOLA MUNDO JAVASCRIPT  "
texto.trim()                    // "Hola Mundo JavaScript" (quita espacios)
texto.trimStart()               // "Hola Mundo JavaScript  " 🔥 ES2019
texto.trimEnd()                 // "  Hola Mundo JavaScript" 🔥 ES2019

// 🔄 Reemplazo
texto.replace("Mundo", "Universo")      // Solo primera ocurrencia
texto.replaceAll("a", "@")              // 🔥 ES2021 - Todas las ocurrencias
texto.replace(/a/g, "@")                // Con regex (alternativa)

// ✂️ División
"apple,banana,orange".split(",")        // ['apple', 'banana', 'orange']
"hello".split("")                       // ['h', 'e', 'l', 'l', 'o']

// 🎯 Padding (ES2017)
"5".padStart(3, "0")                    // "005"
"5".padEnd(3, "0")                      // "500"

// 🔄 Repetición (ES6)
"Ha".repeat(3)                          // "HaHaHa"
```

### 🔥 **Template Literals (ES6)**

```javascript
const nombre = "Ana";
const edad = 25;

// 🎨 Interpolación básica
const mensaje = `Hola ${nombre}, tienes ${edad} años`;

// 🎭 Expresiones complejas
const saludo = `${nombre.toUpperCase()}, en 10 años tendrás ${edad + 10} años`;

// 📄 Multilinea
const html = `
    <div class="usuario">
        <h2>${nombre}</h2>
        <p>Edad: ${edad}</p>
    </div>
`;

// 🎪 Tagged templates (avanzado)
function highlight(strings, ...values) {
    return strings.reduce((result, string, i) => {
        return result + string + (values[i] ? `<mark>${values[i]}</mark>` : '');
    }, '');
}

const destacado = highlight`El usuario ${nombre} tiene ${edad} años`;
// "El usuario <mark>Ana</mark> tiene <mark>25</mark> años"
```

---

## 🕐 **Fechas y Tiempo**

### 📅 **Date Object**

```javascript
// 🎯 Creación
const ahora = new Date();                    // Fecha/hora actual
const especifica = new Date(2024, 0, 15);   // 15 enero 2024 (mes base 0)
const desde_string = new Date("2024-01-15"); // Desde string ISO
const timestamp = new Date(1642204800000);   // Desde timestamp

// 📊 Obtener componentes
ahora.getFullYear()     // 2024
ahora.getMonth()        // 0-11 (0 = enero) 🐛
ahora.getDate()         // 1-31 (día del mes)
ahora.getDay()          // 0-6 (0 = domingo) 🐛
ahora.getHours()        // 0-23
ahora.getMinutes()      // 0-59
ahora.getSeconds()      // 0-59
ahora.getTime()         // Timestamp en milisegundos

// 🎨 Formatear
ahora.toString()        // "Mon Jan 15 2024 10:30:00 GMT+0100"
ahora.toDateString()    // "Mon Jan 15 2024"
ahora.toTimeString()    // "10:30:00 GMT+0100"
ahora.toISOString()     // "2024-01-15T09:30:00.000Z"
ahora.toLocaleDateString() // "15/1/2024" (depende del locale)

// 🔄 Modificar
ahora.setFullYear(2025)
ahora.setMonth(11)      // Diciembre
ahora.setDate(25)       // Día 25

// ⚡ Métodos estáticos útiles
Date.now()              // Timestamp actual
Date.parse("2024-01-15") // Convierte string a timestamp
```

### 🎯 **Operaciones Comunes**

```javascript
// 📊 Calcular diferencias
const fecha1 = new Date("2024-01-01");
const fecha2 = new Date("2024-01-15");
const diferenciaDias = (fecha2 - fecha1) / (1000 * 60 * 60 * 24); // 14 días

// 🎨 Formateo personalizado
function formatearFecha(fecha) {
    const dia = fecha.getDate().toString().padStart(2, '0');
    const mes = (fecha.getMonth() + 1).toString().padStart(2, '0');
    const año = fecha.getFullYear();
    return `${dia}/${mes}/${año}`;
}

// 🌍 Intl.DateTimeFormat (ES6) - Más potente
const formateador = new Intl.DateTimeFormat('es-ES', {
    year: 'numeric',
    month: 'long',
    day: 'numeric',
    weekday: 'long'
});
formateador.format(new Date()); // "lunes, 15 de enero de 2024"

// ⏱️ Timeout y Interval
setTimeout(() => console.log("Después de 1 segundo"), 1000);
const intervalo = setInterval(() => console.log("Cada 2 segundos"), 2000);
clearInterval(intervalo); // Para detener
```

---

## 🎯 **Métodos Útiles**

### 🧮 **Math Object**

```javascript
// 🎯 Constantes
Math.PI         // 3.141592653589793
Math.E          // 2.718281828459045

// 🔢 Redondeo
Math.round(4.7)     // 5    - Redondeo normal
Math.ceil(4.1)      // 5    - Hacia arriba
Math.floor(4.9)     // 4    - Hacia abajo
Math.trunc(4.9)     // 4    - Quita decimales 🔥 ES6

// 📊 Min/Max
Math.min(1, 2, 3)   // 1
Math.max(1, 2, 3)   // 3
Math.min(...array)  // Min de array usando spread

// 🎲 Random
Math.random()                    // 0-1 (no incluye 1)
Math.floor(Math.random() * 10)   // 0-9
Math.floor(Math.random() * (max - min + 1)) + min // Entre min y max

// ⚡ Potencias y raíces
Math.pow(2, 3)      // 8    - 2³
Math.sqrt(16)       // 4    - Raíz cuadrada
Math.cbrt(27)       // 3    - Raíz cúbica 🔥 ES6

// 🎭 Trigonometría
Math.sin(Math.PI / 2)   // 1
Math.cos(0)             // 1
Math.tan(Math.PI / 4)   // 1

// 📈 Absoluto y signo
Math.abs(-5)        // 5
Math.sign(-5)       // -1 🔥 ES6
Math.sign(0)        // 0
Math.sign(5)        // 1
```

### 🎨 **Utilidades de Conversión**

```javascript
// 🔢 String a Number
parseInt("123px")       // 123
parseFloat("123.45px")  // 123.45
Number("123")           // 123
+"123"                  // 123 (conversión implícita)

// 📝 Number a String
const num = 123.456;
num.toString()          // "123.456"
num.toFixed(2)          // "123.46" (2 decimales)
num.toPrecision(4)      // "123.5" (4 cifras significativas)

// 🎯 Boolean
Boolean(1)              // true
Boolean(0)              // false
Boolean("")             // false
Boolean("texto")        // true
!!valor                 // Conversión rápida a boolean

// 📊 JSON
const obj = {nombre: "Ana", edad: 25};
JSON.stringify(obj)     // '{"nombre":"Ana","edad":25}'
JSON.parse('{"a":1}')   // {a: 1}

// 🎨 Con formato
JSON.stringify(obj, null, 2);  // Formato bonito con indentación
```

---

## 🚨 **Manejo de Errores**

### 🛡️ **Try-Catch-Finally**

```javascript
// 🎯 Básico
try {
    // Código que puede fallar
    const resultado = operacionRiesgosa();
    console.log(resultado);
} catch (error) {
    // Manejo del error
    console.error("Error:", error.message);
} finally {
    // Se ejecuta siempre
    console.log("Limpieza");
}

// 🎭 Diferentes tipos de errores
try {
    throw new Error("Error genérico");
    throw new TypeError("Error de tipo");
    throw new ReferenceError("Variable no definida");
    throw new SyntaxError("Error de sintaxis");
} catch (error) {
    if (error instanceof TypeError) {
        console.log("Es un error de tipo");
    } else if (error instanceof ReferenceError) {
        console.log("Variable no encontrada");
    } else {
        console.log("Otro tipo de error:", error.name);
    }
}

// 🎯 Errores personalizados
class MiError extends Error {
    constructor(mensaje) {
        super(mensaje);
        this.name = "MiError";
    }
}

throw new MiError("Algo salió mal");
```

### 🔄 **Async/Await con Errores**

```javascript
// 🚀 Con funciones async
async function manejarAsync() {
    try {
        const datos = await fetch('https://api.ejemplo.com/datos');
        const json = await datos.json();
        return json;
    } catch (error) {
        console.error("Error en la petición:", error);
        throw error; // Re-lanzar si es necesario
    } finally {
        console.log("Petición completada");
    }
}

// 🎯 Múltiples awaits
async function procesoComplejo() {
    try {
        const paso1 = await operacion1();
        const paso2 = await operacion2(paso1);
        const paso3 = await operacion3(paso2);
        return paso3;
    } catch (error) {
        // Cualquier await que falle llegará aquí
        console.error("Error en el proceso:", error);
    }
}
```

---

## 🌟 **ES6+ Características Modernas**

### 🔄 **Promises**

```javascript
// 🎯 Crear Promise
const miPromise = new Promise((resolve, reject) => {
    setTimeout(() => {
        if (Math.random() > 0.5) {
            resolve("¡Éxito!");
        } else {
            reject("Error!");
        }
    }, 1000);
});

// 🎭 Usar Promise
miPromise
    .then(resultado => console.log(resultado))
    .catch(error => console.error(error))
    .finally(() => console.log("Terminado"));

// 🚀 Promise.all - Todas deben completarse
Promise.all([promise1, promise2, promise3])
    .then(resultados => console.log(resultados))
    .catch(error => console.log("Una falló:", error));

// 🏃 Promise.race - La primera en completarse
Promise.race([promise1, promise2])
    .then(resultado => console.log("Primera:", resultado));

// 🔥 Promise.allSettled - Espera todas, sin importar resultado (ES2020)
Promise.allSettled([promise1, promise2])
    .then(resultados => {
        resultados.forEach(resultado => {
            if (resultado.status === 'fulfilled') {
                console.log('Éxito:', resultado.value);
            } else {
                console.log('Error:', resultado.reason);
            }
        });
    });
```

### 🎨 **Modules (ES6)**

```javascript
// 📤 Export (archivo: utils.js)
export const PI = 3.14159;
export function sumar(a, b) { return a + b; }
export default function multiplicar(a, b) { return a * b; }

// Export todo junto
const utils = { PI, sumar };
export default utils;

// 📥 Import (archivo: app.js)
import multiplicar from './utils.js';           // Default import
import { PI, sumar } from './utils.js';         // Named imports
import multiplicar, { PI, sumar } from './utils.js'; // Ambos
import * as utils from './utils.js';            // Todo como objeto
import('./utils.js').then(module => {          // Dynamic import 🔥 ES2020
    console.log(module.PI);
});

// 🎯 Re-export
export { sumar, restar } from './matematicas.js';
export { default as Calculadora } from './Calculadora.js';
```

### 🎪 **Generators (ES6)**

```javascript
// 🎭 Generator function
function* contador() {
    let i = 0;
    while (true) {
        yield i++;
    }
}

const gen = contador();
gen.next().value;  // 0
gen.next().value;  // 1
gen.next().value;  // 2

// 🎯 Generator con return
function* fibonacci() {
    let a = 0, b = 1;
    while (true) {
        yield a;
        [a, b] = [b, a + b];
    }
}

// 🔄 Iterar generator
for (const num of fibonacci()) {
    if (num > 100) break;
    console.log(num);
}

// 🎨 Generator con datos externos
function* procesamientoDatos() {
    const dato1 = yield "Dame el primer dato";
    const dato2 = yield "Dame el segundo dato";
    return `Resultado: ${dato1 + dato2}`;
}

const proc = procesamientoDatos();
proc.next();           // {value: "Dame el primer dato", done: false}
proc.next(10);         // {value: "Dame el segundo dato", done: false}
const final = proc.next(20); // {value: "Resultado: 30", done: true}
```

---

## 🎯 **Patrones y Mejores Prácticas**

### 🏗️ **Patrones Comunes**

```javascript
// 🎭 Module Pattern
const MiModulo = (function() {
    let variablePrivada = 0;
    
    function funcionPrivada() {
        return "privado";
    }
    
    return {
        funcionPublica() {
            return ++variablePrivada;
        },
        get valor() {
            return variablePrivada;
        }
    };
})();

// 🏭 Factory Pattern
function crearUsuario(nombre, tipo = 'normal') {
    const usuario = {
        nombre,
        tipo,
        permisos: tipo === 'admin' ? ['leer', 'escribir', 'eliminar'] : ['leer']
    };
    
    return Object.freeze(usuario); // Inmutable
}

// 🎯 Observer Pattern (simple)
class EventEmitter {
    constructor() {
        this.eventos = {};
    }
    
    on(evento, callback) {
        if (!this.eventos[evento]) {
            this.eventos[evento] = [];
        }
        this.eventos[evento].push(callback);
    }
    
    emit(evento, datos) {
        if (this.eventos[evento]) {
            this.eventos[evento].forEach(callback => callback(datos));
        }
    }
    
    off(evento, callback) {
        if (this.eventos[evento]) {
            this.eventos[evento] = this.eventos[evento].filter(cb => cb !== callback);
        }
    }
}

// 🔄 Mixin Pattern
const Volador = {
    volar() {
        console.log(`${this.nombre} está volando`);
    }
};

const Nadador = {
    nadar() {
        console.log(`${this.nombre} está nadando`);
    }
};

// Aplicar mixins
Object.assign(Ave.prototype, Volador);
Object.assign(Pez.prototype, Nadador);
Object.assign(Pato.prototype, Volador, Nadador); // Pato puede volar y nadar
```

### ✅ **Mejores Prácticas**

```javascript
// 🎯 Naming Conventions
const API_URL = 'https://api.com';          // ✅ Constantes: MAYÚSCULAS
const usuarioActivo = getCurrentUser();     // ✅ Variables: camelCase
const _datoPrivado = 'secreto';             // ✅ Privado: _underscore

function calcularImpuestos() {}             // ✅ Funciones: verbo + sustantivo
function esUsuarioValido() {}               // ✅ Booleanos: es/tiene/puede + ?

class ProductoManager {}                    // ✅ Clases: PascalCase

// 🧹 Código Limpio
// ❌ Malo
function calc(x, y, z) {
    if (z == 1) return x + y;
    else if (z == 2) return x - y;
    else return 0;
}

// ✅ Bueno
function calcularOperacion(primerNumero, segundoNumero, tipoOperacion) {
    const OPERACIONES = {
        SUMA: 1,
        RESTA: 2
    };
    
    switch (tipoOperacion) {
        case OPERACIONES.SUMA:
            return primerNumero + segundoNumero;
        case OPERACIONES.RESTA:
            return primerNumero - segundoNumero;
        default:
            throw new Error('Operación no válida');
    }
}

// 🎯 Funciones Puras (sin efectos secundarios)
// ❌ Impura
let contador = 0;
function incrementar() {
    return ++contador; // Modifica variable externa
}

// ✅ Pura
function incrementar(valor) {
    return valor + 1; // Solo depende de parámetros
}

// 🔄 Inmutabilidad
// ❌ Muta el objeto original
function actualizarUsuario(usuario, cambios) {
    usuario.nombre = cambios.nombre;
    return usuario;
}

// ✅ Retorna nuevo objeto
function actualizarUsuario(usuario, cambios) {
    return {
        ...usuario,
        ...cambios
    };
}
```

---

## 💡 **Tips de Rendimiento**

```javascript
// ⚡ Loop optimizations
// ❌ Lento - Calcula length en cada iteración
for (let i = 0; i < array.length; i++) {}

// ✅ Rápido - Cachea la longitud
for (let i = 0, len = array.length; i < len; i++) {}

// ✅ Más rápido aún para arrays grandes
let i = array.length;
while (i--) {
    // Procesar array[i]
}

// 🎯 Object lookup vs Switch
// ❌ Múltiples if-else
function getTipo(codigo) {
    if (codigo === 'A') return 'Admin';
    if (codigo === 'U') return 'Usuario';
    if (codigo === 'G') return 'Invitado';
}

// ✅ Object lookup - Más rápido
const TIPOS = {
    'A': 'Admin',
    'U': 'Usuario', 
    'G': 'Invitado'
};
function getTipo(codigo) {
    return TIPOS[codigo] || 'Desconocido';
}

// 🔍 Usar Map para keys no-string
const cache = new Map();
cache.set(1, 'uno');
cache.set('1', 'string uno'); // Diferentes keys

// ⚡ Debouncing para eventos frecuentes
function debounce(func, delay) {
    let timeoutId;
    return function(...args) {
        clearTimeout(timeoutId);
        timeoutId = setTimeout(() => func.apply(this, args), delay);
    };
}

const buscarDB = debounce(query => {
    // Búsqueda costosa
}, 300);

// 🎯 Throttling para scroll/resize
function throttle(func, limit) {
    let inThrottle;
    return function(...args) {
        if (!inThrottle) {
            func.apply(this, args);
            inThrottle = true;
            setTimeout(() => inThrottle = false, limit);
        }
    };
}
```

---

## 🎨 **Snippets Útiles**

```javascript
// 🎲 Número aleatorio entre min y max (inclusive)
const randomBetween = (min, max) => Math.floor(Math.random() * (max - min + 1)) + min;

// 🎯 Eliminar duplicados de array
const unique = arr => [...new Set(arr)];
const uniqueBy = (arr, key) => arr.filter((item, index, self) => 
    index === self.findIndex(t => t[key] === item[key])
);

// 🔄 Chunk array en grupos
const chunk = (arr, size) => 
    Array.from({ length: Math.ceil(arr.length / size) }, (_, i) =>
        arr.slice(i * size, i * size + size)
    );

// 📊 Agrupar array por propiedad
const groupBy = (arr, key) => 
    arr.reduce((groups, item) => {
        const group = item[key];
        groups[group] = groups[group] || [];
        groups[group].push(item);
        return groups;
    }, {});

// 🎯 Formatear números
const formatNumber = (num) => new Intl.NumberFormat('es-ES').format(num);
const formatCurrency = (num) => new Intl.NumberFormat('es-ES', {
    style: 'currency',
    currency: 'EUR'
}).format(num);

// ⏱️ Medir tiempo de ejecución
const timeFunction = (fn, ...args) => {
    const start = performance.now();
    const result = fn(...args);
    const end = performance.now();
    console.log(`Función tardó ${end - start} ms`);
    return result;
};

// 🎪 Capitalizar string
const capitalize = str => str.charAt(0).toUpperCase() + str.slice(1).toLowerCase();
const capitalizeWords = str => str.replace(/\w\S*/g, capitalize);

// 🔍 Deep clone de objetos
const deepClone = obj => JSON.parse(JSON.stringify(obj)); // Simple pero limitado
const deepCloneAdvanced = obj => structuredClone(obj); // 🔥 Nuevo API nativo

// 🎯 Validar email (básico)
const isValidEmail = email => /^[^\s@]+@[^\s@]+\.[^\s@]+$/.test(email);

// 🌈 Generar color aleatorio
const randomColor = () => `#${Math.floor(Math.random()*16777215).toString(16)}`;

// 📱 Detectar dispositivo móvil
const isMobile = () => /Android|webOS|iPhone|iPad|iPod|BlackBerry|IEMobile|Opera Mini/i.test(navigator.userAgent);

// 🎭 Funciones de utilidad funcional
const pipe = (...fns) => (value) => fns.reduce((acc, fn) => fn(acc), value);
const compose = (...fns) => (value) => fns.reduceRight((acc, fn) => fn(acc), value);

// Ejemplo de uso:
const procesarTexto = pipe(
    str => str.trim(),
    str => str.toLowerCase(),
    str => str.replace(/\s+/g, '-')
);

procesarTexto("  Hola Mundo  "); // "hola-mundo"
```

---

## 🎉 **¡Cheatsheet Completado!**

**🎯 Recuerda:**
- Este cheatsheet es tu **referencia rápida** para el día a día
- Úsalo junto con la documentación oficial para casos complejos
- **Practica** cada concepto con ejemplos reales
- **Evoluciona** tu código: de principiante a avanzado gradualmente

**💡 Próximos pasos:**
1. **Experimenta** con cada snippet en tu consola
2. **Combina** diferentes técnicas en proyectos reales
3. **Profundiza** en los temas que más te interesen
4. **Comparte** tu conocimiento con otros desarrolladores

```javascript
// 🚀 Tu viaje como programador continúa
console.log("📝 Cheatsheet dominado - ¡Hora de crear cosas increíbles!");
```

---

**📌 Este cheatsheet es un documento complementario al libro principal de Lógica de Programación.**

---

[🔙 **Volver al Libro Principal**](./LOGICA-PROGRAMACION-LIBRO.md) | [🏠 **Índice General**](../../../README.md) | [📚 **Navegación**](../../../NAVEGACION-DOCUMENTOS.md)
