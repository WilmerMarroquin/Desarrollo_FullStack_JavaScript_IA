[🏠 **Volver al Índice de Navegación**](../../../NAVEGACION-DOCUMENTOS.md)

---

# 📝 **Estructuras de Datos - Cheatsheet Visual**

> **📝 "Una referencia rápida vale más que mil tutoriales cuando estás manipulando datos. Aquí tienes tu guía definitiva de estructuras de datos en JavaScript."**

**📖 Tema 2 - Referencia Visual** • **⏱️ Consulta rápida** • **🎓 Todos los niveles**

---

## 🎨 **Guía de Uso del Cheatsheet**

```javascript
// 🎯 Cómo usar este cheatsheet:
const guiaUso = {
    purpose: "📋 Referencia rápida mientras programas con estructuras de datos",
    usage: "🔍 Busca por sesión o usa Ctrl+F para encontrar métodos específicos",
    level: "📈 Desde arrays básicos hasta algoritmos avanzados",
    format: "💻 Código copiable y ejemplos prácticos"
};

// 🌈 Leyenda de símbolos:
// ✅ Recomendado / Mejor práctica
// ❌ Evitar / Ineficiente  
// 🔥 Moderno / ES6+
// ⚡ Alta performance
// 🐛 Cuidado con edge cases
// 💡 Tip importante
// 🎯 Caso de uso común
```

---

## 🧭 **NAVEGACIÓN POR SESIONES**

### 📚 **Índice de Sesiones**

| **📊 SESIÓN** | **🎯 CONTENIDO** | **⏱️ CONSULTA** |
|:--------------|:-----------------|:----------------|
| [**SESIÓN 1**](#sesión-1-📊-arrays-esenciales) | 📊 Arrays Esenciales | Métodos básicos, creación, acceso |
| [**SESIÓN 2**](#sesión-2-⚡-métodos-funcionales) | ⚡ Métodos Funcionales | map, filter, reduce, forEach |
| [**SESIÓN 3**](#sesión-3-🏛️-objetos-y-propiedades) | 🏛️ Objetos y Propiedades | Creación, acceso, métodos de Object |
| [**SESIÓN 4**](#sesión-4-🛠️-estructuras-avanzadas) | 🛠️ Estructuras Avanzadas | Map, Set, WeakMap, WeakSet |
| [**SESIÓN 5**](#sesión-5-📈-algoritmos-búsqueda) | 📈 Algoritmos Búsqueda | Linear, binary, interpolation |
| [**SESIÓN 6**](#sesión-6-🔄-algoritmos-ordenamiento) | 🔄 Algoritmos Ordenamiento | Bubble, quick, merge sort |
| [**SESIÓN 7**](#sesión-7-🏗️-estructuras-personalizadas) | 🏗️ Estructuras Personalizadas | Stack, Queue, Trees |
| [**SESIÓN 8**](#sesión-8-⚡-optimización-performance) | ⚡ Optimización Performance | Big O, memoización, cache |

---

## **SESIÓN 1: 📊 Arrays Esenciales**

### 🎯 **Creación y Declaración**

```javascript
// 📊 CREACIÓN DE ARRAYS
const vacio = [];                           // ✅ Array vacío
const numeros = [1, 2, 3, 4, 5];           // ✅ Array literal
const mixto = [1, "texto", true, null];    // ✅ Tipos mixtos
const repetido = Array(5).fill(0);         // [0, 0, 0, 0, 0]
const secuencia = Array.from({length: 5}, (_, i) => i); // [0,1,2,3,4]

// 🔥 MÉTODOS MODERNOS DE CREACIÓN
const desde = Array.from("hola");          // ['h','o','l','a']
const spread = [...Array(3).keys()];       // [0, 1, 2]
const of = Array.of(1, 2, 3);             // [1, 2, 3] vs Array(3)
```

### 🎯 **Acceso y Modificación**

```javascript
const frutas = ['🍎', '🍌', '🍊', '🍇'];

// 📍 ACCESO POR ÍNDICE
frutas[0]           // '🍎' (primer elemento)
frutas[-1]          // undefined (JS no soporta índices negativos)
frutas.at(-1)       // '🍇' 🔥 ES2022 - último elemento
frutas.at(-2)       // '🍊' 🔥 penúltimo elemento

// 📝 MODIFICACIÓN
frutas[1] = '🥝';   // Cambia 🍌 por 🥝
frutas[10] = '🥭'; // Crea espacios vacíos (sparse array) 🐛

// 📏 PROPIEDADES
frutas.length       // 4 (longitud)
frutas.length = 2   // Trunca array a ['🍎', '🥝'] 🐛
```

### 🎯 **Métodos de Modificación (Mutating)**

```javascript
const lista = [1, 2, 3];

// ➕ AGREGAR ELEMENTOS
lista.push(4, 5);        // [1,2,3,4,5] - Al final
lista.unshift(0);        // [0,1,2,3,4,5] - Al inicio
lista.splice(2, 0, 1.5); // [0,1,1.5,2,3,4,5] - En posición específica

// ➖ REMOVER ELEMENTOS  
lista.pop();             // Remueve y devuelve último: 5
lista.shift();           // Remueve y devuelve primero: 0
lista.splice(2, 1);      // Remueve 1 elemento desde posición 2

// 🔄 REORDENAR
lista.reverse();         // ❌ Muta el array original
lista.sort();            // ❌ Muta y ordena alfabéticamente por defecto
lista.sort((a, b) => a - b); // ✅ Orden numérico ascendente
```

### 🎯 **Métodos de Consulta (Non-mutating)**

```javascript
const datos = [1, 2, 3, 4, 5, 2];

// 🔍 BÚSQUEDA
datos.indexOf(2);        // 1 (primera ocurrencia)
datos.lastIndexOf(2);    // 5 (última ocurrencia)
datos.includes(3);       // true 🔥 ES7
datos.find(x => x > 3);  // 4 (primer elemento que cumple)
datos.findIndex(x => x > 3); // 3 (índice del elemento)

// 🧪 VERIFICACIÓN
datos.every(x => x > 0); // true (todos cumplen condición)
datos.some(x => x > 4);  // true (al menos uno cumple)

// ✂️ EXTRACCIÓN (No mutating)
datos.slice(1, 3);       // [2, 3] (desde índice 1 hasta 3, no inclusive)
datos.slice(-2);         // [5, 2] (últimos 2 elementos)
[...datos];              // 🔥 Copia superficial con spread
```

### 💡 **Casos de Uso Comunes**

```javascript
// 🎯 ENCONTRAR ELEMENTO EN ARRAY DE OBJETOS
const usuarios = [
    {id: 1, nombre: 'Ana'},
    {id: 2, nombre: 'Carlos'},
    {id: 3, nombre: 'Elena'}
];

const usuario = usuarios.find(u => u.id === 2);        // {id: 2, nombre: 'Carlos'}
const existe = usuarios.some(u => u.nombre === 'Ana'); // true
const indice = usuarios.findIndex(u => u.id === 3);    // 2

// 🎯 ELIMINAR DUPLICADOS
const conDuplicados = [1, 2, 2, 3, 3, 4];
const unicos = [...new Set(conDuplicados)];            // [1, 2, 3, 4] ✅

// 🎯 ÚLTIMO ELEMENTO SEGURO
const obtenerUltimo = arr => arr[arr.length - 1];      // ✅ Método clásico
const ultimo = arr => arr.at(-1);                      // 🔥 Método moderno

// 🎯 VERIFICAR SI ES ARRAY
Array.isArray([1, 2, 3]);   // true ✅
Array.isArray('string');    // false
```

---

## **SESIÓN 2: ⚡ Métodos Funcionales**

### 🎯 **map() - Transformar Elementos**

```javascript
const numeros = [1, 2, 3, 4, 5];

// 🔄 TRANSFORMACIONES BÁSICAS
numeros.map(x => x * 2);              // [2, 4, 6, 8, 10]
numeros.map(x => x ** 2);             // [1, 4, 9, 16, 25] (cuadrados)
numeros.map((num, indice) => ({       // Objetos con índice
    numero: num,
    posicion: indice
}));

// 🎯 CASOS REALES
const productos = [
    {nombre: 'Laptop', precio: 1000},
    {nombre: 'Mouse', precio: 25}
];

// Extraer solo nombres
const nombres = productos.map(p => p.nombre);          // ['Laptop', 'Mouse']
// Aplicar descuento
const conDescuento = productos.map(p => ({
    ...p,
    precio: p.precio * 0.9
}));

// 🔥 CHAINING (Encadenamiento)
numeros
    .map(x => x * 2)        // [2, 4, 6, 8, 10]
    .map(x => x + 1)        // [3, 5, 7, 9, 11]
    .map(x => `#${x}`);     // ['#3', '#5', '#7', '#9', '#11']
```

### 🎯 **filter() - Filtrar Elementos**

```javascript
const numeros = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10];

// 🔍 FILTROS BÁSICOS
numeros.filter(x => x > 5);           // [6, 7, 8, 9, 10]
numeros.filter(x => x % 2 === 0);     // [2, 4, 6, 8, 10] (pares)
numeros.filter(x => x % 2 !== 0);     // [1, 3, 5, 7, 9] (impares)

// 🎯 FILTROS COMPLEJOS
const usuarios = [
    {nombre: 'Ana', edad: 25, activo: true},
    {nombre: 'Carlos', edad: 17, activo: false},
    {nombre: 'Elena', edad: 30, activo: true}
];

// Usuarios adultos activos
const adultosActivos = usuarios.filter(u => u.edad >= 18 && u.activo);

// Filtrar y transformar
const nombresAdultos = usuarios
    .filter(u => u.edad >= 18)         // Solo adultos
    .map(u => u.nombre.toUpperCase()); // ['ANA', 'ELENA']

// 🔥 FILTRAR VALORES FALSY
const datos = [0, 1, '', 'texto', null, 'hola', undefined, false, true];
const soloTruthy = datos.filter(Boolean);  // [1, 'texto', 'hola', true] ✅
```

### 🎯 **reduce() - Acumular/Reducir**

```javascript
const numeros = [1, 2, 3, 4, 5];

// 📊 OPERACIONES BÁSICAS
numeros.reduce((suma, num) => suma + num, 0);          // 15 (suma)
numeros.reduce((producto, num) => producto * num, 1);  // 120 (producto)
numeros.reduce((max, num) => Math.max(max, num));      // 5 (máximo)

// 🎯 CASOS AVANZADOS
const texto = ['H', 'o', 'l', 'a'];
const palabra = texto.reduce((acc, letra) => acc + letra, ''); // 'Hola'

// Contar ocurrencias
const frutas = ['🍎', '🍌', '🍎', '🍊', '🍌', '🍎'];
const contador = frutas.reduce((acc, fruta) => {
    acc[fruta] = (acc[fruta] || 0) + 1;
    return acc;
}, {});  // {'🍎': 3, '🍌': 2, '🍊': 1}

// Agrupar por propiedad
const personas = [
    {nombre: 'Ana', ciudad: 'Madrid'},
    {nombre: 'Carlos', ciudad: 'Barcelona'},
    {nombre: 'Elena', ciudad: 'Madrid'}
];

const agrupados = personas.reduce((acc, persona) => {
    const ciudad = persona.ciudad;
    if (!acc[ciudad]) acc[ciudad] = [];
    acc[ciudad].push(persona);
    return acc;
}, {});

// 🔥 FLATTEN ARRAY
const anidado = [[1, 2], [3, 4], [5, 6]];
const plano = anidado.reduce((acc, arr) => acc.concat(arr), []); // [1,2,3,4,5,6]
// O mejor con flat(): anidado.flat() 🔥 ES2019
```

### 🎯 **forEach() - Iterar sin Retorno**

```javascript
const tareas = ['Leer', 'Escribir', 'Programar'];

// 🔄 ITERACIÓN BÁSICA
tareas.forEach(tarea => console.log(`📋 ${tarea}`));

// Con índice
tareas.forEach((tarea, indice) => {
    console.log(`${indice + 1}. ${tarea}`);
});

// 🚨 NO hacer esto (mejor usar map)
const resultado = [];
numeros.forEach(num => resultado.push(num * 2)); // ❌ Efecto secundario

// ✅ Mejor así
const resultado = numeros.map(num => num * 2);   // ✅ Funcional puro
```

### 💡 **Combinaciones Poderosas**

```javascript
// 🎯 PIPELINE DE TRANSFORMACIÓN
const ventas = [
    {producto: 'Laptop', precio: 1000, cantidad: 2},
    {producto: 'Mouse', precio: 25, cantidad: 10},
    {producto: 'Teclado', precio: 75, cantidad: 5}
];

const resumen = ventas
    .map(v => ({...v, total: v.precio * v.cantidad}))    // Calcular totales
    .filter(v => v.total > 100)                          // Solo ventas > 100
    .reduce((suma, v) => suma + v.total, 0);             // Suma total

// 🎯 BÚSQUEDA AVANZADA
const encontrarYTransformar = (array, condicion, transformador) =>
    array
        .filter(condicion)
        .map(transformador);

const usuarios = [{nombre: 'Ana', edad: 25}, {nombre: 'Carlos', edad: 17}];
const adultosMayusculas = encontrarYTransformar(
    usuarios,
    u => u.edad >= 18,
    u => u.nombre.toUpperCase()
); // ['ANA']
```

---

## **SESIÓN 3: 🏛️ Objetos y Propiedades**

### 🎯 **Creación y Declaración**

```javascript
// 🏗️ CREACIÓN DE OBJETOS
const vacio = {};                           // ✅ Objeto vacío
const literal = {                          // ✅ Literal
    nombre: 'Ana',
    edad: 25,
    'clave-especial': 'valor'              // Claves con caracteres especiales
};

const dinamico = {
    [variable]: 'valor',                   // 🔥 Propiedades computadas
    ['prop_' + numero]: 'dinámico'
};

// 🔥 SHORTHAND PROPERTIES (ES6)
const nombre = 'Carlos';
const edad = 30;
const persona = {nombre, edad};            // {nombre: 'Carlos', edad: 30}

// 🎯 CONSTRUCTOR Y PROTOTYPE
const obj = new Object();                  // ❌ Menos eficiente
const obj2 = Object.create(null);          // ✅ Sin prototype
```

### 🎯 **Acceso a Propiedades**

```javascript
const usuario = {
    nombre: 'Ana',
    edad: 25,
    direccion: {
        calle: 'Main St',
        ciudad: 'Madrid'
    },
    'dato-especial': 'valor'
};

// 📍 ACCESO CON DOT NOTATION
usuario.nombre              // 'Ana' ✅ Más limpio
usuario.direccion.ciudad    // 'Madrid'

// 📍 ACCESO CON BRACKET NOTATION
usuario['nombre']           // 'Ana'
usuario['dato-especial']    // 'valor' (necesario para claves especiales)
const prop = 'edad';
usuario[prop]               // 25 (acceso dinámico)

// 🔥 OPTIONAL CHAINING (ES2020)
usuario.direccion?.codigo   // undefined (no error si no existe)
usuario.contacto?.telefono?.movil; // undefined (navegación segura)

// 🔥 NULLISH COALESCING (??)
const telefono = usuario.telefono ?? 'No disponible';  // Si es null/undefined
const nombre = usuario.nombre || 'Anónimo';             // Si es falsy
```

### 🎯 **Métodos de Object**

```javascript
const producto = {
    nombre: 'Laptop',
    precio: 1000,
    categoria: 'Electrónicos'
};

// 🔑 TRABAJAR CON CLAVES
Object.keys(producto);         // ['nombre', 'precio', 'categoria']
Object.values(producto);       // ['Laptop', 1000, 'Electrónicos']  
Object.entries(producto);      // [['nombre', 'Laptop'], ['precio', 1000], ...]

// 📊 INFORMACIÓN DEL OBJETO
Object.hasOwnProperty('nombre');           // true (método del objeto)
producto.hasOwnProperty('precio');         // true ✅
'categoria' in producto;                   // true (incluye prototype)

// 🔄 ITERACIÓN
for (const clave in producto) {            // Itera claves
    console.log(clave, producto[clave]);
}

for (const [clave, valor] of Object.entries(producto)) { // 🔥 ES6
    console.log(clave, valor);
}

// 📏 TAMAÑO
Object.keys(producto).length;              // 3 (número de propiedades)
```

### 🎯 **Clonado y Fusión**

```javascript
const original = {
    nombre: 'Ana',
    datos: {edad: 25, ciudad: 'Madrid'}
};

// 📋 COPIA SUPERFICIAL (Shallow Copy)
const copia1 = {...original};             // 🔥 Spread operator (ES6)
const copia2 = Object.assign({}, original); // Método clásico

// 🚨 PROBLEMA: Referencias compartidas
copia1.datos.edad = 30;                   // ¡Cambia también en original! 🐛

// 📋 COPIA PROFUNDA (Deep Copy)
const copiaProf = JSON.parse(JSON.stringify(original)); // ✅ Simple
// 🐛 Limitaciones: No copia funciones, dates, regex, etc.

// 🔄 FUSIÓN DE OBJETOS
const obj1 = {a: 1, b: 2};
const obj2 = {b: 3, c: 4};
const fusionado = {...obj1, ...obj2};     // {a: 1, b: 3, c: 4} (obj2 gana)

// 🎯 FUSIÓN PROFUNDA (Manual)
const fusionProfunda = (obj1, obj2) => {
    const resultado = {...obj1};
    for (const clave in obj2) {
        if (typeof obj2[clave] === 'object' && obj2[clave] !== null) {
            resultado[clave] = fusionProfunda(resultado[clave] || {}, obj2[clave]);
        } else {
            resultado[clave] = obj2[clave];
        }
    }
    return resultado;
};
```

### 🎯 **Destructuring Avanzado**

```javascript
const usuario = {
    nombre: 'Ana',
    edad: 25,
    direccion: {
        calle: 'Main St',
        ciudad: 'Madrid',
        pais: 'España'
    },
    hobbies: ['leer', 'nadar', 'programar']
};

// 🎯 DESTRUCTURING BÁSICO
const {nombre, edad} = usuario;           // nombre='Ana', edad=25

// 🏷️ RENOMBRAR VARIABLES
const {nombre: n, edad: e} = usuario;     // n='Ana', e=25

// 🎁 VALORES POR DEFECTO
const {telefono = 'No disponible'} = usuario; // telefono='No disponible'

// 🏗️ DESTRUCTURING ANIDADO
const {direccion: {ciudad, pais}} = usuario;  // ciudad='Madrid', pais='España'

// 📊 DESTRUCTURING EN ARRAYS
const {hobbies: [primero, segundo]} = usuario; // primero='leer', segundo='nadar'

// 🔄 REST EN OBJETOS
const {nombre, ...resto} = usuario;       // resto contiene todo excepto nombre

// 🎯 EN PARÁMETROS DE FUNCIÓN
const saludar = ({nombre, edad = 0}) => `Hola ${nombre}, tienes ${edad} años`;
saludar(usuario); // 'Hola Ana, tienes 25 años'
```

### 💡 **Patrones Útiles**

```javascript
// 🎯 TRANSFORMAR OBJETO
const precios = {laptop: 1000, mouse: 25, teclado: 75};

// Aplicar descuento a todos
const conDescuento = Object.fromEntries(
    Object.entries(precios).map(([producto, precio]) => 
        [producto, precio * 0.9]
    )
);

// 🎯 FILTRAR PROPIEDADES
const filtrarObj = (obj, condicion) =>
    Object.fromEntries(
        Object.entries(obj).filter(([clave, valor]) => condicion(clave, valor))
    );

const caros = filtrarObj(precios, (prod, precio) => precio > 50);

// 🎯 VALIDAR ESTRUCTURA
const validarUsuario = (obj) => {
    const requeridos = ['nombre', 'email', 'edad'];
    return requeridos.every(campo => campo in obj);
};

// 🎯 MERGE CONDICIONAL
const mergearSiExiste = (obj1, obj2) => ({
    ...obj1,
    ...Object.fromEntries(
        Object.entries(obj2).filter(([_, valor]) => valor != null)
    )
});
```

---

## **SESIÓN 4: 🛠️ Estructuras Avanzadas**

### 🎯 **Map - Mapas Clave-Valor**

```javascript
// 🗺️ CREACIÓN
const mapa = new Map();                    // ✅ Map vacío
const mapaInicial = new Map([              // Con valores iniciales
    ['clave1', 'valor1'],
    ['clave2', 'valor2']
]);

// 🔧 OPERACIONES BÁSICAS
mapa.set('nombre', 'Ana');                 // Agregar/actualizar
mapa.set(42, 'número como clave');         // ✅ Cualquier tipo de clave
mapa.set(true, 'boolean como clave');

mapa.get('nombre');                        // 'Ana' (obtener valor)
mapa.has('nombre');                        // true (verificar existencia)
mapa.delete('nombre');                     // true (eliminar, retorna success)
mapa.clear();                              // Vaciar completamente
mapa.size;                                 // 0 (tamaño)

// 🎯 VENTAJAS SOBRE OBJECTS
const objetoClave = {id: 1};
mapa.set(objetoClave, 'objeto como clave'); // ✅ Objetos como claves
mapa.set('size', 100);                     // ✅ No conflicto con propiedades nativas

// 🔄 ITERACIÓN
for (const [clave, valor] of mapa) {       // ✅ Iteración directa
    console.log(clave, valor);
}

mapa.forEach((valor, clave) => {           // forEach nativo
    console.log(clave, valor);
});

// 📊 CONVERSIONES
const objeto = Object.fromEntries(mapa);   // Map → Object
const mapaDesdeObj = new Map(Object.entries(objeto)); // Object → Map
const array = [...mapa];                   // Map → Array de pares
```

### 🎯 **Set - Colecciones Únicas**

```javascript
// 🎯 CREACIÓN
const conjunto = new Set();                // Set vacío
const conValores = new Set([1, 2, 3, 2, 1]); // [1, 2, 3] (automáticamente únicos)

// 🔧 OPERACIONES BÁSICAS
conjunto.add(1);                           // Agregar elemento
conjunto.add(2).add(3);                    // ✅ Chaineable
conjunto.has(2);                           // true (verificar)
conjunto.delete(1);                        // true (eliminar)
conjunto.clear();                          // Vaciar
conjunto.size;                             // 0 (tamaño)

// 🎯 CASOS DE USO COMUNES
const numeros = [1, 2, 2, 3, 3, 4, 5, 5];
const unicos = [...new Set(numeros)];     // [1, 2, 3, 4, 5] ✅ Eliminar duplicados

// 🧮 OPERACIONES DE CONJUNTOS
const setA = new Set([1, 2, 3, 4]);
const setB = new Set([3, 4, 5, 6]);

// Unión
const union = new Set([...setA, ...setB]); // [1, 2, 3, 4, 5, 6]

// Intersección
const interseccion = new Set([...setA].filter(x => setB.has(x))); // [3, 4]

// Diferencia
const diferencia = new Set([...setA].filter(x => !setB.has(x))); // [1, 2]

// 🔄 ITERACIÓN
for (const valor of conjunto) {            // Iteración directa
    console.log(valor);
}

conjunto.forEach(valor => {                // forEach nativo
    console.log(valor);
});
```

### 🎯 **WeakMap - Referencias Débiles**

```javascript
// 💾 CREACIÓN (solo objetos como claves)
const weakMap = new WeakMap();
const obj1 = {nombre: 'Ana'};
const obj2 = {nombre: 'Carlos'};

// 🔧 OPERACIONES (limitadas)
weakMap.set(obj1, 'datos privados');       // ✅ Solo objetos como claves
weakMap.get(obj1);                         // 'datos privados'
weakMap.has(obj1);                         // true
weakMap.delete(obj1);                      // true

// ❌ NO disponible: size, clear, iteración

// 🎯 CASOS DE USO: DATOS PRIVADOS
const datosPrivados = new WeakMap();

class Usuario {
    constructor(nombre) {
        this.nombre = nombre;
        datosPrivados.set(this, {
            password: 'secreto',
            intentosLogin: 0
        });
    }
    
    login(password) {
        const datos = datosPrivados.get(this);
        if (datos.password === password) {
            datos.intentosLogin = 0;
            return true;
        }
        datos.intentosLogin++;
        return false;
    }
}

// 🧹 GARBAGE COLLECTION AUTOMÁTICO
let usuario = new Usuario('Ana');
// Cuando usuario = null, los datos privados también se eliminan automáticamente
```

### 🎯 **WeakSet - Referencias Débiles de Objetos**

```javascript
// 🔗 CREACIÓN (solo objetos)
const weakSet = new WeakSet();
const obj1 = {id: 1};
const obj2 = {id: 2};

// 🔧 OPERACIONES (limitadas)
weakSet.add(obj1);                         // ✅ Agregar objeto
weakSet.has(obj1);                         // true
weakSet.delete(obj1);                      // true

// ❌ NO disponible: size, clear, iteración

// 🎯 CASOS DE USO: TRACKING DE OBJETOS
const objetosProcesados = new WeakSet();

function procesar(objeto) {
    if (objetosProcesados.has(objeto)) {
        console.log('Ya procesado');
        return;
    }
    
    // Procesar objeto...
    objetosProcesados.add(objeto);
    console.log('Procesado exitosamente');
}

// 🛡️ CONTROL DE ACCESO
const usuariosAutorizados = new WeakSet();

class SistemaSeguro {
    static autorizar(usuario) {
        usuariosAutorizados.add(usuario);
    }
    
    static accionSegura(usuario, accion) {
        if (!usuariosAutorizados.has(usuario)) {
            throw new Error('Acceso denegado');
        }
        return accion();
    }
}
```

### 💡 **Comparación y Cuándo Usar**

```javascript
// 🎯 GUÍA DE DECISIÓN
const guiaEstructuras = {
    Array: {
        cuando: "Lista ordenada, acceso por índice, métodos funcionales",
        ejemplo: "Lista de tareas, carrousel de imágenes"
    },
    
    Object: {
        cuando: "Pares clave-valor con claves string, estructura conocida",
        ejemplo: "Configuración, datos de formulario"
    },
    
    Map: {
        cuando: "Claves de cualquier tipo, iteración frecuente, tamaño dinámico",
        ejemplo: "Cache, contadores, relaciones objeto-valor"
    },
    
    Set: {
        cuando: "Valores únicos, operaciones de conjunto",
        ejemplo: "Tags únicos, IDs de elementos seleccionados"
    },
    
    WeakMap: {
        cuando: "Metadatos de objetos, datos privados, evitar memory leaks",
        ejemplo: "Propiedades privadas, cache temporal"
    },
    
    WeakSet: {
        cuando: "Tracking de objetos, flags temporales",
        ejemplo: "Objetos procesados, control de acceso"
    }
};

// 🎯 PERFORMANCE COMPARISON
const performanceTest = {
    busqueda: {
        Array: "O(n) - Linear search",
        Object: "O(1) - Hash lookup", 
        Map: "O(1) - Hash lookup",
        Set: "O(1) - Hash lookup"
    },
    
    insercion: {
        Array: "O(1) al final, O(n) al inicio",
        Object: "O(1)",
        Map: "O(1)",
        Set: "O(1)"
    }
};
```

---

[🔜 **Continúa con SESIÓN 5: Algoritmos de Búsqueda**](#sesión-5-📈-algoritmos-búsqueda)

---

## **SESIÓN 5: 📈 Algoritmos de Búsqueda**

### 🎯 **Búsqueda Lineal (Linear Search)**

```javascript
// 🔍 BÚSQUEDA BÁSICA - O(n)
const busquedaLineal = (array, objetivo) => {
    for (let i = 0; i < array.length; i++) {
        if (array[i] === objetivo) {
            return i;  // Retorna índice
        }
    }
    return -1;  // No encontrado
};

// 🔥 VERSIÓN MODERNA CON findIndex
const buscarModerno = (array, condicion) => 
    array.findIndex(condicion);  // ✅ Más legible

// 🎯 BÚSQUEDA EN OBJETOS
const usuarios = [
    {id: 1, nombre: 'Ana'},
    {id: 2, nombre: 'Carlos'}
];

const buscarPorId = (array, id) => 
    array.find(item => item.id === id);  // Retorna objeto completo

const buscarIndiceId = (array, id) => 
    array.findIndex(item => item.id === id);  // Retorna índice

// 🚀 BÚSQUEDA MÚLTIPLE
const buscarTodos = (array, condicion) => 
    array.filter(condicion);  // Todos los que cumplen

// Ejemplo: Encontrar todos los adultos
const adultos = usuarios.filter(u => u.edad >= 18);
```

### 🎯 **Búsqueda Binaria (Binary Search)**

```javascript
// 📈 BÚSQUEDA BINARIA - O(log n) ⚡ REQUIERE ARRAY ORDENADO
const busquedaBinaria = (array, objetivo) => {
    let inicio = 0;
    let fin = array.length - 1;
    
    while (inicio <= fin) {
        const medio = Math.floor((inicio + fin) / 2);
        
        if (array[medio] === objetivo) {
            return medio;  // ✅ Encontrado
        }
        
        if (array[medio] < objetivo) {
            inicio = medio + 1;  // Buscar en mitad derecha
        } else {
            fin = medio - 1;     // Buscar en mitad izquierda
        }
    }
    
    return -1;  // No encontrado
};

// 🎯 VERSIÓN RECURSIVA
const busquedaBinariaRecursiva = (array, objetivo, inicio = 0, fin = array.length - 1) => {
    if (inicio > fin) return -1;
    
    const medio = Math.floor((inicio + fin) / 2);
    
    if (array[medio] === objetivo) return medio;
    
    return array[medio] < objetivo 
        ? busquedaBinariaRecursiva(array, objetivo, medio + 1, fin)
        : busquedaBinariaRecursiva(array, objetivo, inicio, medio - 1);
};

// 🎯 ENCONTRAR POSICIÓN DE INSERCIÓN
const posicionInsercion = (array, valor) => {
    let inicio = 0;
    let fin = array.length;
    
    while (inicio < fin) {
        const medio = Math.floor((inicio + fin) / 2);
        if (array[medio] < valor) {
            inicio = medio + 1;
        } else {
            fin = medio;
        }
    }
    
    return inicio;  // Posición donde insertar para mantener orden
};
```

### 🎯 **Búsquedas Especializadas**

```javascript
// 🔄 BÚSQUEDA INTERPOLADA - O(log log n) para datos uniformemente distribuidos
const busquedaInterpolada = (array, objetivo) => {
    let inicio = 0;
    let fin = array.length - 1;
    
    while (inicio <= fin && objetivo >= array[inicio] && objetivo <= array[fin]) {
        if (inicio === fin) {
            return array[inicio] === objetivo ? inicio : -1;
        }
        
        // Estimación inteligente de posición
        const pos = inicio + Math.floor(
            ((objetivo - array[inicio]) / (array[fin] - array[inicio])) * (fin - inicio)
        );
        
        if (array[pos] === objetivo) return pos;
        
        if (array[pos] < objetivo) {
            inicio = pos + 1;
        } else {
            fin = pos - 1;
        }
    }
    
    return -1;
};

// 🎯 BÚSQUEDA TERNARIA - O(log₃ n)
const busquedaTernaria = (array, objetivo) => {
    let inicio = 0;
    let fin = array.length - 1;
    
    while (inicio <= fin) {
        const mid1 = inicio + Math.floor((fin - inicio) / 3);
        const mid2 = fin - Math.floor((fin - inicio) / 3);
        
        if (array[mid1] === objetivo) return mid1;
        if (array[mid2] === objetivo) return mid2;
        
        if (objetivo < array[mid1]) {
            fin = mid1 - 1;
        } else if (objetivo > array[mid2]) {
            inicio = mid2 + 1;
        } else {
            inicio = mid1 + 1;
            fin = mid2 - 1;
        }
    }
    
    return -1;
};

// 🎯 BÚSQUEDA CON HASH - O(1) promedio ⚡
const crearIndiceHash = (array, obtenerClave) => {
    const indice = new Map();
    array.forEach((elemento, i) => {
        const clave = obtenerClave(elemento);
        if (!indice.has(clave)) {
            indice.set(clave, []);
        }
        indice.get(clave).push(i);
    });
    return indice;
};

// Uso del índice hash
const productos = [{id: 1, nombre: 'Laptop'}, {id: 2, nombre: 'Mouse'}];
const indicePorId = crearIndiceHash(productos, p => p.id);
const buscarPorHash = (indice, clave) => indice.get(clave) || [];
```

### 💡 **Comparación de Performance**

```javascript
// 📊 BENCHMARK DE ALGORITMOS
const compararBusquedas = (array, objetivo) => {
    const arrayOrdenado = [...array].sort((a, b) => a - b);
    
    // Linear Search
    console.time('Lineal');
    const resultLineal = busquedaLineal(array, objetivo);
    console.timeEnd('Lineal');
    
    // Binary Search (requiere array ordenado)
    console.time('Binaria');
    const resultBinaria = busquedaBinaria(arrayOrdenado, objetivo);
    console.timeEnd('Binaria');
    
    // Métodos nativos
    console.time('indexOf');
    const resultIndexOf = array.indexOf(objetivo);
    console.timeEnd('indexOf');
    
    return { resultLineal, resultBinaria, resultIndexOf };
};

// 🎯 CUÁNDO USAR CADA UNO
const guiaBusqueda = {
    lineal: {
        usar: "Arrays pequeños (<100), datos no ordenados, búsqueda única",
        complejidad: "O(n)",
        ventajas: ["Funciona con cualquier array", "Simple de implementar"]
    },
    
    binaria: {
        usar: "Arrays grandes ordenados, búsquedas frecuentes",
        complejidad: "O(log n)",
        ventajas: ["Muy rápida", "Escalable"],
        requisito: "Array debe estar ordenado"
    },
    
    hash: {
        usar: "Búsquedas muy frecuentes, datos que no cambian mucho",
        complejidad: "O(1) promedio",
        ventajas: ["Más rápida posible", "Múltiples búsquedas eficientes"],
        desventaja: "Requiere pre-procesamiento"
    }
};
```

---

## **SESIÓN 6: 🔄 Algoritmos de Ordenamiento**

### 🎯 **Bubble Sort - Ordenamiento Burbuja**

```javascript
// 🫧 BUBBLE SORT - O(n²) - Solo para aprender
const bubbleSort = (array) => {
    const arr = [...array];  // ✅ No mutar original
    const n = arr.length;
    
    for (let i = 0; i < n - 1; i++) {
        let intercambio = false;
        
        for (let j = 0; j < n - i - 1; j++) {
            if (arr[j] > arr[j + 1]) {
                // Intercambiar elementos
                [arr[j], arr[j + 1]] = [arr[j + 1], arr[j]];  // 🔥 Destructuring swap
                intercambio = true;
            }
        }
        
        // ⚡ Optimización: Si no hubo intercambios, ya está ordenado
        if (!intercambio) break;
    }
    
    return arr;
};

// 🎯 USO: Solo para arrays muy pequeños o con fines educativos
console.log(bubbleSort([64, 34, 25, 12, 22, 11, 90]));
```

### 🎯 **Quick Sort - Ordenamiento Rápido**

```javascript
// ⚡ QUICK SORT - O(n log n) promedio, O(n²) peor caso
const quickSort = (array) => {
    if (array.length <= 1) return array;
    
    const pivot = array[Math.floor(array.length / 2)];  // Elemento pivote
    const menores = [];
    const iguales = [];
    const mayores = [];
    
    for (const elemento of array) {
        if (elemento < pivot) {
            menores.push(elemento);
        } else if (elemento > pivot) {
            mayores.push(elemento);
        } else {
            iguales.push(elemento);
        }
    }
    
    return [
        ...quickSort(menores),
        ...iguales,
        ...quickSort(mayores)
    ];
};

// 🎯 VERSIÓN OPTIMIZADA IN-PLACE
const quickSortInPlace = (arr, inicio = 0, fin = arr.length - 1) => {
    if (inicio < fin) {
        const pivotIndex = particion(arr, inicio, fin);
        quickSortInPlace(arr, inicio, pivotIndex - 1);
        quickSortInPlace(arr, pivotIndex + 1, fin);
    }
    return arr;
};

const particion = (arr, inicio, fin) => {
    const pivot = arr[fin];
    let i = inicio - 1;
    
    for (let j = inicio; j < fin; j++) {
        if (arr[j] <= pivot) {
            i++;
            [arr[i], arr[j]] = [arr[j], arr[i]];
        }
    }
    
    [arr[i + 1], arr[fin]] = [arr[fin], arr[i + 1]];
    return i + 1;
};
```

### 🎯 **Merge Sort - Ordenamiento por Mezcla**

```javascript
// 🔄 MERGE SORT - O(n log n) garantizado, estable
const mergeSort = (array) => {
    if (array.length <= 1) return array;
    
    const medio = Math.floor(array.length / 2);
    const izquierda = mergeSort(array.slice(0, medio));
    const derecha = mergeSort(array.slice(medio));
    
    return merge(izquierda, derecha);
};

const merge = (izq, der) => {
    const resultado = [];
    let i = 0, j = 0;
    
    // Mezclar arrays ordenados
    while (i < izq.length && j < der.length) {
        if (izq[i] <= der[j]) {
            resultado.push(izq[i]);
            i++;
        } else {
            resultado.push(der[j]);
            j++;
        }
    }
    
    // Agregar elementos restantes
    return resultado
        .concat(izq.slice(i))
        .concat(der.slice(j));
};

// 🎯 USO: Mejor para arrays grandes, garantiza O(n log n)
console.log(mergeSort([38, 27, 43, 3, 9, 82, 10]));
```

### 🎯 **Algoritmos Nativos de JavaScript**

```javascript
// 🔥 SORT NATIVO - Más eficiente y optimizado
const numeros = [40, 100, 1, 5, 25, 10];

// ❌ Sort por defecto (lexicográfico)
numeros.sort();  // [1, 10, 100, 25, 40, 5] 🐛 Orden alfabético

// ✅ Sort numérico
numeros.sort((a, b) => a - b);    // [1, 5, 10, 25, 40, 100] Ascendente
numeros.sort((a, b) => b - a);    // [100, 40, 25, 10, 5, 1] Descendente

// 🎯 ORDENAR OBJETOS
const personas = [
    {nombre: 'Ana', edad: 25},
    {nombre: 'Carlos', edad: 30},
    {nombre: 'Elena', edad: 20}
];

// Por edad ascendente
personas.sort((a, b) => a.edad - b.edad);

// Por nombre alfabético
personas.sort((a, b) => a.nombre.localeCompare(b.nombre));

// 🔥 ORDENAMIENTO MÚLTIPLE (por edad, luego por nombre)
personas.sort((a, b) => {
    if (a.edad !== b.edad) {
        return a.edad - b.edad;  // Primero por edad
    }
    return a.nombre.localeCompare(b.nombre);  // Luego por nombre
});

// ⚡ VERSIÓN NO MUTANTE (ES2023)
const ordenado = [...numeros].sort((a, b) => a - b);  // ✅ Original intacto
// O usando toSorted() cuando esté disponible
// const ordenado = numeros.toSorted((a, b) => a - b);  // 🔥 Futuro
```

### 💡 **Comparación y Cuándo Usar**

```javascript
// 📊 GUÍA DE ALGORITMOS DE ORDENAMIENTO
const guiaOrdenamiento = {
    bubbleSort: {
        complejidad: "O(n²)",
        estable: true,
        inPlace: true,
        usar: "Solo con fines educativos",
        evitar: "Arrays > 50 elementos"
    },
    
    quickSort: {
        complejidad: "O(n log n) promedio, O(n²) peor caso",
        estable: false,
        inPlace: true,
        usar: "Arrays grandes, memoria limitada",
        ventaja: "Muy rápido en promedio"
    },
    
    mergeSort: {
        complejidad: "O(n log n) garantizado",
        estable: true,
        inPlace: false,
        usar: "Cuando necesitas estabilidad y performance consistente",
        ventaja: "Rendimiento predecible"
    },
    
    nativeSort: {
        complejidad: "O(n log n) optimizado",
        estable: true,
        usar: "✅ SIEMPRE que sea posible",
        ventaja: "Altamente optimizado, implementación nativa"
    }
};

// 🎯 BENCHMARK COMPARISON
const benchmarkSort = (array) => {
    const tests = [
        ['Native Sort', () => [...array].sort((a, b) => a - b)],
        ['Quick Sort', () => quickSort(array)],
        ['Merge Sort', () => mergeSort(array)],
        ['Bubble Sort', () => bubbleSort(array)]  // Solo para arrays pequeños
    ];
    
    tests.forEach(([nombre, fn]) => {
        console.time(nombre);
        fn();
        console.timeEnd(nombre);
    });
};
```

---

## **SESIÓN 7: 🏗️ Estructuras Personalizadas**

### 🎯 **Stack - Pila LIFO (Last In, First Out)**

```javascript
// 🏗️ IMPLEMENTACIÓN DE STACK
class Stack {
    constructor() {
        this.items = [];
    }
    
    // ➕ Agregar elemento al tope
    push(element) {
        this.items.push(element);
        return this.size();
    }
    
    // ➖ Remover y retornar elemento del tope
    pop() {
        if (this.isEmpty()) {
            throw new Error('Stack is empty');
        }
        return this.items.pop();
    }
    
    // 👁️ Ver elemento del tope sin remover
    peek() {
        if (this.isEmpty()) return null;
        return this.items[this.items.length - 1];
    }
    
    // ❓ Verificar si está vacía
    isEmpty() {
        return this.items.length === 0;
    }
    
    // 📏 Obtener tamaño
    size() {
        return this.items.length;
    }
    
    // 🧹 Limpiar stack
    clear() {
        this.items = [];
    }
    
    // 🖨️ Representación string
    toString() {
        return this.items.toString();
    }
}

// 🎯 CASOS DE USO COMUNES
// 1. Validador de paréntesis
const validarParentesis = (expresion) => {
    const stack = new Stack();
    const pares = {'(': ')', '[': ']', '{': '}'};
    
    for (const char of expresion) {
        if (char in pares) {
            stack.push(char);  // Apertura
        } else if (Object.values(pares).includes(char)) {
            if (stack.isEmpty() || pares[stack.pop()] !== char) {
                return false;  // No coincide
            }
        }
    }
    
    return stack.isEmpty();  // Todos cerrados
};

// 2. Historial de navegación
class HistorialNavegacion {
    constructor() {
        this.historial = new Stack();
        this.adelante = new Stack();
    }
    
    visitar(pagina) {
        this.historial.push(pagina);
        this.adelante.clear();  // Limpiar historial "adelante"
    }
    
    atras() {
        if (this.historial.size() > 1) {
            this.adelante.push(this.historial.pop());
            return this.historial.peek();
        }
        return null;
    }
    
    adelantar() {
        if (!this.adelante.isEmpty()) {
            this.historial.push(this.adelante.pop());
            return this.historial.peek();
        }
        return null;
    }
}

// 3. Calculadora RPN (Notación Polaca Inversa)
const calcularRPN = (expresion) => {
    const stack = new Stack();
    const operadores = {
        '+': (a, b) => a + b,
        '-': (a, b) => a - b,
        '*': (a, b) => a * b,
        '/': (a, b) => a / b
    };
    
    for (const token of expresion.split(' ')) {
        if (token in operadores) {
            const b = stack.pop();
            const a = stack.pop();
            stack.push(operadores[token](a, b));
        } else {
            stack.push(parseFloat(token));
        }
    }
    
    return stack.pop();
};

console.log(calcularRPN("3 4 + 2 *"));  // (3 + 4) * 2 = 14
```

### 🎯 **Queue - Cola FIFO (First In, First Out)**

```javascript
// 🔄 IMPLEMENTACIÓN DE QUEUE
class Queue {
    constructor() {
        this.items = [];
    }
    
    // ➕ Agregar elemento al final
    enqueue(element) {
        this.items.push(element);
        return this.size();
    }
    
    // ➖ Remover y retornar primer elemento
    dequeue() {
        if (this.isEmpty()) {
            throw new Error('Queue is empty');
        }
        return this.items.shift();
    }
    
    // 👁️ Ver primer elemento sin remover
    front() {
        if (this.isEmpty()) return null;
        return this.items[0];
    }
    
    // 👁️ Ver último elemento
    rear() {
        if (this.isEmpty()) return null;
        return this.items[this.items.length - 1];
    }
    
    isEmpty() {
        return this.items.length === 0;
    }
    
    size() {
        return this.items.length;
    }
    
    clear() {
        this.items = [];
    }
    
    toString() {
        return this.items.toString();
    }
}

// ⚡ QUEUE OPTIMIZADA (Circular Buffer)
class CircularQueue {
    constructor(capacity = 10) {
        this.items = new Array(capacity);
        this.capacity = capacity;
        this.front = 0;
        this.rear = 0;
        this.size = 0;
    }
    
    enqueue(element) {
        if (this.isFull()) {
            throw new Error('Queue is full');
        }
        
        this.items[this.rear] = element;
        this.rear = (this.rear + 1) % this.capacity;
        this.size++;
        return this.size;
    }
    
    dequeue() {
        if (this.isEmpty()) {
            throw new Error('Queue is empty');
        }
        
        const element = this.items[this.front];
        this.items[this.front] = null;
        this.front = (this.front + 1) % this.capacity;
        this.size--;
        return element;
    }
    
    isEmpty() {
        return this.size === 0;
    }
    
    isFull() {
        return this.size === this.capacity;
    }
}

// 🎯 CASOS DE USO
// 1. Sistema de tareas asíncronas
class TaskQueue {
    constructor() {
        this.queue = new Queue();
        this.processing = false;
    }
    
    addTask(task) {
        this.queue.enqueue(task);
        if (!this.processing) {
            this.processNext();
        }
    }
    
    async processNext() {
        if (this.queue.isEmpty()) {
            this.processing = false;
            return;
        }
        
        this.processing = true;
        const task = this.queue.dequeue();
        
        try {
            await task();
        } catch (error) {
            console.error('Task failed:', error);
        }
        
        this.processNext();  // Procesar siguiente
    }
}

// 2. Búsqueda BFS (Breadth-First Search)
const bfsGraph = (graph, start, target) => {
    const queue = new Queue();
    const visited = new Set();
    
    queue.enqueue([start, [start]]);  // [nodo, camino]
    visited.add(start);
    
    while (!queue.isEmpty()) {
        const [current, path] = queue.dequeue();
        
        if (current === target) {
            return path;  // Camino encontrado
        }
        
        for (const neighbor of graph[current] || []) {
            if (!visited.has(neighbor)) {
                visited.add(neighbor);
                queue.enqueue([neighbor, [...path, neighbor]]);
            }
        }
    }
    
    return null;  // No encontrado
};
```

### 🎯 **Árboles Binarios**

```javascript
// 🌳 NODO DE ÁRBOL BINARIO
class TreeNode {
    constructor(value) {
        this.value = value;
        this.left = null;
        this.right = null;
    }
}

// 🌳 ÁRBOL BINARIO DE BÚSQUEDA (BST)
class BinarySearchTree {
    constructor() {
        this.root = null;
    }
    
    // ➕ Insertar valor
    insert(value) {
        const newNode = new TreeNode(value);
        
        if (!this.root) {
            this.root = newNode;
            return this;
        }
        
        let current = this.root;
        while (true) {
            if (value === current.value) return undefined;  // Duplicado
            
            if (value < current.value) {
                if (!current.left) {
                    current.left = newNode;
                    return this;
                }
                current = current.left;
            } else {
                if (!current.right) {
                    current.right = newNode;
                    return this;
                }
                current = current.right;
            }
        }
    }
    
    // 🔍 Buscar valor
    find(value) {
        if (!this.root) return false;
        
        let current = this.root;
        while (current) {
            if (value === current.value) return current;
            current = value < current.value ? current.left : current.right;
        }
        
        return false;
    }
    
    // 📊 RECORRIDOS
    // Inorden: Izquierda → Raíz → Derecha (ordenado)
    inOrder(node = this.root, result = []) {
        if (node) {
            this.inOrder(node.left, result);
            result.push(node.value);
            this.inOrder(node.right, result);
        }
        return result;
    }
    
    // Preorden: Raíz → Izquierda → Derecha
    preOrder(node = this.root, result = []) {
        if (node) {
            result.push(node.value);
            this.preOrder(node.left, result);
            this.preOrder(node.right, result);
        }
        return result;
    }
    
    // Postorden: Izquierda → Derecha → Raíz
    postOrder(node = this.root, result = []) {
        if (node) {
            this.postOrder(node.left, result);
            this.postOrder(node.right, result);
            result.push(node.value);
        }
        return result;
    }
    
    // 📏 Propiedades del árbol
    height(node = this.root) {
        if (!node) return -1;
        return 1 + Math.max(this.height(node.left), this.height(node.right));
    }
    
    isBalanced(node = this.root) {
        if (!node) return true;
        
        const leftHeight = this.height(node.left);
        const rightHeight = this.height(node.right);
        
        return Math.abs(leftHeight - rightHeight) <= 1 &&
               this.isBalanced(node.left) &&
               this.isBalanced(node.right);
    }
}

// 🎯 EJEMPLO DE USO
const bst = new BinarySearchTree();
[15, 10, 20, 8, 12, 25, 6].forEach(val => bst.insert(val));

console.log('Inorden:', bst.inOrder());      // [6, 8, 10, 12, 15, 20, 25] - Ordenado
console.log('Altura:', bst.height());        // Altura del árbol
console.log('Balanceado:', bst.isBalanced()); // Si está balanceado
```

### 💡 **Cuándo Usar Cada Estructura**

```javascript
// 🎯 GUÍA DE ESTRUCTURAS PERSONALIZADAS
const guiaEstructuras = {
    Stack: {
        usar: "LIFO, deshacer/rehacer, validación de sintaxis, navegación",
        ejemplos: ["Historial del navegador", "Ctrl+Z", "Calculadora RPN", "Paréntesis balanceados"],
        complejidad: "O(1) para push/pop"
    },
    
    Queue: {
        usar: "FIFO, procesamiento en orden, BFS, sistemas de tareas",
        ejemplos: ["Cola de impresión", "Procesamiento de tareas", "BFS en grafos", "Buffer de eventos"],
        complejidad: "O(1) para enqueue/dequeue"
    },
    
    BinarySearchTree: {
        usar: "Búsqueda rápida en datos ordenados, rangos",
        ejemplos: ["Índices de base de datos", "Autocompletado", "Rangos de fechas"],
        complejidad: "O(log n) búsqueda/inserción (si balanceado)"
    }
};

// ⚡ PERFORMANCE TIPS
const performanceTips = {
    Stack: "Usar Array nativo con push/pop es eficiente en JS",
    Queue: "Para alta performance, usar CircularQueue o deque libraries",
    Tree: "Para uso intensivo, considerar bibliotecas como AVL o Red-Black trees"
};
```

---

## **SESIÓN 8: ⚡ Optimización y Performance**

### 🎯 **Análisis Big O - Complejidad Temporal**

```javascript
// 📊 EJEMPLOS DE COMPLEJIDADES
const ejemplosComplejidad = {
    
    // O(1) - Constante ⚡ MUY RÁPIDO
    accesoDirecto: (array, index) => array[index],
    mapGet: (map, key) => map.get(key),
    
    // O(log n) - Logarítmico ⚡ RÁPIDO
    busquedaBinaria: (sortedArray, target) => {
        // Implementación anterior...
    },
    
    // O(n) - Lineal 📈 ACEPTABLE
    busquedaLineal: (array, target) => array.indexOf(target),
    sumarArray: (array) => array.reduce((sum, num) => sum + num, 0),
    
    // O(n log n) - Log-lineal 📈 BUENO PARA ORDENAMIENTO
    ordenamientoEficiente: (array) => array.sort((a, b) => a - b),
    
    // O(n²) - Cuadrático ⚠️ LENTO
    comparacionesPares: (array) => {
        const pares = [];
        for (let i = 0; i < array.length; i++) {
            for (let j = i + 1; j < array.length; j++) {
                pares.push([array[i], array[j]]);
            }
        }
        return pares;
    },
    
    // O(2^n) - Exponencial 🚨 MUY LENTO
    fibonacciRecursivo: (n) => {
        if (n <= 1) return n;
        return fibonacciRecursivo(n - 1) + fibonacciRecursivo(n - 2);
    }
};

// 📏 MEDICIÓN DE PERFORMANCE
const medirTiempo = (fn, nombre, ...args) => {
    console.time(nombre);
    const resultado = fn(...args);
    console.timeEnd(nombre);
    return resultado;
};

// 🎯 COMPARAR ALGORITMOS
const compararAlgoritmos = (array, target) => {
    const sortedArray = [...array].sort((a, b) => a - b);
    
    console.log(`Comparando con array de ${array.length} elementos:`);
    
    medirTiempo(array => array.indexOf(target), 'Búsqueda Lineal', array);
    medirTiempo((arr, tgt) => busquedaBinaria(arr, tgt), 'Búsqueda Binaria', sortedArray, target);
};
```

### 🎯 **Memoización - Cache de Resultados**

```javascript
// 💾 MEMOIZACIÓN BÁSICA
const memoize = (fn) => {
    const cache = new Map();
    
    return function(...args) {
        const key = JSON.stringify(args);
        
        if (cache.has(key)) {
            console.log('Cache hit! 🎯');
            return cache.get(key);
        }
        
        console.log('Calculando... ⚡');
        const result = fn.apply(this, args);
        cache.set(key, result);
        return result;
    };
};

// 🎯 FIBONACCI OPTIMIZADO
const fibonacciMemo = memoize((n) => {
    if (n <= 1) return n;
    return fibonacciMemo(n - 1) + fibonacciMemo(n - 2);
});

// Comparación dramática:
// fibonacciRecursivo(40) - varios segundos 🐌
// fibonacciMemo(40) - milisegundos ⚡

// 💾 CACHE CON TTL (Time To Live)
class CacheConTTL {
    constructor(ttl = 60000) {  // 1 minuto por defecto
        this.cache = new Map();
        this.ttl = ttl;
    }
    
    set(key, value) {
        this.cache.set(key, {
            value,
            timestamp: Date.now()
        });
    }
    
    get(key) {
        const item = this.cache.get(key);
        
        if (!item) return null;
        
        if (Date.now() - item.timestamp > this.ttl) {
            this.cache.delete(key);
            return null;
        }
        
        return item.value;
    }
    
    has(key) {
        return this.get(key) !== null;
    }
    
    clear() {
        this.cache.clear();
    }
    
    // Limpieza automática de elementos expirados
    cleanup() {
        const now = Date.now();
        for (const [key, item] of this.cache) {
            if (now - item.timestamp > this.ttl) {
                this.cache.delete(key);
            }
        }
    }
}

// 🎯 MEMOIZACIÓN AVANZADA CON LRU
class LRUCache {
    constructor(capacity = 100) {
        this.capacity = capacity;
        this.cache = new Map();
    }
    
    get(key) {
        if (this.cache.has(key)) {
            // Mover al final (más reciente)
            const value = this.cache.get(key);
            this.cache.delete(key);
            this.cache.set(key, value);
            return value;
        }
        return null;
    }
    
    set(key, value) {
        if (this.cache.has(key)) {
            this.cache.delete(key);
        } else if (this.cache.size >= this.capacity) {
            // Eliminar el menos usado (primero)
            const firstKey = this.cache.keys().next().value;
            this.cache.delete(firstKey);
        }
        
        this.cache.set(key, value);
    }
}
```

### 🎯 **Técnicas de Optimización**

```javascript
// ⚡ DEBOUNCE - Retrasar ejecución
const debounce = (func, delay) => {
    let timeoutId;
    return function(...args) {
        clearTimeout(timeoutId);
        timeoutId = setTimeout(() => func.apply(this, args), delay);
    };
};

// Uso común: Búsqueda mientras escribes
const busquedaDebounced = debounce((query) => {
    console.log(`Buscando: ${query}`);
    // Hacer petición a API...
}, 300);

// ⚡ THROTTLE - Limitar frecuencia
const throttle = (func, limit) => {
    let inThrottle;
    return function(...args) {
        if (!inThrottle) {
            func.apply(this, args);
            inThrottle = true;
            setTimeout(() => inThrottle = false, limit);
        }
    };
};

// Uso común: Scroll events
const onScrollThrottled = throttle(() => {
    console.log('Scroll event');
}, 100);

// 🔄 LAZY LOADING - Carga diferida
const lazyLoad = (factory) => {
    let instance;
    return () => {
        if (!instance) {
            instance = factory();
        }
        return instance;
    };
};

const expensiveData = lazyLoad(() => {
    console.log('Cargando datos costosos...');
    return Array.from({length: 10000}, (_, i) => i * i);
});

// 📦 BATCH PROCESSING - Procesamiento por lotes
const batchProcess = (items, batchSize, processor) => {
    const results = [];
    
    for (let i = 0; i < items.length; i += batchSize) {
        const batch = items.slice(i, i + batchSize);
        results.push(...processor(batch));
    }
    
    return results;
};

// Procesar 10,000 elementos en lotes de 100
const procesarDatos = (datos) => {
    return batchProcess(datos, 100, (batch) => 
        batch.map(item => item * 2)
    );
};

// 🎯 OBJECT POOLING - Reutilización de objetos
class ObjectPool {
    constructor(createFn, resetFn, capacity = 10) {
        this.createFn = createFn;
        this.resetFn = resetFn;
        this.pool = [];
        this.capacity = capacity;
    }
    
    acquire() {
        if (this.pool.length > 0) {
            return this.pool.pop();
        }
        return this.createFn();
    }
    
    release(obj) {
        if (this.pool.length < this.capacity) {
            this.resetFn(obj);
            this.pool.push(obj);
        }
    }
}

// Ejemplo: Pool de objetos Vector2D
const vectorPool = new ObjectPool(
    () => ({x: 0, y: 0}),           // Crear
    (obj) => {obj.x = 0; obj.y = 0;} // Reset
);
```

### 🎯 **Identificar Cuellos de Botella**

```javascript
// 🔍 PROFILING Y ANÁLISIS
const profileFunction = (fn, name, iterations = 1000) => {
    const start = performance.now();
    
    for (let i = 0; i < iterations; i++) {
        fn();
    }
    
    const end = performance.now();
    const total = end - start;
    const average = total / iterations;
    
    console.log(`${name}:`);
    console.log(`  Total: ${total.toFixed(2)}ms`);
    console.log(`  Average: ${average.toFixed(4)}ms per iteration`);
    console.log(`  Operations/sec: ${(1000 / average).toFixed(0)}`);
    
    return { total, average };
};

// 🎯 MEMORY USAGE (si está disponible)
const measureMemory = (fn) => {
    const memBefore = performance.memory?.usedJSHeapSize || 0;
    const result = fn();
    const memAfter = performance.memory?.usedJSHeapSize || 0;
    
    console.log(`Memory used: ${memAfter - memBefore} bytes`);
    return result;
};

// 🚨 ANTIPATRONES COMUNES
const antipatrones = {
    // ❌ Búsqueda ineficiente
    busquedaIneficiente: (array, targets) => {
        return targets.map(target => 
            array.find(item => item.id === target)  // O(n) por cada target
        );
    },
    
    // ✅ Con índice
    busquedaEficiente: (array, targets) => {
        const index = new Map(array.map(item => [item.id, item]));
        return targets.map(target => index.get(target));  // O(1) por target
    },
    
    // ❌ Concatenación ineficiente
    concatenacionIneficiente: (strings) => {
        let result = '';
        for (const str of strings) {
            result += str;  // Crea nueva string cada vez
        }
        return result;
    },
    
    // ✅ Usando join
    concatenacionEficiente: (strings) => {
        return strings.join('');  // Optimizado internamente
    }
};

// 📊 BENCHMARK COMPARISON
const compararImplementaciones = (data) => {
    const targets = [1, 100, 500, 999];
    
    profileFunction(
        () => antipatrones.busquedaIneficiente(data, targets),
        'Búsqueda Ineficiente'
    );
    
    profileFunction(
        () => antipatrones.busquedaEficiente(data, targets),
        'Búsqueda Eficiente'
    );
};
```

### 💡 **Mejores Prácticas de Performance**

```javascript
// 🎯 CHECKLIST DE OPTIMIZACIÓN
const checklistOptimizacion = {
    estructurasDatos: [
        "✅ Usar Map/Set para búsquedas frecuentes O(1)",
        "✅ Arrays para listas ordenadas y acceso por índice",
        "✅ WeakMap/WeakSet para evitar memory leaks"
    ],
    
    algoritmos: [
        "✅ Memoizar funciones costosas",
        "✅ Usar búsqueda binaria en datos ordenados",
        "✅ Batch processing para operaciones masivas",
        "✅ Lazy loading para datos grandes"
    ],
    
    eventos: [
        "✅ Debounce para inputs de usuario",
        "✅ Throttle para eventos frecuentes (scroll, resize)",
        "✅ Event delegation para muchos elementos"
    ],
    
    memoria: [
        "✅ Limpiar referencias no usadas",
        "✅ Usar Object Pooling para objetos temporales",
        "✅ WeakMap para metadatos de objetos"
    ]
};

// 🎯 CUANDO OPTIMIZAR
const cuandoOptimizar = {
    siempre: [
        "Elegir la estructura de datos correcta",
        "Usar algoritmos con buena complejidad",
        "Evitar operaciones costosas en loops"
    ],
    
    despues: [
        "Micro-optimizaciones",
        "Object pooling",
        "Compresión de datos"
    ],
    
    reglaOro: "Measure first, optimize second 📊"
};

console.log("🚀 Optimización completada - ¡Tu código es más rápido y eficiente!");
```

---

## 🎊 **¡CHEATSHEET COMPLETADO!**

```javascript
const cheatsheetCompletado = {
    sesiones: 8,
    temas: [
        "📊 Arrays Esenciales",
        "⚡ Métodos Funcionales", 
        "🏛️ Objetos y Propiedades",
        "🛠️ Estructuras Avanzadas",
        "📈 Algoritmos de Búsqueda",
        "🔄 Algoritmos de Ordenamiento",
        "🏗️ Estructuras Personalizadas",
        "⚡ Optimización y Performance"
    ],
    codigoEjemplos: "200+ snippets prácticos",
    usoPrincipal: "📋 Referencia rápida mientras programas"
};

console.log("🎯 ¡Tienes la referencia definitiva de estructuras de datos en JavaScript!");
console.log("💡 Guarda este enlace y úsalo como tu companion de programación");
```

---

**🔖 BOOKMARKS RÁPIDOS:**
- [📊 Arrays](#sesión-1-📊-arrays-esenciales) | [⚡ Funcionales](#sesión-2-⚡-métodos-funcionales) | [🏛️ Objetos](#sesión-3-🏛️-objetos-y-propiedades) | [🛠️ Avanzadas](#sesión-4-🛠️-estructuras-avanzadas)
- [🔍 Búsqueda](#sesión-5-📈-algoritmos-búsqueda) | [🔄 Ordenamiento](#sesión-6-🔄-algoritmos-ordenamiento) | [🏗️ Personalizadas](#sesión-7-🏗️-estructuras-personalizadas) | [⚡ Performance](#sesión-8-⚡-optimización-performance)

---

[🔙 **Volver al Libro Principal**](./ESTRUCTURAS-DATOS-LIBRO.md) | [🏠 **Índice General**](../../../README.md) | [📚 **Navegación**](../../../NAVEGACION-DOCUMENTOS.md)
