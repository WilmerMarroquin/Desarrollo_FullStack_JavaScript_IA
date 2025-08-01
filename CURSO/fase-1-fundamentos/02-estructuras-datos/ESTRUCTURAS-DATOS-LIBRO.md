[🏠 **Volver al Índice de Navegación**](../../../NAVEGACION-DOCUMENTOS.md)

---

# 📊 ESTRUCTURAS DE DATOS EN JAVASCRIPT

## La Guía Definitiva para Dominar la Organización y Manipulación de Información

> **🎯 "Los datos sin estructura son como una biblioteca sin catálogo. Aprende a organizar, acceder y transformar información de manera eficiente."**

**📖 Fase 1 - Tema 2** • **⏱️ Tiempo estimado:** 10-14 horas • **🎓 Nivel:** Principiante a Intermedio

---

## 🧭 **NAVEGACIÓN RÁPIDA**

### 📚 **ÍNDICE COMPLETO**

|                     **🏗️ FUNDAMENTOS**                      |                   **📊 ARRAYS**                    |                 **🛠️ ESTRUCTURAS AVANZADAS**                  |               **📋 REFERENCIA**                |
| :---------------------------------------------------------: | :------------------------------------------------: | :---------------------------------------------: | :--------------------------------------------: |
| [📦 ¿Qué son las Estructuras?](#1-📦-qué-son-las-estructuras-de-datos) |    [🔢 Arrays Básicos](#4-🔢-arrays-básicos)     | [🏛️ Objetos y Propiedades](#7-🏛️-objetos-y-propiedades) |   [🧪 Ejercicios](#12-🧪-ejercicios-interactivos)    |
| [🧠 Tipos de Estructuras](#2-🧠-tipos-de-estructuras-de-datos) | [⚡ Métodos de Arrays](#5-⚡-métodos-de-arrays) | [🔗 Objetos Anidados](#8-🔗-objetos-anidados) | [📚 Recursos](#13-📚-recursos-y-referencias) |
|    [💾 Memoria y Rendimiento](#3-💾-memoria-y-rendimiento)     | [🎯 Arrays Avanzados](#6-🎯-arrays-avanzados)  | [🛠️ Maps, Sets y WeakMaps](#9-🛠️-estructuras-de-datos-avanzadas) | [� Cheatsheet](#�-cheatsheet-visual)  |

### 🎮 **ACCESOS RÁPIDOS**

- 🚀 [**Empezar Ahora**](#1-📦-qué-son-las-estructuras-de-datos) - Si eres completamente nuevo
- 🔧 [**Configurar Entorno**](../../GUIA-INSTALACION.md) - Prepara tu PC para programar
- 🧪 [**Ejercicios Prácticos**](./ejercicios-practicos/README-EJERCICIOS.md) - Lista de 20 ejercicios progresivos
- 🎯 [**Proyectos Guiados**](./proyectos-guiados/) - 5 proyectos para aplicar conceptos
- 📋 [**Cheatsheet Visual**](./CHEATSHEET-VISUAL.md) - Referencia rápida de sintaxis

---

## **📖 CONTENIDO COMPLETO**

1. [📦 ¿Qué son las Estructuras de Datos?](#1-📦-qué-son-las-estructuras-de-datos)
2. [🧠 Tipos de Estructuras de Datos](#2-🧠-tipos-de-estructuras-de-datos)
3. [💾 Memoria y Rendimiento](#3-💾-memoria-y-rendimiento)
4. [🔢 Arrays Básicos](#4-🔢-arrays-básicos)
5. [⚡ Métodos de Arrays](#5-⚡-métodos-de-arrays)
6. [🎯 Arrays Avanzados](#6-🎯-arrays-avanzados) 
7. [🏛️ Objetos y Propiedades](#7-🏛️-objetos-y-propiedades)
8. [🔗 Objetos Anidados](#8-🔗-objetos-anidados)
9. [🛠️ Estructuras de Datos Avanzadas](#9-🛠️-estructuras-de-datos-avanzadas)
10. [📈 Algoritmos y Rendimiento](#10-📈-algoritmos-y-rendimiento)
11. [🏗️ Estructuras Especializadas y Proyectos](#11-🏗️-estructuras-especializadas-y-proyectos)
12. [🧪 Ejercicios Interactivos](#12-🧪-ejercicios-interactivos)
13. [📚 Recursos y Referencias](#13-📚-recursos-y-referencias)

📝 **Recursos Complementarios:**
- 📝 [**Cheatsheet Visual**](./CHEATSHEET-VISUAL.md) - Referencia rápida
- 🧪 [**Ejercicios Prácticos**](./ejercicios-practicos/README-EJERCICIOS.md) - 20 ejercicios progresivos
- 🎯 [**Proyectos Guiados**](./proyectos-guiados/) - 5 proyectos aplicados

---

## 🎯 **OBJETIVOS DE APRENDIZAJE**

Al completar este tema, serás capaz de:

### 🏗️ **Fundamentos**
- ✅ **Entender** qué son las estructuras de datos y por qué son importantes
- ✅ **Identificar** cuándo usar cada tipo de estructura
- ✅ **Optimizar** el rendimiento según el tipo de datos

### 📊 **Arrays**
- ✅ **Crear y manipular** arrays de forma eficiente
- ✅ **Dominar** todos los métodos nativos de JavaScript
- ✅ **Aplicar** técnicas funcionales (map, filter, reduce)

### 🏛️ **Objetos**
- ✅ **Estructurar** información compleja con objetos
- ✅ **Navegar** por estructuras anidadas
- ✅ **Combinar** arrays y objetos para casos reales

### 🌐 **Estructuras Avanzadas**
- ✅ **Implementar** Map y Set para casos específicos
- ✅ **Manejar** WeakMap y WeakSet con referencias débiles  
- ✅ **Dominar** algoritmos de búsqueda y ordenamiento
- ✅ **Optimizar** rendimiento y complejidad temporal

### 🎯 **Aplicación Práctica**
- ✅ **Crear** estructuras personalizadas (Stack, Queue, Trees)
- ✅ **Resolver** problemas del mundo real
- ✅ **Integrar** conceptos en proyectos completos
- ✅ **Evaluar** trade-offs de rendimiento vs memoria

---

## 🚀 **PRERREQUISITOS**

### ✅ **Conocimientos Necesarios**
- 🧠 **Lógica de Programación** (Tema 1 completo)
- 📦 Variables, funciones y condicionales básicas
- 💻 Entorno de desarrollo configurado

### 🔧 **Herramientas Requeridas**
- ✅ Node.js instalado
- ✅ VS Code con extensiones JavaScript
- ✅ Navegador con DevTools
- ✅ Git configurado

> **💡 Tip:** Si no has completado estos requisitos, visita la [**Guía de Instalación**](../../GUIA-INSTALACION.md) primero.

---

## 🎨 **METODOLOGÍA DE ESTUDIO**

### 📚 **Cómo Usar Este Libro**

```javascript
// 🎯 Proceso de aprendizaje recomendado:
const metodologiaEstructuras = {
    1: "📖 Lee cada concepto completo antes de codificar",
    2: "💻 Practica cada ejemplo en tu editor",
    3: "🔄 Experimenta con variaciones del código",
    4: "🧪 Completa los ejercicios progresivamente", 
    5: "🎯 Aplica lo aprendido en los proyectos",
    6: "📝 Usa el cheatsheet como referencia constante",
    7: "🔁 Repite y refuerza conceptos difíciles"
};

// 💡 Consejos para el éxito:
const consejosAprendizaje = {
    consistencia: "🔄 30 minutos diarios > 4 horas una vez",
    practica: "💻 Escribe código, no solo leas",
    experimentacion: "🧪 Rompe el código para entender cómo funciona",
    proyectos: "🎯 Aplica conceptos en problemas reales",
    comunidad: "👥 Comparte dudas y descubrimientos"
};
```

### 🌟 **Niveles de Dificultad**

- 🟢 **BÁSICO** - Conceptos fundamentales de estructuras
- 🟡 **INTERMEDIO** - Manipulación y transformación de datos
- 🔴 **AVANZADO** - Optimización y estructuras complejas
- 🟣 **EXPERTO** - Casos de uso del mundo real

---

## 🏁 **¡COMENCEMOS!**

### 🎯 **Tu Ruta de Aprendizaje**

```javascript
const rutaAprendizaje = {
    semana1: {
        enfoque: "🏗️ Fundamentos y Arrays Básicos",
        tiempo: "3-4 horas",
        capitulos: [1, 2, 3, 4],
        resultado: "Dominio de arrays unidimensionales"
    },
    semana2: {
        enfoque: "⚡ Métodos y Arrays Avanzados", 
        tiempo: "3-4 horas",
        capitulos: [5, 6],
        resultado: "Maestría en transformación de arrays"
    },
    semana3: {
        enfoque: "🏛️ Objetos y Estructuras Complejas",
        tiempo: "4-5 horas", 
        capitulos: [7, 8, 9],
        resultado: "Manejo experto de objetos y Maps/Sets"
    },
    semana4: {
        enfoque: "📈 Algoritmos y Proyectos Finales",
        tiempo: "3-4 horas",
        capitulos: [10, 11],
        resultado: "Aplicación práctica y optimización"
    }
};

console.log("🚀 ¿Listo para comenzar tu aventura con las estructuras de datos?");
```

---

**🎊 ¿Estás listo para transformar la forma en que organizas y manipulas datos?**

[🚀 **¡Empezar con el Capítulo 1!**](#1-📦-qué-son-las-estructuras-de-datos)

---

[🔙 **Tema Anterior: Lógica**](../01-logica-programacion/LOGICA-PROGRAMACION-LIBRO.md) | [🏠 **Fase 1**](../README.md) | [🔜 **Tema Siguiente: JS Moderno**](../03-javascript-moderno/) | [🔗 **Tema 4: Git**](../04-git-github/)

---

# 📖 **CONTENIDO DETALLADO**

---

## 1. 📦 **¿Qué son las Estructuras de Datos?**

### 🎯 **Introducción Conceptual**

Las estructuras de datos son la **columna vertebral** de cualquier programa. Son formas organizadas de almacenar, acceder y manipular información de manera eficiente.

```javascript
// 🤔 Piensa en las estructuras de datos como contenedores:
const ejemploVidaReal = {
    // 📚 Una biblioteca organiza libros por categorías
    biblioteca: {
        ficcion: ["1984", "Cien años de soledad", "El principito"],
        ciencia: ["Cosmos", "Breve historia del tiempo"],
        historia: ["Sapiens", "El arte de la guerra"]
    },
    
    // 📞 Una agenda telefónica organiza contactos por nombre
    agenda: {
        "Juan Pérez": "555-0123",
        "María García": "555-0456", 
        "Carlos López": "555-0789"
    },
    
    // 🛒 Una lista de compras organiza productos por orden
    listaCompras: ["Leche", "Pan", "Huevos", "Frutas", "Verduras"]
};

console.log("📊 Las estructuras de datos organizan información como en la vida real");
```

### 🧠 **¿Por Qué Son Importantes?**

```javascript
// ❌ Sin estructura: Información caótica
let info = "Juan25años555-0123MaríaGarcía30años555-0456CarlosLópez28años555-0789";

// ✅ Con estructura: Información organizada
const personas = [
    { nombre: "Juan", edad: 25, telefono: "555-0123" },
    { nombre: "María García", edad: 30, telefono: "555-0456" },
    { nombre: "Carlos López", edad: 28, telefono: "555-0789" }
];

// 🎯 Beneficios inmediatos:
// 1. Fácil acceso a datos específicos
console.log("Primera persona:", personas[0].nombre);

// 2. Búsqueda eficiente
const personaEnccontrada = personas.find(p => p.nombre === "María García");

// 3. Transformación de datos
const soloNombres = personas.map(p => p.nombre);

// 4. Filtrado de información
const mayoresDe25 = personas.filter(p => p.edad > 25);
```

### 🏗️ **Características Clave**

```javascript
// 📊 Las buenas estructuras de datos tienen:
const caracteristicasEstructuras = {
    // 🎯 1. ORGANIZACIÓN - Todo tiene su lugar
    organizacion: {
        ejemplo: "Arrays para listas, Objetos para entidades",
        beneficio: "Fácil localización de datos"
    },
    
    // ⚡ 2. EFICIENCIA - Acceso rápido
    eficiencia: {
        ejemplo: "Array[0] es más rápido que buscar en 1000 elementos",
        beneficio: "Mejor rendimiento del programa"
    },
    
    // 🔄 3. MANIPULACIÓN - Fácil modificación
    manipulacion: {
        ejemplo: "array.push() para agregar, array.filter() para filtrar",
        beneficio: "Código más limpio y mantenible"
    },
    
    // 🛡️ 4. INTEGRIDAD - Datos consistentes
    integridad: {
        ejemplo: "Validaciones y tipos consistentes",
        beneficio: "Menos errores en producción"
    }
};
```

### 🌟 **Casos de Uso Reales**

```javascript
// 🎮 Ejemplo práctico: Sistema de gestión escolar
class SistemaEscolar {
    constructor() {
        // 📚 Array para listas ordenadas
        this.estudiantes = [];
        
        // 🏛️ Objeto para datos estructurados
        this.escuela = {
            nombre: "Instituto Tecnológico",
            direccion: "Calle Principal 123",
            telefono: "555-ESCUELA"
        };
        
        // 📊 Map para relaciones clave-valor únicas
        this.calificaciones = new Map();
        
        // 🎯 Set para elementos únicos
        this.materias = new Set();
    }
    
    // ➕ Agregar estudiante
    agregarEstudiante(estudiante) {
        this.estudiantes.push(estudiante);
        this.calificaciones.set(estudiante.id, []);
    }
    
    // 📝 Registrar calificación
    registrarCalificacion(estudianteId, materia, nota) {
        this.materias.add(materia);
        const notas = this.calificaciones.get(estudianteId);
        notas.push({ materia, nota, fecha: new Date() });
    }
    
    // 📊 Obtener promedio
    obtenerPromedio(estudianteId) {
        const notas = this.calificaciones.get(estudianteId);
        const suma = notas.reduce((acc, item) => acc + item.nota, 0);
        return suma / notas.length;
    }
}

// 🚀 Uso del sistema
const sistema = new SistemaEscolar();
sistema.agregarEstudiante({ id: 1, nombre: "Ana Rodríguez" });
sistema.registrarCalificacion(1, "Matemáticas", 85);
sistema.registrarCalificacion(1, "Historia", 92);

console.log("📊 Promedio de Ana:", sistema.obtenerPromedio(1));
```

---

## 2. 🧠 **Tipos de Estructuras de Datos**

### 📋 **Clasificación Principal**

```javascript
// 🏗️ JavaScript nos ofrece diferentes tipos de estructuras:
const tiposEstructuras = {
    // 1️⃣ PRIMITIVAS - Datos simples
    primitivas: {
        number: 42,
        string: "Hola mundo",
        boolean: true,
        null: null,
        undefined: undefined,
        symbol: Symbol("único"),
        bigint: 123456789012345678901234567890n
    },
    
    // 2️⃣ COMPUESTAS - Agrupan datos
    compuestas: {
        // 📊 Arrays - Listas ordenadas
        arrays: [1, 2, 3, 4, 5],
        
        // 🏛️ Objects - Colecciones clave-valor
        objects: { nombre: "Juan", edad: 30 },
        
        // 🎯 Functions - Bloques de código reutilizable
        functions: function() { return "¡Hola!"; }
    },
    
    // 3️⃣ ESPECIALIZADAS - Para casos específicos
    especializadas: {
        // 🗂️ Set - Elementos únicos
        set: new Set([1, 2, 3, 3, 3]), // Solo guardará [1, 2, 3]
        
        // 🗺️ Map - Mapeo clave-valor avanzado
        map: new Map([
            ["clave1", "valor1"],
            ["clave2", "valor2"]
        ]),
        
        // 📅 Date - Manejo de fechas
        date: new Date(),
        
        // 🔢 Array tipados - Para datos numéricos
        typedArray: new Int32Array([1, 2, 3, 4])
    }
};
```

### 🎯 **¿Cuándo Usar Cada Una?**

```javascript
// 🤔 Guía de decisión para elegir estructura:
const guiaEstructuras = {
    // 📊 USA ARRAYS CUANDO:
    arrays: {
        casos: [
            "Necesites orden específico",
            "Tengas elementos duplicados",
            "Requieras acceso por índice",
            "Vayas a iterar frecuentemente"
        ],
        ejemplos: {
            listaTareas: ["Estudiar", "Ejercicio", "Leer", "Dormir"],
            historialCompras: [
                { producto: "Laptop", precio: 1200 },
                { producto: "Mouse", precio: 25 },
                { producto: "Teclado", precio: 75 }
            ],
            numerosLoteria: [7, 13, 22, 31, 45, 50]
        }
    },
    
    // 🏛️ USA OBJETOS CUANDO:
    objects: {
        casos: [
            "Modeles entidades del mundo real",
            "Necesites propiedades nombradas",
            "Requieras estructura jerárquica",
            "Tengas datos relacionados"
        ],
        ejemplos: {
            usuario: {
                id: 12345,
                nombre: "Elena Martínez",
                email: "elena@email.com",
                preferencias: {
                    tema: "oscuro",
                    idioma: "español",
                    notificaciones: true
                }
            },
            configuracion: {
                api: { url: "https://api.ejemplo.com", timeout: 5000 },
                ui: { mostrarTutorial: false, animaciones: true }
            }
        }
    },
    
    // 🎯 USA SET CUANDO:
    sets: {
        casos: [
            "Necesites elementos únicos",
            "Requieras búsquedas rápidas",
            "Hagas operaciones de conjuntos",
            "Elimines duplicados"
        ],
        ejemplos: {
            tagsUnicos: new Set(["javascript", "react", "node", "javascript"]),
            visitasUnicas: new Set(),
            permisosUsuario: new Set(["leer", "escribir", "admin"])
        }
    },
    
    // 🗺️ USA MAP CUANDO:
    maps: {
        casos: [
            "Las claves no sean strings",
            "Necesites tamaño dinámico",
            "Requieras iteración ordenada",
            "Tengas operaciones frecuentes de inserción/eliminación"
        ],
        ejemplos: {
            cache: new Map([
                [1, { datos: "usuario1" }],
                ["config", { tema: "claro" }],
                [true, "valor booleano"]
            ]),
            contadores: new Map([
                ["clicks", 0],
                ["visitas", 0],
                ["errores", 0]
            ])
        }
    }
};
```

### 📊 **Comparación de Rendimiento**

```javascript
// ⚡ Análisis de eficiencia por operación:
const rendimientoEstructuras = {
    // 🔍 BÚSQUEDA DE ELEMENTOS
    busqueda: {
        array: {
            complejidad: "O(n) - Lineal",
            ejemplo: "array.find(item => item.id === 5)",
            mejor_para: "Listas pequeñas, búsquedas ocasionales"
        },
        object: {
            complejidad: "O(1) - Constante",
            ejemplo: "object[clave]",
            mejor_para: "Acceso directo por clave"
        },
        set: {
            complejidad: "O(1) - Constante",
            ejemplo: "set.has(valor)",
            mejor_para: "Verificar existencia"
        },
        map: {
            complejidad: "O(1) - Constante",
            ejemplo: "map.get(clave)",
            mejor_para: "Claves complejas"
        }
    },
    
    // ➕ INSERCIÓN DE ELEMENTOS
    insercion: {
        array: {
            inicio: "O(n) - Desplaza todos los elementos",
            final: "O(1) - Muy rápido",
            medio: "O(n) - Desplaza elementos posteriores"
        },
        object: {
            complejidad: "O(1) - Constante",
            nota: "Siempre rápido para nuevas propiedades"
        },
        set: {
            complejidad: "O(1) - Constante",
            nota: "No permite duplicados"
        },
        map: {
            complejidad: "O(1) - Constante",
            nota: "Mantiene orden de inserción"
        }
    }
};

// 🧪 Ejemplo práctico de rendimiento
function demostracionRendimiento() {
    const datos = Array.from({length: 100000}, (_, i) => i);
    
    console.time("Array - Búsqueda lineal");
    datos.find(x => x === 99999);
    console.timeEnd("Array - Búsqueda lineal");
    
    const set = new Set(datos);
    console.time("Set - Búsqueda constante");
    set.has(99999);
    console.timeEnd("Set - Búsqueda constante");
    
    const map = new Map(datos.map(x => [x, `valor${x}`]));
    console.time("Map - Búsqueda constante");
    map.get(99999);
    console.timeEnd("Map - Búsqueda constante");
}
```

---

## 3. 💾 **Memoria y Rendimiento**

### 🧠 **Cómo JavaScript Maneja la Memoria**

```javascript
// 🏗️ JavaScript gestiona dos tipos de memoria:
const gestionMemoria = {
    // 📦 STACK (Pila) - Datos primitivos y referencias
    stack: {
        descripcion: "Memoria rápida para datos simples",
        contiene: ["primitivos", "referencias a objetos"],
        ejemplo: () => {
            let numero = 42;           // 💾 Guardado en Stack
            let texto = "Hola";        // 💾 Guardado en Stack
            let objeto;                // 💾 Solo la referencia en Stack
        }
    },
    
    // 🏗️ HEAP (Montón) - Objetos y estructuras complejas
    heap: {
        descripcion: "Memoria flexible para datos complejos",
        contiene: ["objetos", "arrays", "funciones"],
        ejemplo: () => {
            let array = [1, 2, 3];     // 💾 Datos en Heap, referencia en Stack
            let obj = {a: 1, b: 2};    // 💾 Datos en Heap, referencia en Stack
        }
    }
};

// 🔄 Demostración de referencias vs copias
function demoReferenciasVsCopias() {
    // 📦 PRIMITIVOS - Se copian por valor
    let a = 10;
    let b = a;      // ✅ 'b' es una copia independiente
    a = 20;
    console.log("a:", a, "b:", b); // a: 20, b: 10
    
    // 🏛️ OBJETOS - Se copian por referencia
    let obj1 = { numero: 10 };
    let obj2 = obj1;  // ⚠️ 'obj2' apunta al mismo objeto
    obj1.numero = 20;
    console.log("obj1:", obj1.numero, "obj2:", obj2.numero); // Ambos: 20
    
    // ✅ Para copiar objetos independientemente:
    let obj3 = { ...obj1 };        // Copia superficial
    let obj4 = JSON.parse(JSON.stringify(obj1)); // Copia profunda
}
```

### ⚡ **Optimización de Rendimiento**

```javascript
// 🎯 Técnicas para mejorar el rendimiento:
class OptimizacionEstructuras {
    
    // 1️⃣ REUTILIZACIÓN DE OBJETOS
    static ejemploReutilizacion() {
        // ❌ Creación excesiva de objetos
        function procesarDatosMalo(datos) {
            return datos.map(item => {
                return { // 🐛 Nuevo objeto en cada iteración
                    resultado: item * 2,
                    timestamp: new Date(), // 🐛 Nueva fecha cada vez
                    metadata: { procesado: true }
                };
            });
        }
        
        // ✅ Reutilización inteligente
        function procesarDatosBueno(datos) {
            const metadata = { procesado: true }; // ♻️ Reutilizar
            const baseTimestamp = Date.now();     // ♻️ Una sola vez
            
            return datos.map((item, index) => ({
                resultado: item * 2,
                timestamp: baseTimestamp + index,
                metadata // ♻️ Referencia compartida
            }));
        }
    }
    
    // 2️⃣ ESTRUCTURAS APROPIADAS PARA EL CONTEXTO
    static ejemploEstructurasApropiadas() {
        // 🎯 Para búsquedas frecuentes - Usa Map/Set
        const busquedasFrecuentes = new Map([
            ["user123", { nombre: "Juan", activo: true }],
            ["user456", { nombre: "María", activo: false }]
        ]);
        
        // 🎯 Para listas ordenadas - Usa Array
        const ranking = [
            { usuario: "Ana", puntos: 1500 },
            { usuario: "Luis", puntos: 1200 },
            { usuario: "Carmen", puntos: 900 }
        ];
        
        // 🎯 Para elementos únicos - Usa Set
        const tagsUnicos = new Set();
        const agregarTag = (tag) => tagsUnicos.add(tag.toLowerCase());
    }
    
    // 3️⃣ LAZY LOADING - Carga bajo demanda
    static ejemploLazyLoading() {
        class DataManager {
            constructor() {
                this._cache = new Map();
                this._datosCompletos = null;
            }
            
            // 💤 Solo carga cuando se necesita
            async obtenerDatos(id) {
                if (this._cache.has(id)) {
                    return this._cache.get(id);
                }
                
                const datos = await this.cargarDatos(id);
                this._cache.set(id, datos);
                return datos;
            }
            
            async cargarDatos(id) {
                // Simular carga de datos
                return new Promise(resolve => {
                    setTimeout(() => resolve({ id, data: `Datos para ${id}` }), 100);
                });
            }
        }
    }
}
```

### 📊 **Monitoreo de Memoria**

```javascript
// 🔍 Herramientas para monitorear el rendimiento:
class MonitoreoRendimiento {
    
    // ⏱️ Medir tiempo de ejecución
    static medirTiempo(nombre, funcion) {
        console.time(nombre);
        const resultado = funcion();
        console.timeEnd(nombre);
        return resultado;
    }
    
    // 💾 Monitorear uso de memoria (Node.js)
    static monitorearMemoria() {
        if (typeof process !== 'undefined') {
            const memoria = process.memoryUsage();
            console.log("📊 Uso de memoria:", {
                rss: `${Math.round(memoria.rss / 1024 / 1024 * 100) / 100} MB`,
                heapTotal: `${Math.round(memoria.heapTotal / 1024 / 1024 * 100) / 100} MB`,
                heapUsed: `${Math.round(memoria.heapUsed / 1024 / 1024 * 100) / 100} MB`
            });
        }
    }
    
    // 🧪 Benchmarking de estructuras
    static compararEstructuras() {
        const datos = Array.from({length: 10000}, (_, i) => i);
        
        // Array vs Set para búsquedas
        console.log("\n🔍 Comparación de búsquedas:");
        
        const array = datos;
        const set = new Set(datos);
        
        this.medirTiempo("Array.includes", () => {
            for(let i = 0; i < 1000; i++) {
                array.includes(Math.floor(Math.random() * 10000));
            }
        });
        
        this.medirTiempo("Set.has", () => {
            for(let i = 0; i < 1000; i++) {
                set.has(Math.floor(Math.random() * 10000));
            }
        });
    }
}

// 🚀 Ejecutar demostraciones
// MonitoreoRendimiento.compararEstructuras();
```

---

## 4. 🔢 **Arrays Básicos**

### 📚 **Fundamentos de Arrays**

```javascript
// 📊 Los Arrays son la estructura más versátil de JavaScript
const fundamentosArrays = {
    // 🏗️ CREACIÓN DE ARRAYS
    creacion: {
        // Método literal (recomendado)
        literal: [1, 2, 3, 4, 5],
        vacio: [],
        mixto: [1, "texto", true, null, { nombre: "Juan" }],
        
        // Constructor Array
        constructor: new Array(5), // Array vacío con 5 posiciones
        conDatos: new Array(1, 2, 3, 4, 5),
        
        // Métodos de creación
        fromRange: Array.from({length: 5}, (_, i) => i + 1),
        filled: Array(3).fill("JavaScript"),
        ofValues: Array.of(1, 2, 3, 4, 5)
    }
};

// 🎯 Ejemplos prácticos de creación
function ejemplosCreacionArrays() {
    // 📋 Lista de tareas
    const tareas = [
        "Revisar emails",
        "Estudiar JavaScript", 
        "Hacer ejercicio",
        "Leer documentación"
    ];
    
    // 🎮 Puntuaciones de juego
    const puntuaciones = [1500, 2300, 1800, 2100, 1650];
    
    // 👥 Información de usuarios
    const usuarios = [
        { id: 1, nombre: "Ana", activo: true },
        { id: 2, nombre: "Luis", activo: false },
        { id: 3, nombre: "Carmen", activo: true }
    ];
    
    // 🌍 Estructura multinivel
    const regiones = [
        {
            pais: "España",
            ciudades: ["Madrid", "Barcelona", "Valencia"],
            poblacion: 47000000
        },
        {
            pais: "México",
            ciudades: ["CDMX", "Guadalajara", "Monterrey"],
            poblacion: 128000000
        }
    ];
    
    return { tareas, puntuaciones, usuarios, regiones };
}
```

### 🔍 **Acceso y Manipulación Básica**

```javascript
// 🎯 Operaciones fundamentales con arrays
class ArrayBasico {
    
    // 📖 ACCESO A ELEMENTOS
    static ejemplosAcceso() {
        const frutas = ["🍎", "🍌", "🍊", "🍇", "🥝"];
        
        // Por índice (base 0)
        console.log("Primera fruta:", frutas[0]);        // 🍎
        console.log("Última fruta:", frutas[4]);         // 🥝
        console.log("Última (dinámico):", frutas[frutas.length - 1]); // 🥝
        
        // Índices negativos (no nativo, pero común)
        const obtenerDesdeAtras = (arr, pos) => arr[arr.length - pos];
        console.log("Penúltima:", obtenerDesdeAtras(frutas, 2)); // 🍇
        
        // Verificar existencia
        console.log("Índice 2 existe:", 2 < frutas.length);
        console.log("Índice 10 existe:", 10 < frutas.length);
        
        return frutas;
    }
    
    // ➕ AGREGADO DE ELEMENTOS
    static ejemplosAgregar() {
        let numeros = [1, 2, 3];
        
        // Al final
        numeros.push(4);                    // [1, 2, 3, 4]
        numeros.push(5, 6, 7);             // [1, 2, 3, 4, 5, 6, 7]
        
        // Al inicio
        numeros.unshift(0);                // [0, 1, 2, 3, 4, 5, 6, 7]
        numeros.unshift(-2, -1);           // [-2, -1, 0, 1, 2, 3, 4, 5, 6, 7]
        
        // En posición específica
        numeros.splice(2, 0, "NUEVO");     // [-2, -1, "NUEVO", 0, 1, 2, 3, 4, 5, 6, 7]
        
        console.log("📊 Array después de agregar:", numeros);
        return numeros;
    }
    
    // ➖ ELIMINACIÓN DE ELEMENTOS  
    static ejemplosEliminar() {
        let colores = ["rojo", "verde", "azul", "amarillo", "morado"];
        
        // Desde el final
        const ultimo = colores.pop();      // Remueve "morado"
        console.log("Eliminado:", ultimo, "Restantes:", colores);
        
        // Desde el inicio
        const primero = colores.shift();   // Remueve "rojo"
        console.log("Eliminado:", primero, "Restantes:", colores);
        
        // Por índice específico
        const eliminados = colores.splice(1, 1); // Remueve "azul"
        console.log("Eliminados:", eliminados, "Restantes:", colores);
        
        // Múltiples elementos
        colores.splice(0, 2);              // Remueve primeros 2
        console.log("Final:", colores);
        
        return colores;
    }
    
    // 🔄 MODIFICACIÓN DE ELEMENTOS
    static ejemplosModificar() {
        let estudiantes = [
            { nombre: "Ana", nota: 85 },
            { nombre: "Luis", nota: 92 },
            { nombre: "Carmen", nota: 78 }
        ];
        
        // Modificación directa
        estudiantes[0].nota = 90;
        
        // Reemplazar elemento completo
        estudiantes[2] = { nombre: "Carmen", nota: 82, mejorada: true };
        
        // Modificación con splice
        estudiantes.splice(1, 1, { nombre: "Luis", nota: 95, destacado: true });
        
        console.log("📚 Estudiantes modificados:", estudiantes);
        return estudiantes;
    }
}

// 🚀 Demostraciones prácticas
console.log("🔍 === DEMOS DE ARRAYS BÁSICOS ===");
ArrayBasico.ejemplosAcceso();
ArrayBasico.ejemplosAgregar();
ArrayBasico.ejemplosEliminar();
ArrayBasico.ejemplosModificar();
```

### 📊 **Propiedades y Métodos Esenciales**

```javascript
// 🔧 Propiedades y métodos que debes dominar
class PropiedadesArrays {
    
    // 📏 PROPIEDADES FUNDAMENTALES
    static propiedadesBasicas() {
        const datos = [10, 20, 30, 40, 50];
        
        console.log("📊 Propiedades del array:");
        console.log("Longitud:", datos.length);              // 5
        console.log("Constructor:", datos.constructor.name); // Array
        console.log("Es array:", Array.isArray(datos));     // true
        
        // Modificar longitud
        datos.length = 3;
        console.log("Después de reducir:", datos);          // [10, 20, 30]
        
        datos.length = 6;
        console.log("Después de aumentar:", datos);         // [10, 20, 30, empty × 3]
        
        return datos;
    }
    
    // 🔄 MÉTODOS DE CONVERSIÓN
    static metodosConversion() {
        const numeros = [1, 2, 3, 4, 5];
        const mixto = ["a", 1, true, null];
        
        console.log("🔄 Conversiones:");
        
        // A string
        console.log("toString():", numeros.toString());        // "1,2,3,4,5"
        console.log("join(' - '):", numeros.join(" - "));     // "1 - 2 - 3 - 4 - 5"
        console.log("join(''):", numeros.join(""));           // "12345"
        
        // Desde string
        const desdeCadena = "rojo,verde,azul".split(",");
        console.log("Desde string:", desdeCadena);            // ["rojo", "verde", "azul"]
        
        // Con JSON
        const jsonString = JSON.stringify(mixto);
        const desdeJson = JSON.parse(jsonString);
        console.log("JSON:", jsonString);
        console.log("Desde JSON:", desdeJson);
        
        return { numeros, mixto, desdeCadena };
    }
    
    // 🔍 MÉTODOS DE BÚSQUEDA BÁSICA
    static metodosBusqueda() {
        const frutas = ["manzana", "banana", "naranja", "banana", "kiwi"];
        const numeros = [10, 25, 30, 45, 50];
        
        console.log("🔍 Búsquedas básicas:");
        
        // Existencia
        console.log("Incluye 'banana':", frutas.includes("banana"));        // true
        console.log("Incluye 'pera':", frutas.includes("pera"));           // false
        
        // Índices
        console.log("Primer 'banana':", frutas.indexOf("banana"));         // 1
        console.log("Último 'banana':", frutas.lastIndexOf("banana"));     // 3
        console.log("Índice de 'pera':", frutas.indexOf("pera"));          // -1
        
        // Con condiciones
        const primerMayor30 = numeros.find(n => n > 30);
        const indiceMayor30 = numeros.findIndex(n => n > 30);
        
        console.log("Primer número > 30:", primerMayor30);                 // 45
        console.log("Índice primer > 30:", indiceMayor30);                 // 3
        
        return { frutas, numeros };
    }
    
    // 📋 COPIA Y CLONADO
    static metodosCopiado() {
        const original = [1, { nombre: "Juan" }, [2, 3]];
        
        console.log("📋 Métodos de copiado:");
        
        // Copia superficial (shallow copy)
        const copia1 = [...original];                    // Spread operator
        const copia2 = Array.from(original);             // Array.from
        const copia3 = original.slice();                 // slice sin parámetros
        
        // ⚠️ Las copias superficiales comparten objetos internos
        copia1[1].nombre = "María";
        console.log("Original afectado:", original[1].nombre); // "María"
        
        // ✅ Copia profunda (deep copy)
        const copiaConCompleta = JSON.parse(JSON.stringify(original));
        copiaConCompleta[1].nombre = "Carlos";
        console.log("Original no afectado:", original[1].nombre); // "María"
        
        return { original, copia1, copiaConCompleta };
    }
}

// 🎯 Ejemplo integral: Gestión de inventario
class GestorInventario {
    constructor() {
        this.productos = [];
        this.historialCambios = [];
    }
    
    // ➕ Agregar producto
    agregarProducto(producto) {
        producto.id = this.productos.length + 1;
        producto.fechaCreacion = new Date();
        this.productos.push(producto);
        this.registrarCambio("AGREGAR", producto.id);
        return producto.id;
    }
    
    // 🔍 Buscar productos
    buscarPorNombre(nombre) {
        return this.productos.filter(p => 
            p.nombre.toLowerCase().includes(nombre.toLowerCase())
        );
    }
    
    // 📊 Obtener estadísticas
    obtenerEstadisticas() {
        return {
            total: this.productos.length,
            valorTotal: this.productos.reduce((sum, p) => sum + p.precio, 0),
            categorias: [...new Set(this.productos.map(p => p.categoria))],
            cambiosRecientes: this.historialCambios.slice(-5)
        };
    }
    
    // 📝 Registrar cambios
    registrarCambio(accion, productoPorId) {
        this.historialCambios.push({
            accion,
            productoPorId,
            timestamp: new Date()
        });
    }
}

// 🚀 Demo del gestor
function demoGestorInventario() {
    const gestor = new GestorInventario();
    
    gestor.agregarProducto({ nombre: "Laptop", precio: 1200, categoria: "Electrónicos" });
    gestor.agregarProducto({ nombre: "Silla", precio: 150, categoria: "Muebles" });
    gestor.agregarProducto({ nombre: "Smartphone", precio: 800, categoria: "Electrónicos" });
    
    console.log("🛍️ Productos con 'a':", gestor.buscarPorNombre("a"));
    console.log("📊 Estadísticas:", gestor.obtenerEstadisticas());
}

// demoGestorInventario();
```

---

## 5. ⚡ **Métodos de Arrays**

### 🎯 **Introducción a los Métodos de Arrays**

Los métodos de arrays son la **herramienta más poderosa** para manipular y transformar datos en JavaScript. Son la diferencia entre código básico y código elegante.

```javascript
// 🔄 Los métodos de arrays se dividen en categorías:
const categoriaMetodos = {
    // 🔍 BÚSQUEDA Y FILTRADO
    busqueda: ["find", "findIndex", "filter", "includes", "indexOf"],
    
    // 🔄 TRANSFORMACIÓN
    transformacion: ["map", "flatMap", "reduce", "reduceRight"],
    
    // ✅ VALIDACIÓN
    validacion: ["every", "some"],
    
    // 🎯 ITERACIÓN
    iteracion: ["forEach", "entries", "keys", "values"],
    
    // 🏗️ CONSTRUCCIÓN
    construccion: ["concat", "slice", "splice", "join"],
    
    // 📊 ORDENAMIENTO
    ordenamiento: ["sort", "reverse"],
    
    // 🔧 MODIFICACIÓN
    modificacion: ["push", "pop", "shift", "unshift", "fill"]
};

console.log("⚡ JavaScript tiene más de 30 métodos de arrays integrados");
```

### 🔍 **Métodos de Búsqueda y Filtrado**

```javascript
// 🔍 Los métodos más útiles para encontrar y filtrar elementos
class MetodosBusqueda {
    
    // 🎯 FIND - Encuentra el primer elemento que cumple condición
    static ejemplosFind() {
        const usuarios = [
            { id: 1, nombre: "Ana", edad: 25, activo: true },
            { id: 2, nombre: "Luis", edad: 30, activo: false },
            { id: 3, nombre: "Carmen", edad: 28, activo: true },
            { id: 4, nombre: "Juan", edad: 35, activo: false }
        ];
        
        // Buscar primer usuario activo
        const primerActivo = usuarios.find(user => user.activo);
        console.log("Primer activo:", primerActivo); // { id: 1, nombre: "Ana", ... }
        
        // Buscar por edad específica
        const usuario30 = usuarios.find(user => user.edad === 30);
        console.log("Usuario de 30:", usuario30); // { id: 2, nombre: "Luis", ... }
        
        // Si no encuentra, retorna undefined
        const noExiste = usuarios.find(user => user.edad > 50);
        console.log("No existe:", noExiste); // undefined
        
        return usuarios;
    }
    
    // � FINDINDEX - Encuentra el índice del primer elemento
    static ejemplosFindIndex() {
        const productos = [
            { codigo: "A001", precio: 100, categoria: "electronicos" },
            { codigo: "B002", precio: 250, categoria: "ropa" },
            { codigo: "C003", precio: 75, categoria: "electronicos" },
            { codigo: "D004", precio: 180, categoria: "hogar" }
        ];
        
        // Encontrar índice del primer producto caro
        const indiceCaro = productos.findIndex(p => p.precio > 200);
        console.log("Índice producto caro:", indiceCaro); // 1
        
        // Usar el índice para modificar
        if (indiceCaro !== -1) {
            productos[indiceCaro].descuento = 10;
            console.log("Producto con descuento:", productos[indiceCaro]);
        }
        
        return productos;
    }
    
    // 🔎 FILTER - Filtra elementos que cumplen condición
    static ejemplosFilter() {
        const ventas = [
            { mes: "enero", monto: 15000, vendedor: "Ana" },
            { mes: "febrero", monto: 22000, vendedor: "Luis" },
            { mes: "marzo", monto: 18000, vendedor: "Ana" },
            { mes: "abril", monto: 25000, vendedor: "Carmen" },
            { mes: "mayo", monto: 19000, vendedor: "Luis" }
        ];
        
        // Filtrar ventas altas (>20000)
        const ventasAltas = ventas.filter(venta => venta.monto > 20000);
        console.log("Ventas altas:", ventasAltas);
        
        // Filtrar por vendedor específico
        const ventasAna = ventas.filter(venta => venta.vendedor === "Ana");
        console.log("Ventas de Ana:", ventasAna);
        
        // Combinar múltiples condiciones
        const ventasLuisAltas = ventas.filter(venta => 
            venta.vendedor === "Luis" && venta.monto > 20000
        );
        console.log("Ventas altas de Luis:", ventasLuisAltas);
        
        return { ventasAltas, ventasAna, ventasLuisAltas };
    }
    
    // ✅ INCLUDES - Verifica si existe un elemento
    static ejemplosIncludes() {
        const tecnologias = ["HTML", "CSS", "JavaScript", "React", "Node.js"];
        const numeros = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10];
        
        // Verificar existencia
        console.log("Conoce React:", tecnologias.includes("React")); // true
        console.log("Conoce Vue:", tecnologias.includes("Vue")); // false
        
        // Con números
        console.log("Tiene número 7:", numeros.includes(7)); // true
        console.log("Tiene número 15:", numeros.includes(15)); // false
        
        // Con segundo parámetro (desde qué índice buscar)
        console.log("React después del índice 2:", tecnologias.includes("React", 3)); // true
        console.log("JavaScript después del índice 3:", tecnologias.includes("JavaScript", 3)); // false
        
        return { tecnologias, numeros };
    }
}

// 🚀 Demostraciones
console.log("🔍 MÉTODOS DE BÚSQUEDA");
MetodosBusqueda.ejemplosFind();
MetodosBusqueda.ejemplosFindIndex();
MetodosBusqueda.ejemplosFilter();
MetodosBusqueda.ejemplosIncludes();
```

### 🔄 **Métodos de Transformación**

```javascript
// 🔄 Los métodos más poderosos para transformar datos
class MetodosTransformacion {
    
    // 🗺️ MAP - Transforma cada elemento del array
    static ejemplosMap() {
        const numeros = [1, 2, 3, 4, 5];
        const empleados = [
            { nombre: "Ana", salario: 3000 },
            { nombre: "Luis", salario: 3500 },
            { nombre: "Carmen", salario: 4000 }
        ];
        
        // Transformaciones simples
        const cuadrados = numeros.map(n => n * n);
        console.log("Cuadrados:", cuadrados); // [1, 4, 9, 16, 25]
        
        const dobles = numeros.map(n => n * 2);
        console.log("Dobles:", dobles); // [2, 4, 6, 8, 10]
        
        // Transformar objetos
        const empleadosConBono = empleados.map(emp => ({
            ...emp,
            salarioConBono: emp.salario * 1.1,
            categoria: emp.salario > 3500 ? "Senior" : "Junior"
        }));
        console.log("Con bonos:", empleadosConBono);
        
        // Extraer solo nombres
        const soloNombres = empleados.map(emp => emp.nombre);
        console.log("Solo nombres:", soloNombres); // ["Ana", "Luis", "Carmen"]
        
        // Con índice
        const conIndice = numeros.map((valor, indice) => ({
            posicion: indice,
            valor: valor,
            esPar: valor % 2 === 0
        }));
        console.log("Con índices:", conIndice);
        
        return { cuadrados, empleadosConBono, soloNombres };
    }
    
    // 🎯 REDUCE - Reduce array a un solo valor
    static ejemplosReduce() {
        const numeros = [1, 2, 3, 4, 5];
        const compras = [
            { producto: "Laptop", precio: 1200, cantidad: 1 },
            { producto: "Mouse", precio: 25, cantidad: 2 },
            { producto: "Teclado", precio: 75, cantidad: 1 },
            { producto: "Monitor", precio: 300, cantidad: 2 }
        ];
        
        // Suma básica
        const suma = numeros.reduce((acum, num) => acum + num, 0);
        console.log("Suma:", suma); // 15
        
        // Producto (multiplicación)
        const producto = numeros.reduce((acum, num) => acum * num, 1);
        console.log("Producto:", producto); // 120
        
        // Total de compras
        const totalCompras = compras.reduce((total, item) => 
            total + (item.precio * item.cantidad), 0
        );
        console.log("Total compras:", totalCompras); // 1925
        
        // Encontrar el más caro  
        const masCaro = compras.reduce((caro, actual) => 
            actual.precio > caro.precio ? actual : caro
        );
        console.log("Más caro:", masCaro);
        
        // Contar por categorías
        const palabras = ["hola", "mundo", "javascript", "es", "genial"];
        const contadorLetras = palabras.reduce((contador, palabra) => {
            const longitud = palabra.length;
            contador[longitud] = (contador[longitud] || 0) + 1;
            return contador;
        }, {});
        console.log("Contador por longitud:", contadorLetras);
        
        // Agrupar objetos
        const agrupados = compras.reduce((grupos, item) => {
            const categoria = item.precio > 100 ? "caro" : "barato";
            if (!grupos[categoria]) grupos[categoria] = [];
            grupos[categoria].push(item);
            return grupos;
        }, {});
        console.log("Agrupados:", agrupados);
        
        return { suma, totalCompras, masCaro, agrupados };
    }
    
    // 🔀 FLATMAP - Map + aplanar en una operación
    static ejemplosFlatMap() {
        const frases = ["Hola mundo", "JavaScript es genial", "Programar es divertido"];
        const numeros = [1, 2, 3, 4];
        
        // Dividir frases en palabras
        const palabras = frases.flatMap(frase => frase.split(" "));
        console.log("Palabras:", palabras);
        // ["Hola", "mundo", "JavaScript", "es", "genial", "Programar", "es", "divertido"]
        
        // Generar múltiples valores por elemento
        const duplicados = numeros.flatMap(n => [n, n * 2]);
        console.log("Duplicados:", duplicados); // [1, 2, 2, 4, 3, 6, 4, 8]
        
        // Ejemplo práctico: extraer tags de posts
        const posts = [
            { titulo: "Intro a JS", tags: ["javascript", "principiante"] },
            { titulo: "React Hooks", tags: ["react", "hooks", "avanzado"] },
            { titulo: "CSS Grid", tags: ["css", "layout"] }
        ];
        
        const todosLosTags = posts.flatMap(post => post.tags);
        console.log("Todos los tags:", todosLosTags);
        
        // Tags únicos
        const tagsUnicos = [...new Set(todosLosTags)];
        console.log("Tags únicos:", tagsUnicos);
        
        return { palabras, duplicados, tagsUnicos };
    }
}

// 🚀 Demostraciones
console.log("� MÉTODOS DE TRANSFORMACIÓN");
MetodosTransformacion.ejemplosMap();
MetodosTransformacion.ejemplosReduce();
MetodosTransformacion.ejemplosFlatMap();
```

### ✅ **Métodos de Validación**

```javascript
// ✅ Métodos para validar condiciones en arrays
class MetodosValidacion {
    
    // 🎯 EVERY - Verifica si TODOS los elementos cumplen condición
    static ejemplosEvery() {
        const numeros = [2, 4, 6, 8, 10];
        const numerosImpar = [1, 3, 5, 7, 9];
        const numerosMixtos = [2, 4, 5, 8, 10];
        
        const usuarios = [
            { nombre: "Ana", edad: 25, activo: true },
            { nombre: "Luis", edad: 30, activo: true },
            { nombre: "Carmen", edad: 28, activo: true }
        ];
        
        // Verificar si todos son pares
        const todosPares = numeros.every(n => n % 2 === 0);
        console.log("Todos pares:", todosPares); // true
        
        const mixtosPares = numerosMixtos.every(n => n % 2 === 0);
        console.log("Mixtos todos pares:", mixtosPares); // false
        
        // Verificar usuarios activos
        const todosActivos = usuarios.every(user => user.activo);
        console.log("Todos activos:", todosActivos); // true
        
        // Verificar edades mínimas
        const todosAdultos = usuarios.every(user => user.edad >= 18);
        console.log("Todos adultos:", todosAdultos); // true
        
        // Caso práctico: validar formulario
        const formulario = [
            { campo: "nombre", valor: "Juan", valido: true },
            { campo: "email", valor: "juan@email.com", valido: true },
            { campo: "edad", valor: "25", valido: true }
        ];
        
        const formularioValido = formulario.every(campo => campo.valido);
        console.log("Formulario válido:", formularioValido); // true
        
        return { todosPares, todosActivos, formularioValido };
    }
    
    // 🔍 SOME - Verifica si AL MENOS UNO cumple condición
    static ejemplosSome() {
        const numeros = [1, 3, 5, 7, 8];
        const productos = [
            { nombre: "Laptop", precio: 1200, oferta: false },
            { nombre: "Mouse", precio: 25, oferta: true },
            { nombre: "Teclado", precio: 75, oferta: false }
        ];
        
        // Verificar si hay algún par
        const hayPares = numeros.some(n => n % 2 === 0);
        console.log("Hay pares:", hayPares); // true (el 8)
        
        // Verificar si hay números grandes
        const hayGrandes = numeros.some(n => n > 100);
        console.log("Hay grandes:", hayGrandes); // false
        
        // Verificar ofertas
        const hayOfertas = productos.some(p => p.oferta);
        console.log("Hay ofertas:", hayOfertas); // true
        
        // Verificar productos caros
        const hayCaros = productos.some(p => p.precio > 1000);
        console.log("Hay productos caros:", hayCaros); // true
        
        // Caso práctico: permisos de usuario
        const permisos = ["leer", "escribir"];
        const tieneAdmin = permisos.some(permiso => permiso === "admin");
        const tieneEscritura = permisos.some(permiso => permiso === "escribir");
        
        console.log("Tiene permisos admin:", tieneAdmin); // false
        console.log("Tiene permisos escritura:", tieneEscritura); // true
        
        return { hayPares, hayOfertas, tieneEscritura };
    }
    
    // � Combinando EVERY y SOME
    static ejemplosCombinados() {
        const estudiantes = [
            { nombre: "Ana", notas: [8, 9, 7, 8] },
            { nombre: "Luis", notas: [6, 7, 8, 5] },
            { nombre: "Carmen", notas: [9, 10, 9, 8] },
            { nombre: "Juan", notas: [4, 5, 6, 3] }
        ];
        
        // Estudiantes que tienen todas las notas aprobadas (>= 6)
        const todosAprobados = estudiantes.filter(est => 
            est.notas.every(nota => nota >= 6)
        );
        console.log("Todos aprobados:", todosAprobados.map(e => e.nombre));
        
        // Estudiantes que tienen al menos una nota excelente (>= 9)
        const conExcelencia = estudiantes.filter(est => 
            est.notas.some(nota => nota >= 9)
        );
        console.log("Con excelencia:", conExcelencia.map(e => e.nombre));
        
        // Verificar si toda la clase tiene al menos una nota aprobada
        const claseAprobada = estudiantes.every(est => 
            est.notas.some(nota => nota >= 6)
        );
        console.log("Clase aprobada:", claseAprobada);
        
        // Verificar si hay algún estudiante con todas las notas excelentes
        const hayExcelente = estudiantes.some(est => 
            est.notas.every(nota => nota >= 9)
        );
        console.log("Hay estudiante excelente:", hayExcelente);
        
        return { todosAprobados, conExcelencia, claseAprobada };
    }
}

// 🚀 Demostraciones
console.log("✅ MÉTODOS DE VALIDACIÓN");
MetodosValidacion.ejemplosEvery();
MetodosValidacion.ejemplosSome();
MetodosValidacion.ejemplosCombinados();
```

### 🎯 **Métodos de Iteración**

```javascript
// 🎯 Métodos para recorrer y procesar arrays
class MetodosIteracion {
    
    // 🔄 FOREACH - Ejecuta función para cada elemento
    static ejemplosForEach() {
        const productos = [
            { id: 1, nombre: "Laptop", precio: 1200 },
            { id: 2, nombre: "Mouse", precio: 25 },
            { id: 3, nombre: "Teclado", precio: 75 }
        ];
        
        // Iterar básico
        console.log("� Lista de productos:");
        productos.forEach(producto => {
            console.log(`- ${producto.nombre}: $${producto.precio}`);
        });
        
        // Con índice
        console.log("\n📊 Productos numerados:");
        productos.forEach((producto, indice) => {
            console.log(`${indice + 1}. ${producto.nombre}`);
        });
        
        // Modificar elementos (cuidado: modifica el original)
        console.log("\n💰 Aplicando descuento del 10%:");
        productos.forEach(producto => {
            producto.precioConDescuento = producto.precio * 0.9;
        });
        productos.forEach(p => 
            console.log(`${p.nombre}: $${p.precio} -> $${p.precioConDescuento}`)
        );
        
        // Caso práctico: envío de emails
        const usuarios = ["ana@email.com", "luis@email.com", "carmen@email.com"];
        console.log("\n📧 Enviando emails:");
        usuarios.forEach((email, indice) => {
            // Simular envío de email
            setTimeout(() => {
                console.log(`✅ Email enviado a ${email}`);
            }, indice * 1000);
        });
        
        return productos;
    }
    
    // 🔑 ENTRIES, KEYS, VALUES - Iteradores especiales
    static ejemplosIteradores() {
        const tecnologias = ["HTML", "CSS", "JavaScript", "React"];
        
        console.log("🔑 Métodos iteradores:");
        
        // KEYS - Obtiene los índices
        console.log("Índices:", Array.from(tecnologias.keys())); // [0, 1, 2, 3]
        
        // VALUES - Obtiene los valores (igual que el array)
        console.log("Valores:", Array.from(tecnologias.values())); // ["HTML", "CSS", ...]
        
        // ENTRIES - Obtiene pares [índice, valor]
        console.log("Entradas:", Array.from(tecnologias.entries()));
        // [[0, "HTML"], [1, "CSS"], [2, "JavaScript"], [3, "React"]]
        
        // Uso práctico con for...of
        console.log("\n🔄 Iterando con for...of:");
        for (const [indice, tecnologia] of tecnologias.entries()) {
            console.log(`${indice}: ${tecnologia}`);
        }
        
        // Caso práctico: crear índice de búsqueda
        const indice = {};
        for (const [pos, tech] of tecnologias.entries()) {
            indice[tech.toLowerCase()] = pos;
        }
        console.log("Índice de búsqueda:", indice);
        
        return { tecnologias, indice };
    }
    
    // 🔧 Métodos de iteración personalizados
    static ejemplosPersonalizados() {
        const numeros = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10];
        
        // Función personalizada: procesarConCondicion
        function procesarConCondicion(array, condicion, procesador) {
            const resultados = [];
            array.forEach((elemento, indice) => {
                if (condicion(elemento, indice)) {
                    resultados.push(procesador(elemento, indice));
                }
            });
            return resultados;
        }
        
        // Procesar solo números pares, multiplicándolos por 3
        const paresTriplicados = procesarConCondicion(
            numeros,
            num => num % 2 === 0,  // condición
            num => num * 3         // procesador
        );
        console.log("Pares triplicados:", paresTriplicados); // [6, 12, 18, 24, 30]
        
        // Función personalizada: iterarConDelay
        async function iterarConDelay(array, callback, delay = 1000) {
            for (let i = 0; i < array.length; i++) {
                await new Promise(resolve => setTimeout(resolve, delay));
                callback(array[i], i);
            }
        }
        
        // Uso: mostrar elementos con delay
        const frutas = ["🍎", "🍌", "🍊"];
        console.log("🍓 Mostrando frutas con delay:");
        // iterarConDelay(frutas, (fruta, i) => console.log(`${i}: ${fruta}`), 500);
        
        return { paresTriplicados };
    }
}

// 🚀 Demostraciones
console.log("🎯 MÉTODOS DE ITERACIÓN");
MetodosIteracion.ejemplosForEach();
MetodosIteracion.ejemplosIteradores();
MetodosIteracion.ejemplosPersonalizados();
```

### 🧩 **Encadenamiento de Métodos (Method Chaining)**

```javascript
// 🧩 El poder real: combinar múltiples métodos
class EncadenamientoMetodos {
    
    // 🎯 Ejemplos básicos de encadenamiento
    static ejemplosBasicos() {
        const ventas = [
            { vendedor: "Ana", mes: "enero", monto: 15000, region: "norte" },
            { vendedor: "Luis", mes: "enero", monto: 22000, region: "sur" },
            { vendedor: "Carmen", mes: "enero", monto: 18000, region: "norte" },
            { vendedor: "Ana", mes: "febrero", monto: 25000, region: "norte" },
            { vendedor: "Luis", mes: "febrero", monto: 19000, region: "sur" },
            { vendedor: "Juan", mes: "febrero", monto: 21000, region: "centro" }
        ];
        
        // Encontrar vendedores top del norte con ventas > 20000
        const topVendedoresNorte = ventas
            .filter(venta => venta.region === "norte")
            .filter(venta => venta.monto > 20000)
            .map(venta => venta.vendedor)
            .filter((vendedor, indice, arr) => arr.indexOf(vendedor) === indice); // únicos
        
        console.log("Top vendedores norte:", topVendedoresNorte);
        
        // Calcular promedio de ventas por región
        const promediosPorRegion = ventas
            .reduce((acc, venta) => {
                if (!acc[venta.region]) {
                    acc[venta.region] = { total: 0, cantidad: 0 };
                }
                acc[venta.region].total += venta.monto;
                acc[venta.region].cantidad += 1;
                return acc;
            }, {});
        
        // Convertir a formato más legible
        const promediosFormateados = Object.entries(promediosPorRegion)
            .map(([region, datos]) => ({
                region,
                promedio: Math.round(datos.total / datos.cantidad)
            }))
            .sort((a, b) => b.promedio - a.promedio);
        
        console.log("Promedios por región:", promediosFormateados);
        
        return { topVendedoresNorte, promediosFormateados };
    }
    
    // 🚀 Casos de uso avanzados
    static casosAvanzados() {
        const estudiantes = [
            { 
                nombre: "Ana", 
                materias: [
                    { nombre: "Matemáticas", nota: 8.5 },
                    { nombre: "Física", nota: 7.8 },
                    { nombre: "Química", nota: 9.2 }
                ]
            },
            { 
                nombre: "Luis", 
                materias: [
                    { nombre: "Matemáticas", nota: 7.2 },
                    { nombre: "Física", nota: 8.1 },
                    { nombre: "Historia", nota: 9.0 }
                ]
            },
            { 
                nombre: "Carmen", 
                materias: [
                    { nombre: "Matemáticas", nota: 9.5 },
                    { nombre: "Química", nota: 8.8 },
                    { nombre: "Historia", nota: 8.3 }
                ]
            }
        ];
        
        // Ranking de estudiantes por promedio
        const ranking = estudiantes
            .map(estudiante => ({
                ...estudiante,
                promedio: estudiante.materias.reduce((sum, m) => sum + m.nota, 0) / estudiante.materias.length
            }))
            .sort((a, b) => b.promedio - a.promedio)
            .map((estudiante, indice) => ({
                posicion: indice + 1,
                nombre: estudiante.nombre,
                promedio: Math.round(estudiante.promedio * 100) / 100,
                materias: estudiante.materias.length
            }));
        
        console.log("� Ranking de estudiantes:");
        ranking.forEach(est => 
            console.log(`${est.posicion}. ${est.nombre}: ${est.promedio} (${est.materias} materias)`)
        );
        
        // Mejores estudiantes por materia
        const mejoresPorMateria = estudiantes
            .flatMap(est => 
                est.materias.map(materia => ({
                    estudiante: est.nombre,
                    materia: materia.nombre,
                    nota: materia.nota
                }))
            )
            .reduce((acc, item) => {
                if (!acc[item.materia] || acc[item.materia].nota < item.nota) {
                    acc[item.materia] = item;
                }
                return acc;
            }, {});
        
        console.log("🎓 Mejores por materia:", mejoresPorMateria);
        
        return { ranking, mejoresPorMateria };
    }
    
    // 🔧 Pipeline de procesamiento de datos
    static pipelineDatos() {
        const transacciones = [
            { id: 1, tipo: "ingreso", monto: 5000, fecha: "2024-01-15", categoria: "salario" },
            { id: 2, tipo: "gasto", monto: 1200, fecha: "2024-01-16", categoria: "alquiler" },
            { id: 3, tipo: "gasto", monto: 300, fecha: "2024-01-17", categoria: "comida" },
            { id: 4, tipo: "ingreso", monto: 2000, fecha: "2024-01-18", categoria: "freelance" },
            { id: 5, tipo: "gasto", monto: 150, fecha: "2024-01-19", categoria: "transporte" },
            { id: 6, tipo: "gasto", monto: 800, fecha: "2024-01-20", categoria: "comida" },
        ];
        
        // Pipeline completo de análisis financiero
        const analisisFinanciero = transacciones
            // 1. Agregar mes para agrupación
            .map(t => ({
                ...t,
                mes: t.fecha.substring(0, 7), // "2024-01"
                montoConSigno: t.tipo === "ingreso" ? t.monto : -t.monto
            }))
            // 2. Filtrar transacciones significativas (> 200)
            .filter(t => t.monto > 200)
            // 3. Ordenar por fecha
            .sort((a, b) => new Date(a.fecha) - new Date(b.fecha))
            // 4. Calcular balance acumulado
            .reduce((acc, transaccion, indice) => {
                const balanceAnterior = indice > 0 ? acc[indice - 1].balanceAcumulado : 0;
                acc.push({
                    ...transaccion,
                    balanceAcumulado: balanceAnterior + transaccion.montoConSigno
                });
                return acc;
            }, []);
        
        console.log("💰 Análisis financiero:");
        analisisFinanciero.forEach(t => 
            console.log(`${t.fecha}: ${t.tipo} $${t.monto} (Balance: $${t.balanceAcumulado})`)
        );
        
        // Resumen por categoría
        const resumenCategoria = transacciones
            .reduce((acc, t) => {
                if (!acc[t.categoria]) {
                    acc[t.categoria] = { ingresos: 0, gastos: 0, neto: 0 };
                }
                if (t.tipo === "ingreso") {
                    acc[t.categoria].ingresos += t.monto;
                } else {
                    acc[t.categoria].gastos += t.monto;
                }
                acc[t.categoria].neto = acc[t.categoria].ingresos - acc[t.categoria].gastos;
                return acc;
            }, {});
        
        console.log("� Resumen por categoría:", resumenCategoria);
        
        return { analisisFinanciero, resumenCategoria };
    }
}

// 🚀 Demostraciones
console.log("🧩 ENCADENAMIENTO DE MÉTODOS");
EncadenamientoMetodos.ejemplosBasicos();
EncadenamientoMetodos.casosAvanzados();
EncadenamientoMetodos.pipelineDatos();
```

**✅ CAPÍTULO 5 COMPLETADO**

### 🎯 **Lo que acabamos de cubrir:**

1. **🔍 Búsqueda y Filtrado** - find, findIndex, filter, includes
2. **🔄 Transformación** - map, reduce, flatMap con casos reales
3. **✅ Validación** - every, some para verificar condiciones
4. **🎯 Iteración** - forEach, entries, keys, values
5. **🧩 Encadenamiento** - Combinar métodos para pipelines potentes

---

## 6. 🎯 **Arrays Avanzados**

### 🌟 **Introducción a Arrays Avanzados**

Los arrays avanzados van más allá de listas simples. Incluyen matrices multidimensionales, técnicas de optimización y patrones avanzados que encuentras en aplicaciones del mundo real.

```javascript
// 🎯 Los arrays avanzados incluyen:
const tiposArraysAvanzados = {
    // 📊 MULTIDIMENSIONALES
    matrices: [
        [1, 2, 3],
        [4, 5, 6],
        [7, 8, 9]
    ],
    
    // 🕳️ SPARSE ARRAYS (con huecos)
    sparse: [1, , , 4, , 6], // elementos undefined en posiciones 1, 2, 4
    
    // 🔢 TYPED ARRAYS (para rendimiento)
    typedArrays: {
        enteros: new Int32Array([1, 2, 3, 4]),
        flotantes: new Float64Array([1.1, 2.2, 3.3])
    },
    
    // 🎛️ ARRAY-LIKE OBJECTS
    arrayLike: {
        0: "primer",
        1: "segundo", 
        2: "tercero",
        length: 3
    }
};

console.log("🎯 Explorando arrays más allá de lo básico");
```

### 📊 **Arrays Multidimensionales (Matrices)**

```javascript
// 📊 Trabajando con matrices y estructuras bidimensionales
class ArraysMultidimensionales {
    
    // 🏗️ CREACIÓN DE MATRICES
    static crearMatrices() {
        // Matriz 2D básica
        const matriz2D = [
            [1, 2, 3],
            [4, 5, 6],
            [7, 8, 9]
        ];
        
        // Crear matriz de ceros
        const filas = 3, columnas = 4;
        const matrizCeros = Array(filas).fill(null).map(() => Array(columnas).fill(0));
        console.log("Matriz de ceros:", matrizCeros);
        
        // Crear matriz con valores específicos
        const matrizSecuencial = Array(3).fill(null).map((_, i) => 
            Array(3).fill(null).map((_, j) => i * 3 + j + 1)
        );
        console.log("Matriz secuencial:", matrizSecuencial);
        
        // Matriz de identidad
        const tamaño = 4;
        const identidad = Array(tamaño).fill(null).map((_, i) => 
            Array(tamaño).fill(null).map((_, j) => i === j ? 1 : 0)
        );
        console.log("Matriz identidad:", identidad);
        
        return { matriz2D, matrizCeros, identidad };
    }
    
    // 🔍 NAVEGACIÓN Y ACCESO
    static navegarMatrices() {
        const tablero = [
            ['♜', '♞', '♝', '♛', '♚', '♝', '♞', '♜'],
            ['♟', '♟', '♟', '♟', '♟', '♟', '♟', '♟'],
            [' ', ' ', ' ', ' ', ' ', ' ', ' ', ' '],
            [' ', ' ', ' ', ' ', ' ', ' ', ' ', ' '],
            [' ', ' ', ' ', ' ', ' ', ' ', ' ', ' '],
            [' ', ' ', ' ', ' ', ' ', ' ', ' ', ' '],
            ['♙', '♙', '♙', '♙', '♙', '♙', '♙', '♙'],
            ['♖', '♘', '♗', '♕', '♔', '♗', '♘', '♖']
        ];
        
        // Acceso por coordenadas
        console.log("Pieza en (0,4):", tablero[0][4]); // ♚ (Rey negro)
        
        // Iterar por filas
        console.log("🏁 Tablero de ajedrez:");
        tablero.forEach((fila, i) => {
            console.log(`${8-i} ${fila.join(' ')}`);
        });
        
        // Obtener columna específica
        const obtenerColumna = (matriz, col) => matriz.map(fila => fila[col]);
        const primeraColumna = obtenerColumna(tablero, 0);
        console.log("Primera columna:", primeraColumna);
        
        // Obtener diagonal
        const diagonal = tablero.map((fila, i) => fila[i]);
        console.log("Diagonal principal:", diagonal);
        
        return tablero;
    }
    
    // 🔄 OPERACIONES CON MATRICES
    static operacionesMatrices() {
        const matrizA = [
            [1, 2, 3],
            [4, 5, 6]
        ];
        
        const matrizB = [
            [7, 8, 9],
            [10, 11, 12]
        ];
        
        // Suma de matrices
        const sumarMatrices = (a, b) => 
            a.map((fila, i) => fila.map((val, j) => val + b[i][j]));
        
        const suma = sumarMatrices(matrizA, matrizB);
        console.log("Suma de matrices:", suma);
        
        // Transponer matriz
        const transponer = (matriz) => 
            matriz[0].map((_, colIndex) => matriz.map(fila => fila[colIndex]));
        
        const transpuesta = transponer(matrizA);
        console.log("Matriz original:", matrizA);
        console.log("Matriz transpuesta:", transpuesta);
        
        // Encontrar máximo en matriz
        const encontrarMaximo = (matriz) => 
            Math.max(...matriz.flat());
        
        const maximo = encontrarMaximo(matrizA);
        console.log("Máximo en matriz:", maximo);
        
        // Aplicar función a toda la matriz
        const aplicarFuncion = (matriz, fn) => 
            matriz.map(fila => fila.map(fn));
        
        const matrizCuadrados = aplicarFuncion(matrizA, x => x * x);
        console.log("Matriz de cuadrados:", matrizCuadrados);
        
        return { suma, transpuesta, matrizCuadrados };
    }
    
    // 🎮 EJEMPLO PRÁCTICO: JUEGO DE LA VIDA
    static juegoDelaVida() {
        // Implementación simplificada del Juego de la Vida de Conway
        const crearTablero = (filas, cols) => 
            Array(filas).fill(null).map(() => Array(cols).fill(0));
        
        const colocarPatron = (tablero, patron, startRow, startCol) => {
            patron.forEach((fila, i) => {
                fila.forEach((celda, j) => {
                    if (startRow + i < tablero.length && startCol + j < tablero[0].length) {
                        tablero[startRow + i][startCol + j] = celda;
                    }
                });
            });
        };
        
        const contarVecinos = (tablero, fila, col) => {
            const direcciones = [
                [-1, -1], [-1, 0], [-1, 1],
                [0, -1],           [0, 1],
                [1, -1],  [1, 0],  [1, 1]
            ];
            
            return direcciones.reduce((count, [df, dc]) => {
                const nuevaFila = fila + df;
                const nuevaCol = col + dc;
                if (nuevaFila >= 0 && nuevaFila < tablero.length && 
                    nuevaCol >= 0 && nuevaCol < tablero[0].length) {
                    count += tablero[nuevaFila][nuevaCol];
                }
                return count;
            }, 0);
        };
        
        const siguienteGeneracion = (tablero) => {
            const nuevo = crearTablero(tablero.length, tablero[0].length);
            for (let i = 0; i < tablero.length; i++) {
                for (let j = 0; j < tablero[0].length; j++) {
                    const vecinos = contarVecinos(tablero, i, j);
                    const estaVivo = tablero[i][j] === 1;
                    
                    if (estaVivo && (vecinos === 2 || vecinos === 3)) {
                        nuevo[i][j] = 1; // Sobrevive
                    } else if (!estaVivo && vecinos === 3) {
                        nuevo[i][j] = 1; // Nace
                    }
                    // En otros casos muere o permanece muerto (0)
                }
            }
            return nuevo;
        };
        
        // Crear tablero y patrón "glider"
        const tablero = crearTablero(10, 10);
        const glider = [
            [0, 1, 0],
            [0, 0, 1],
            [1, 1, 1]
        ];
        
        colocarPatron(tablero, glider, 1, 1);
        
        console.log("🎮 Juego de la Vida - Generación 0:");
        tablero.forEach(fila => console.log(fila.map(c => c ? '●' : '○').join(' ')));
        
        return { tablero, siguienteGeneracion };
    }
}

// 🚀 Demostraciones
console.log("📊 ARRAYS MULTIDIMENSIONALES");
ArraysMultidimensionales.crearMatrices();
ArraysMultidimensionales.navegarMatrices();
ArraysMultidimensionales.operacionesMatrices();
ArraysMultidimensionales.juegoDelaVida();
```

### 🕳️ **Sparse Arrays y Elementos Vacíos**

```javascript
// 🕳️ Trabajando con arrays que tienen "huecos"
class SparseArrays {
    
    // 🏗️ CREACIÓN Y DETECCIÓN
    static crearSparseArrays() {
        // Diferentes formas de crear sparse arrays
        const sparse1 = [1, , , 4, , 6];           // Literales con comas vacías
        const sparse2 = new Array(5);              // Constructor con un argumento
        const sparse3 = [1, 2, 3];
        delete sparse3[1];                         // Eliminar elemento
        
        console.log("🕳️ Sparse Arrays:");
        console.log("sparse1:", sparse1);           // [1, empty × 2, 4, empty, 6]
        console.log("sparse1.length:", sparse1.length); // 6
        console.log("sparse2:", sparse2);           // [empty × 5]
        console.log("sparse3:", sparse3);           // [1, empty, 3]
        
        // Detectar elementos vacíos
        const tieneHuecos = (arr) => {
            for (let i = 0; i < arr.length; i++) {
                if (!(i in arr)) return true;
            }
            return false;
        };
        
        console.log("sparse1 tiene huecos:", tieneHuecos(sparse1)); // true
        console.log("[1,2,3] tiene huecos:", tieneHuecos([1,2,3])); // false
        
        return { sparse1, sparse2, sparse3 };
    }
    
    // 🔄 COMPORTAMIENTO CON MÉTODOS
    static comportamientoMetodos() {
        const sparse = [1, , 3, , 5];
        
        console.log("🔄 Comportamiento de métodos con sparse arrays:");
        
        // forEach IGNORA elementos vacíos
        console.log("forEach:");
        sparse.forEach((val, i) => console.log(`  [${i}]: ${val}`));
        // Solo imprime índices 0, 2, 4
        
        // map PRESERVA los huecos
        const doubled = sparse.map(x => x * 2);
        console.log("map (×2):", doubled); // [2, empty, 6, empty, 10]
        
        // filter ELIMINA los huecos
        const filtered = sparse.filter(x => true);
        console.log("filter (todos):", filtered); // [1, 3, 5] - ¡sin huecos!
        
        // for...in INCLUYE solo índices con valores
        console.log("for...in:");
        for (const index in sparse) {
            console.log(`  [${index}]: ${sparse[index]}`);
        }
        
        // for...of INCLUYE undefined para huecos
        console.log("for...of:");
        sparse.forEach((val, i) => {
            console.log(`  [${i}]: ${val}`);
        });
        
        return { sparse, doubled, filtered };
    }
    
    // 🔧 UTILIDADES PARA SPARSE ARRAYS
    static utilidadesSparse() {
        // Función para compactar (eliminar huecos)
        const compactar = (arr) => arr.filter(() => true);
        
        // Función para rellenar huecos
        const rellenarHuecos = (arr, valorRelleno = null) => {
            const resultado = [];
            for (let i = 0; i < arr.length; i++) {
                resultado[i] = i in arr ? arr[i] : valorRelleno;
            }
            return resultado;
        };
        
        // Función para obtener solo índices ocupados
        const indicesOcupados = (arr) => {
            const indices = [];
            for (let i = 0; i < arr.length; i++) {
                if (i in arr) indices.push(i);
            }
            return indices;
        };
        
        // Función para obtener densidad (% de elementos no vacíos)
        const calcularDensidad = (arr) => {
            let ocupados = 0;
            for (let i = 0; i < arr.length; i++) {
                if (i in arr) ocupados++;
            }
            return (ocupados / arr.length) * 100;
        };
        
        // Pruebas
        const sparse = [1, , , 4, , 6, , , 9];
        
        console.log("🔧 Utilidades para sparse arrays:");
        console.log("Original:", sparse);
        console.log("Compactado:", compactar(sparse));
        console.log("Relleno con 0:", rellenarHuecos(sparse, 0));
        console.log("Índices ocupados:", indicesOcupados(sparse));
        console.log("Densidad:", calcularDensidad(sparse).toFixed(1) + "%");
        
        return { compactar, rellenarHuecos, indicesOcupados };
    }
    
    // 🎯 CASOS DE USO PRÁCTICOS
    static casosUso() {
        // Caso 1: Matriz dispersa (muchos ceros)
        class MatrizDispersa {
            constructor(filas, columnas) {
                this.filas = filas;
                this.columnas = columnas;
                this.datos = {}; // Solo almacenar valores no-cero
            }
            
            set(fila, col, valor) {
                if (valor !== 0) {
                    this.datos[`${fila},${col}`] = valor;
                } else {
                    delete this.datos[`${fila},${col}`];
                }
            }
            
            get(fila, col) {
                return this.datos[`${fila},${col}`] || 0;
            }
            
            toArray() {
                const resultado = Array(this.filas).fill(null)
                    .map(() => Array(this.columnas).fill(0));
                
                for (const [key, valor] of Object.entries(this.datos)) {
                    const [fila, col] = key.split(',').map(Number);
                    resultado[fila][col] = valor;
                }
                return resultado;
            }
            
            densidad() {
                const totalElementos = this.filas * this.columnas;
                const elementosNoVacios = Object.keys(this.datos).length;
                return (elementosNoVacios / totalElementos) * 100;
            }
        }
        
        // Ejemplo: matriz 1000x1000 con solo 10 valores
        const matrizDispersa = new MatrizDispersa(1000, 1000);
        matrizDispersa.set(0, 0, 5);
        matrizDispersa.set(100, 200, 3);
        matrizDispersa.set(500, 500, 7);
        matrizDispersa.set(999, 999, 2);
        
        console.log("🎯 Matriz dispersa 1000x1000:");
        console.log("Valor en (0,0):", matrizDispersa.get(0, 0));
        console.log("Valor en (1,1):", matrizDispersa.get(1, 1)); // 0
        console.log("Densidad:", matrizDispersa.densidad().toFixed(6) + "%");
        
        // Caso 2: Calendario con eventos
        class CalendarioEventos {
            constructor(año) {
                this.año = año;
                this.eventos = new Array(366); // Máximo días en un año
            }
            
            agregarEvento(mes, dia, evento) {
                const diaDelAño = this.calcularDiaDelAño(mes, dia);
                if (!this.eventos[diaDelAño]) {
                    this.eventos[diaDelAño] = [];
                }
                this.eventos[diaDelAño].push(evento);
            }
            
            obtenerEventos(mes, dia) {
                const diaDelAño = this.calcularDiaDelAño(mes, dia);
                return this.eventos[diaDelAño] || [];
            }
            
            calcularDiaDelAño(mes, dia) {
                const diasPorMes = [31, 28, 31, 30, 31, 30, 31, 31, 30, 31, 30, 31];
                let diaDelAño = dia - 1;
                for (let i = 0; i < mes - 1; i++) {
                    diaDelAño += diasPorMes[i];
                }
                return diaDelAño;
            }
            
            diasConEventos() {
                let count = 0;
                for (let i = 0; i < this.eventos.length; i++) {
                    if (i in this.eventos && this.eventos[i]) count++;
                }
                return count;
            }
        }
        
        const calendario = new CalendarioEventos(2024);
        calendario.agregarEvento(1, 1, "Año Nuevo");
        calendario.agregarEvento(12, 25, "Navidad");
        calendario.agregarEvento(7, 4, "Día de la Independencia");
        
        console.log("📅 Calendario de eventos:");
        console.log("Eventos 1/1:", calendario.obtenerEventos(1, 1));
        console.log("Eventos 2/1:", calendario.obtenerEventos(2, 1));
        console.log("Días con eventos:", calendario.diasConEventos());
        
        return { MatrizDispersa, CalendarioEventos };
    }
}

// 🚀 Demostraciones
console.log("🕳️ SPARSE ARRAYS");
SparseArrays.crearSparseArrays();
SparseArrays.comportamientoMetodos();
SparseArrays.utilidadesSparse();
SparseArrays.casosUso();
```

### 🔢 **Typed Arrays y Rendimiento**

```javascript
// 🔢 Arrays tipados para mejor rendimiento
class TypedArrays {
    
    // 🏗️ TIPOS DISPONIBLES
    static tiposDisponibles() {
        console.log("🔢 Tipos de Typed Arrays disponibles:");
        
        // Enteros con signo
        const int8 = new Int8Array([1, -2, 3]);           // -128 a 127
        const int16 = new Int16Array([1000, -2000]);      // -32,768 a 32,767
        const int32 = new Int32Array([100000, -200000]);  // -2^31 a 2^31-1
        
        // Enteros sin signo
        const uint8 = new Uint8Array([255, 128, 0]);      // 0 a 255
        const uint16 = new Uint16Array([65535, 32768]);   // 0 a 65,535
        const uint32 = new Uint32Array([4294967295]);     // 0 a 2^32-1
        
        // Punto flotante
        const float32 = new Float32Array([3.14, 2.71]);   // 32-bit float
        const float64 = new Float64Array([Math.PI, Math.E]); // 64-bit float
        
        console.log("Int8Array:", int8);
        console.log("Uint8Array:", uint8);
        console.log("Float32Array:", float32);
        console.log("Float64Array:", float64);
        
        // Verificar tamaños
        console.log("\n📏 Tamaños en bytes:");
        console.log("Int8Array.BYTES_PER_ELEMENT:", Int8Array.BYTES_PER_ELEMENT);     // 1
        console.log("Int32Array.BYTES_PER_ELEMENT:", Int32Array.BYTES_PER_ELEMENT);   // 4
        console.log("Float64Array.BYTES_PER_ELEMENT:", Float64Array.BYTES_PER_ELEMENT); // 8
        
        return { int8, uint8, float32, float64 };
    }
    
    // ⚡ COMPARACIÓN DE RENDIMIENTO
    static compararRendimiento() {
        const tamaño = 1000000;
        
        console.log("⚡ Comparación de rendimiento:");
        
        // Crear arrays normales
        console.time("Array normal - creación");
        const arrayNormal = new Array(tamaño);
        for (let i = 0; i < tamaño; i++) {
            arrayNormal[i] = Math.random();
        }
        console.timeEnd("Array normal - creación");
        
        // Crear typed array
        console.time("Float64Array - creación");
        const typedArray = new Float64Array(tamaño);
        for (let i = 0; i < tamaño; i++) {
            typedArray[i] = Math.random();
        }
        console.timeEnd("Float64Array - creación");
        
        // Operaciones matemáticas
        console.time("Array normal - suma");
        let sumaNormal = 0;
        for (let i = 0; i < arrayNormal.length; i++) {
            sumaNormal += arrayNormal[i];
        }
        console.timeEnd("Array normal - suma");
        
        console.time("Float64Array - suma");
        let sumaTyped = 0;
        for (let i = 0; i < typedArray.length; i++) {
            sumaTyped += typedArray[i];
        }
        console.timeEnd("Float64Array - suma");
        
        // Comparar memoria
        const memoriaArray = arrayNormal.length * 8; // aprox 8 bytes por elemento
        const memoriaTyped = typedArray.byteLength;
        
        console.log("💾 Uso de memoria:");
        console.log("Array normal (estimado):", memoriaArray, "bytes");
        console.log("Float64Array (exacto):", memoriaTyped, "bytes");
        
        return { sumaNormal, sumaTyped };
    }
    
    // 🎯 CASOS DE USO PRÁCTICOS
    static casosUsoPracticos() {
        // Caso 1: Procesamiento de imágenes
        class ProcesadorImagen {
            constructor(ancho, alto) {
                this.ancho = ancho;
                this.alto = alto;
                // RGBA: 4 bytes por pixel
                this.datos = new Uint8ClampedArray(ancho * alto * 4);
            }
            
            setPixel(x, y, r, g, b, a = 255) {
                const index = (y * this.ancho + x) * 4;
                this.datos[index] = r;     // Red
                this.datos[index + 1] = g; // Green  
                this.datos[index + 2] = b; // Blue
                this.datos[index + 3] = a; // Alpha
            }
            
            getPixel(x, y) {
                const index = (y * this.ancho + x) * 4;
                return {
                    r: this.datos[index],
                    g: this.datos[index + 1],
                    b: this.datos[index + 2],
                    a: this.datos[index + 3]
                };
            }
            
            aplicarFiltroGris() {
                for (let i = 0; i < this.datos.length; i += 4) {
                    const r = this.datos[i];
                    const g = this.datos[i + 1];
                    const b = this.datos[i + 2];
                    
                    // Conversión a escala de grises
                    const gris = Math.round(0.299 * r + 0.587 * g + 0.114 * b);
                    
                    this.datos[i] = gris;
                    this.datos[i + 1] = gris;
                    this.datos[i + 2] = gris;
                    // Alpha se mantiene igual
                }
            }
        }
        
        // Caso 2: Buffer de audio
        class BufferAudio {
            constructor(sampleRate, duracionSegundos) {
                this.sampleRate = sampleRate;
                this.duracion = duracionSegundos;
                this.samples = new Float32Array(sampleRate * duracionSegundos);
            }
            
            generarSenoidal(frecuencia, amplitud = 1.0) {
                for (let i = 0; i < this.samples.length; i++) {
                    const tiempo = i / this.sampleRate;
                    this.samples[i] = amplitud * Math.sin(2 * Math.PI * frecuencia * tiempo);
                }
            }
            
            aplicarFadeIn(duracionFade) {
                const samplesFade = Math.floor(duracionFade * this.sampleRate);
                for (let i = 0; i < samplesFade && i < this.samples.length; i++) {
                    this.samples[i] *= i / samplesFade;
                }
            }
            
            obtenerPico() {
                let pico = 0;
                for (let i = 0; i < this.samples.length; i++) {
                    pico = Math.max(pico, Math.abs(this.samples[i]));
                }
                return pico;
            }
        }
        
        // Caso 3: Datos científicos
        class DatosCientificos {
            constructor() {
                this.temperaturas = new Float64Array(365); // Año completo
                this.presiones = new Float64Array(365);
                this.humedades = new Uint8Array(365); // 0-100%
            }
            
            registrarDia(dia, temperatura, presion, humedad) {
                this.temperaturas[dia] = temperatura;
                this.presiones[dia] = presion;
                this.humedades[dia] = Math.round(humedad);
            }
            
            calcularPromedios() {
                const sumaTemp = this.temperaturas.reduce((sum, temp) => sum + temp, 0);
                const sumaPresion = this.presiones.reduce((sum, pres) => sum + pres, 0);
                const sumaHumedad = this.humedades.reduce((sum, hum) => sum + hum, 0);
                
                return {
                    temperaturaPromedio: sumaTemp / this.temperaturas.length,
                    presionPromedio: sumaPresion / this.presiones.length,
                    humedadPromedio: sumaHumedad / this.humedades.length
                };
            }
            
            encontrarExtremos() {
                return {
                    tempMin: Math.min(...this.temperaturas),
                    tempMax: Math.max(...this.temperaturas),
                    presionMin: Math.min(...this.presiones),
                    presionMax: Math.max(...this.presiones)
                };
            }
        }
        
        // Demostraciones
        console.log("🎯 Casos de uso prácticos:");
        
        // Imagen pequeña de prueba
        const imagen = new ProcesadorImagen(10, 10);
        imagen.setPixel(5, 5, 255, 0, 0); // Pixel rojo
        console.log("Pixel rojo:", imagen.getPixel(5, 5));
        imagen.aplicarFiltroGris();
        console.log("Después de filtro gris:", imagen.getPixel(5, 5));
        
        // Audio de prueba
        const audio = new BufferAudio(44100, 1); // 1 segundo a 44.1kHz
        audio.generarSenoidal(440); // La4 (440 Hz)
        audio.aplicarFadeIn(0.1); // Fade in de 100ms
        console.log("Pico de audio:", audio.obtenerPico().toFixed(3));
        
        // Datos científicos
        const datos = new DatosCientificos();
        // Simular algunos días
        for (let i = 0; i < 10; i++) {
            datos.registrarDia(i, 20 + Math.random() * 10, 1013 + Math.random() * 20, 50 + Math.random() * 40);
        }
        console.log("Promedios:", datos.calcularPromedios());
        
        return { ProcesadorImagen, BufferAudio, DatosCientificos };
    }
    
    // 🔄 CONVERSIONES Y VISTAS
    static conversionesVistas() {
        console.log("🔄 ArrayBuffer y vistas:");
        
        // Crear un buffer compartido
        const buffer = new ArrayBuffer(16); // 16 bytes
        
        // Diferentes vistas del mismo buffer
        const vista8 = new Uint8Array(buffer);
        const vista16 = new Uint16Array(buffer);
        const vista32 = new Uint32Array(buffer);
        const vistaFloat = new Float32Array(buffer);
        
        // Escribir datos usando vista de 32 bits
        vista32[0] = 0x12345678;
        vista32[1] = 0x9ABCDEF0;
        
        console.log("Buffer como Uint32:", Array.from(vista32));
        console.log("Buffer como Uint16:", Array.from(vista16));
        console.log("Buffer como Uint8:", Array.from(vista8));
        
        // Conversión entre arrays normales y typed arrays
        const arrayNormal = [1, 2, 3, 4, 5];
        const typedDesdeNormal = new Float32Array(arrayNormal);
        const normalDesdeTyped = Array.from(typedDesdeNormal);
        
        console.log("Normal -> Typed:", typedDesdeNormal);
        console.log("Typed -> Normal:", normalDesdeTyped);
        
        return { buffer, vista8, vista32 };
    }
}

// 🚀 Demostraciones
console.log("🔢 TYPED ARRAYS");
TypedArrays.tiposDisponibles();
TypedArrays.compararRendimiento();
TypedArrays.casosUsoPracticos();
TypedArrays.conversionesVistas();
```

### 🎛️ **Array-Like Objects y Conversiones**

```javascript
// 🎛️ Objetos similares a arrays y cómo trabajar con ellos
class ArrayLikeObjects {
    
    // 🔍 IDENTIFICACIÓN Y CREACIÓN
    static identificarArrayLike() {
        // Ejemplos de array-like objects
        const arrayLike1 = {
            0: "primero",
            1: "segundo", 
            2: "tercero",
            length: 3
        };
        
        const arrayLike2 = (function() {
            return arguments; // arguments es array-like
        })(1, 2, 3, 4);
        
        // NodeList (en navegadores)
        // const nodeList = document.querySelectorAll('div'); // array-like
        
        // String es array-like
        const string = "Hola";
        
        console.log("🎛️ Array-like objects:");
        console.log("Objeto personalizado:", arrayLike1);
        console.log("Arguments:", arrayLike2);
        console.log("String:", string);
        
        // Función para detectar si es array-like
        const esArrayLike = (obj) => {
            return obj != null && 
                   typeof obj === 'object' && 
                   typeof obj.length === 'number' && 
                   obj.length >= 0 && 
                   obj.length % 1 === 0;
        };
        
        console.log("✅ Verificaciones:");
        console.log("arrayLike1 es array-like:", esArrayLike(arrayLike1)); // true
        console.log("string es array-like:", esArrayLike(string));         // true
        console.log("[1,2,3] es array-like:", esArrayLike([1,2,3]));       // true
        console.log("{a:1} es array-like:", esArrayLike({a:1}));           // false
        
        return { arrayLike1, arrayLike2, string };
    }
    
    // 🔄 CONVERSIONES A ARRAYS REALES
    static conversionesArrays() {
        const arrayLike = {
            0: "🍎",
            1: "🍌", 
            2: "🍊",
            length: 3
        };
        
        console.log("🔄 Métodos de conversión:");
        
        // Método 1: Array.from()
        const metodo1 = Array.from(arrayLike);
        console.log("Array.from():", metodo1);
        
        // Método 2: Spread operator
        const metodo2 = [...arrayLike]; // ❌ Error: no es iterable
        // console.log("Spread operator:", metodo2); // Comentado para evitar error
        
        // Método 3: Array.prototype.slice.call()
        const metodo3 = Array.prototype.slice.call(arrayLike);
        console.log("slice.call():", metodo3);
        
        // Método 4: for loop manual
        const metodo4 = [];
        for (let i = 0; i < arrayLike.length; i++) {
            metodo4.push(arrayLike[i]);
        }
        console.log("for loop:", metodo4);
        
        // Con argumentos de función
        function ejemploArguments() {
            console.log("Arguments original:", arguments);
            console.log("Arguments es array:", Array.isArray(arguments)); // false
            
            const argsArray = Array.from(arguments);
            console.log("Arguments convertido:", argsArray);
            console.log("Convertido es array:", Array.isArray(argsArray)); // true
            
            // Ahora podemos usar métodos de array
            const doubled = argsArray.map(x => x * 2);
            console.log("Arguments duplicados:", doubled);
        }
        
        ejemploArguments(1, 2, 3, 4, 5);
        
        return { metodo1, metodo3, metodo4 };
    }
    
    // 🛠️ APLICAR MÉTODOS DE ARRAY
    static aplicarMetodosArray() {
        const arrayLike = {
            0: 10,
            1: 20,
            2: 30,
            3: 40,
            length: 4
        };
        
        console.log("🛠️ Aplicando métodos de array a array-like:");
        
        // Usando call/apply para aplicar métodos
        
        // forEach
        console.log("forEach usando call:");
        Array.prototype.forEach.call(arrayLike, (valor, indice) => {
            console.log(`  [${indice}]: ${valor}`);
        });
        
        // map (pero necesitamos convertir el resultado)
        const mapped = Array.prototype.map.call(arrayLike, x => x * 2);
        console.log("map (×2):", mapped);
        
        // filter
        const filtered = Array.prototype.filter.call(arrayLike, x => x > 15);
        console.log("filter (>15):", filtered);
        
        // reduce
        const sum = Array.prototype.reduce.call(arrayLike, (acc, val) => acc + val, 0);
        console.log("reduce (suma):", sum);
        
        // find
        const found = Array.prototype.find.call(arrayLike, x => x > 25);
        console.log("find (>25):", found);
        
        return { mapped, filtered, sum, found };
    }
    
    // 🎯 CASOS PRÁCTICOS
    static casosPracticos() {
        // Caso 1: Trabajar con NodeList (simulado)
        class SimulatedNodeList {
            constructor(elementos) {
                elementos.forEach((elemento, index) => {
                    this[index] = elemento;
                });
                this.length = elementos.length;
            }
            
            // Simular método querySelectorAll
            static querySelectorAll(selector) {
                // Simulamos elementos DOM
                const elementos = [
                    { tagName: 'DIV', textContent: 'Elemento 1', className: 'item' },
                    { tagName: 'DIV', textContent: 'Elemento 2', className: 'item selected' },
                    { tagName: 'DIV', textContent: 'Elemento 3', className: 'item' }
                ];
                return new SimulatedNodeList(elementos);
            }
        }
        
        const nodeList = SimulatedNodeList.querySelectorAll('.item');
        console.log("🎯 Trabajando con NodeList simulado:");
        console.log("NodeList:", nodeList);
        console.log("Es array:", Array.isArray(nodeList)); // false
        
        // Convertir a array para usar métodos
        const elementsArray = Array.from(nodeList);
        const selectedElements = elementsArray.filter(el => 
            el.className.includes('selected')
        );
        console.log("Elementos seleccionados:", selectedElements);
        
        // Caso 2: Función que acepta múltiples argumentos
        function sumarTodos() {
            // arguments es array-like
            console.log("Arguments recibidos:", arguments);
            
            // Convertir a array y usar reduce
            const suma = Array.from(arguments).reduce((acc, val) => acc + val, 0);
            return suma;
        }
        
        const resultado = sumarTodos(1, 2, 3, 4, 5);
        console.log("Suma de argumentos:", resultado);
        
        // Caso 3: Crear array-like personalizado
        class ColeccionPersonalizada {
            constructor() {
                this.length = 0;
            }
            
            add(elemento) {
                this[this.length] = elemento;
                this.length++;
            }
            
            remove(index) {
                if (index >= 0 && index < this.length) {
                    // Desplazar elementos
                    for (let i = index; i < this.length - 1; i++) {
                        this[i] = this[i + 1];
                    }
                    delete this[this.length - 1];
                    this.length--;
                }
            }
            
            toArray() {
                return Array.from(this);
            }
            
            forEach(callback) {
                Array.prototype.forEach.call(this, callback);
            }
            
            map(callback) {
                return Array.prototype.map.call(this, callback);
            }
        }
        
        const coleccion = new ColeccionPersonalizada();
        coleccion.add("Elemento A");
        coleccion.add("Elemento B");
        coleccion.add("Elemento C");
        
        console.log("Colección personalizada:", coleccion);
        console.log("Como array:", coleccion.toArray());
        
        const mayusculas = coleccion.map(item => item.toUpperCase());
        console.log("En mayúsculas:", mayusculas);
        
        return { SimulatedNodeList, ColeccionPersonalizada };
    }
}

// 🚀 Demostraciones
console.log("🎛️ ARRAY-LIKE OBJECTS");
ArrayLikeObjects.identificarArrayLike();
ArrayLikeObjects.conversionesArrays();
ArrayLikeObjects.aplicarMetodosArray();
ArrayLikeObjects.casosPracticos();
```

---

## 7. 🏛️ **Objetos y Propiedades**

### 🌟 **Introducción a Objetos**

Los objetos son la base de JavaScript. Son colecciones de pares clave-valor que pueden contener propiedades y métodos. Todo en JavaScript es un objeto o se comporta como tal.

```javascript
// 🏛️ Los objetos son estructuras fundamentales
const ejemploObjeto = {
    // 🔑 PROPIEDADES (datos)
    nombre: "JavaScript",
    version: "ES2024",
    tipo: "lenguaje",
    
    // 🎯 MÉTODOS (funciones)
    saludar() {
        return `¡Hola desde ${this.nombre}!`;
    },
    
    // 🔢 PROPIEDADES CALCULADAS
    get descripcion() {
        return `${this.nombre} v${this.version}`;
    },
    
    // ⚙️ SETTERS
    set nuevaVersion(v) {
        this.version = v;
        console.log(`Actualizado a versión ${v}`);
    }
};

console.log("🏛️ Objeto completo:", ejemploObjeto);
console.log("Saludo:", ejemploObjeto.saludar());
console.log("Descripción:", ejemploObjeto.descripcion);
```

### 🏗️ **Creación de Objetos**

```javascript
// 🏗️ Diferentes formas de crear objetos
class CreacionObjetos {
    
    // 📝 SINTAXIS LITERAL
    static sintaxisLiteral() {
        // Forma más común y recomendada
        const persona = {
            nombre: "Ana",
            edad: 25,
            profesion: "Desarrolladora",
            saludar() {
                return `Hola, soy ${this.nombre}`;
            }
        };
        
        // Propiedades dinámicas con []
        const propiedad = "habilidades";
        const objeto = {
            [propiedad]: ["JavaScript", "React", "Node.js"],
            [`es_${propiedad.toLowerCase()}`]: true
        };
        
        console.log("🏗️ Objeto literal:", persona);
        console.log("Propiedades dinámicas:", objeto);
        
        return { persona, objeto };
    }
    
    // 🏭 CONSTRUCTOR OBJECT
    static constructorObject() {
        // Usando constructor Object()
        const producto = new Object();
        producto.nombre = "Laptop";
        producto.precio = 999.99;
        producto.categoria = "Electrónicos";
        
        // Equivalente a literal
        const producto2 = {};
        producto2.nombre = "Mouse";
        producto2.precio = 29.99;
        
        console.log("Constructor Object():", producto);
        console.log("Objeto vacío {}:", producto2);
        
        return { producto, producto2 };
    }
    
    // 🏗️ OBJECT.CREATE()
    static objectCreate() {
        // Crear objeto con prototipo específico
        const prototipo = {
            tipo: "Animal",
            dormir() {
                return `${this.nombre} está durmiendo`;
            }
        };
        
        const gato = Object.create(prototipo);
        gato.nombre = "Whiskers";
        gato.especie = "Felino";
        
        // Crear objeto sin prototipo
        const objetoLimpio = Object.create(null);
        objetoLimpio.dato = "Sin herencia";
        
        console.log("Con prototipo:", gato);
        console.log("Gato duerme:", gato.dormir());
        console.log("Sin prototipo:", objetoLimpio);
        console.log("Tiene toString:", "toString" in gato); // true
        console.log("Limpio tiene toString:", "toString" in objetoLimpio); // false
        
        return { gato, objetoLimpio };
    }
    
    // 🏭 CONSTRUCTOR FUNCTIONS
    static constructorFunctions() {
        // Función constructora
        function Vehiculo(marca, modelo, año) {
            this.marca = marca;
            this.modelo = modelo;
            this.año = año;
            this.acelerar = function() {
                return `${this.marca} ${this.modelo} está acelerando`;
            };
        }
        
        // Agregar método al prototipo (más eficiente)
        Vehiculo.prototype.frenar = function() {
            return `${this.marca} ${this.modelo} está frenando`;
        };
        
        const coche = new Vehiculo("Toyota", "Corolla", 2023);
        const moto = new Vehiculo("Honda", "CBR600", 2024);
        
        console.log("🚗 Coche:", coche);
        console.log("Acelerar:", coche.acelerar());
        console.log("Frenar:", coche.frenar());
        
        return { Vehiculo, coche, moto };
    }
    
    // 🎭 CLASES ES6
    static clasesES6() {
        class Estudiante {
            // 🏗️ Constructor
            constructor(nombre, carrera, año) {
                this.nombre = nombre;
                this.carrera = carrera;
                this.año = año;
                this.materias = [];
            }
            
            // 📚 Métodos de instancia
            inscribirMateria(materia) {
                this.materias.push(materia);
                return `${this.nombre} inscrito en ${materia}`;
            }
            
            // 📊 Getter
            get resumen() {
                return `${this.nombre} - ${this.carrera} (${this.año}° año)`;
            }
            
            // ⚙️ Setter
            set nuevoAño(año) {
                if (año > this.año) {
                    this.año = año;
                    console.log(`${this.nombre} promovido a ${año}° año`);
                }
            }
            
            // 🔧 Método estático
            static compararEstudiantes(est1, est2) {
                return est1.año - est2.año;
            }
        }
        
        const estudiante1 = new Estudiante("Carlos", "Ingeniería", 2);
        const estudiante2 = new Estudiante("María", "Medicina", 4);
        
        estudiante1.inscribirMateria("Algoritmos");
        estudiante1.nuevoAño = 3;
        
        console.log("👨‍🎓 Estudiante:", estudiante1);
        console.log("Resumen:", estudiante1.resumen);
        console.log("Comparación:", Estudiante.compararEstudiantes(estudiante1, estudiante2));
        
        return { Estudiante, estudiante1, estudiante2 };
    }
}

// 🚀 Demostraciones
console.log("🏗️ CREACIÓN DE OBJETOS");
CreacionObjetos.sintaxisLiteral();
CreacionObjetos.constructorObject();
CreacionObjetos.objectCreate();
CreacionObjetos.constructorFunctions();
CreacionObjetos.clasesES6();
```

### 🔑 **Acceso a Propiedades**

```javascript
// 🔑 Diferentes formas de acceder a propiedades
class AccesoPropiedades {
    
    // 🎯 DOT NOTATION vs BRACKET NOTATION
    static formasAcceso() {
        const usuario = {
            nombre: "Elena",
            apellido: "García",
            edad: 30,
            "lugar-nacimiento": "Madrid",
            "123numerico": "valor",
            datos: {
                email: "elena@email.com",
                telefono: "123-456-7890"
            }
        };
        
        console.log("🔑 Formas de acceso a propiedades:");
        
        // Dot notation (más legible)
        console.log("Dot notation:");
        console.log("  nombre:", usuario.nombre);
        console.log("  edad:", usuario.edad);
        console.log("  email:", usuario.datos.email);
        
        // Bracket notation (más flexible)
        console.log("Bracket notation:");
        console.log("  nombre:", usuario["nombre"]);
        console.log("  lugar-nacimiento:", usuario["lugar-nacimiento"]); // ❌ usuario.lugar-nacimiento no funciona
        console.log("  123numerico:", usuario["123numerico"]); // ❌ usuario.123numerico no funciona
        
        // Acceso dinámico
        const propiedades = ["nombre", "apellido", "edad"];
        console.log("Acceso dinámico:");
        propiedades.forEach(prop => {
            console.log(`  ${prop}: ${usuario[prop]}`);
        });
        
        return usuario;
    }
    
    // 🔍 VERIFICAR EXISTENCIA DE PROPIEDADES
    static verificarPropiedades() {
        const config = {
            tema: "oscuro",
            idioma: "es",
            notificaciones: true,
            version: undefined
        };
        
        console.log("🔍 Verificar propiedades:");
        
        // Operador 'in'
        console.log("'tema' in config:", "tema" in config); // true
        console.log("'sonido' in config:", "sonido" in config); // false
        console.log("'version' in config:", "version" in config); // true (aunque sea undefined)
        
        // hasOwnProperty (solo propiedades propias)
        console.log("config.hasOwnProperty('tema'):", config.hasOwnProperty('tema')); // true
        console.log("config.hasOwnProperty('toString'):", config.hasOwnProperty('toString')); // false
        
        // Verificar valor definido
        console.log("config.tema !== undefined:", config.tema !== undefined); // true
        console.log("config.version !== undefined:", config.version !== undefined); // false
        
        // Optional chaining (ES2020)
        const usuario = {
            perfil: {
                configuracion: {
                    tema: "claro"
                }
            }
        };
        
        console.log("Optional chaining:");
        console.log("  usuario.perfil?.configuracion?.tema:", usuario.perfil?.configuracion?.tema);
        console.log("  usuario.perfil?.datos?.email:", usuario.perfil?.datos?.email); // undefined
        console.log("  usuario.social?.twitter?.handle:", usuario.social?.twitter?.handle); // undefined
        
        return { config, usuario };
    }
    
    // ⚡ PROPIEDADES DINÁMICAS
    static propiedadesDinamicas() {
        // Crear propiedades basadas en variables
        const prefijo = "user";
        const id = 123;
        const timestamp = Date.now();
        
        const objeto = {
            [`${prefijo}_${id}`]: "Elena García",
            [`created_${timestamp}`]: new Date(),
            [Symbol.toStringTag]: "UsuarioEspecial"
        };
        
        console.log("⚡ Propiedades dinámicas:", objeto);
        
        // Agregar propiedades dinámicamente
        const datos = {};
        const campos = ["nombre", "email", "telefono"];
        const valores = ["Ana", "ana@email.com", "555-0123"];
        
        campos.forEach((campo, index) => {
            datos[campo] = valores[index];
            datos[`${campo}_valido`] = true;
        });
        
        console.log("Datos construidos dinámicamente:", datos);
        
        // Propiedades computadas en clases
        class ProductoComputado {
            constructor(nombre, precio) {
                this.nombre = nombre;
                this.precio = precio;
            }
            
            // Getter computado
            get precioConIva() {
                return this.precio * 1.21;
            }
            
            // Método que usa propiedades dinámicas
            agregarDescuento(porcentaje) {
                const fechaDescuento = new Date().toISOString().split('T')[0];
                this[`descuento_${fechaDescuento}`] = porcentaje;
                this[`precio_con_descuento_${fechaDescuento}`] = this.precio * (1 - porcentaje / 100);
            }
        }
        
        const producto = new ProductoComputado("Laptop", 1000);
        producto.agregarDescuento(15);
        
        console.log("Producto con descuento:", producto);
        console.log("Precio con IVA:", producto.precioConIva);
        
        return { objeto, datos, producto };
    }
    
    // 🎭 DESESTRUCTURACIÓN
    static desestructuracion() {
        const persona = {
            nombre: "David",
            apellido: "López",
            edad: 28,
            trabajo: {
                empresa: "TechCorp",
                puesto: "Developer",
                salario: 50000
            },
            habilidades: ["JavaScript", "Python", "Docker"]
        };
        
        console.log("🎭 Desestructuración de objetos:");
        
        // Desestructuración básica
        const { nombre, edad } = persona;
        console.log("Básica:", { nombre, edad });
        
        // Renombrar variables
        const { nombre: nombreCompleto, apellido: apellidoFamilia } = persona;
        console.log("Renombradas:", { nombreCompleto, apellidoFamilia });
        
        // Valores por defecto
        const { ciudad = "No especificada", pais = "España" } = persona;
        console.log("Con defaults:", { ciudad, pais });
        
        // Desestructuración anidada
        const { trabajo: { empresa, puesto } } = persona;
        console.log("Anidada:", { empresa, puesto });
        
        // Rest operator
        const { nombre: n, ...resto } = persona;
        console.log("Rest:", resto);
        
        // En parámetros de función
        function presentarPersona({ nombre, trabajo: { puesto } }) {
            return `${nombre} trabaja como ${puesto}`;
        }
        
        console.log("En función:", presentarPersona(persona));
        
        // Desestructuración en arrays de objetos
        const empleados = [
            { nombre: "Ana", departamento: "IT" },
            { nombre: "Luis", departamento: "HR" },
            { nombre: "Sara", departamento: "IT" }
        ];
        
        const [{ nombre: primerNombre }, , { departamento: tercerDep }] = empleados;
        console.log("Array de objetos:", { primerNombre, tercerDep });
        
        return { persona, empleados };
    }
}

// 🚀 Demostraciones
console.log("🔑 ACCESO A PROPIEDADES");
AccesoPropiedades.formasAcceso();
AccesoPropiedades.verificarPropiedades();
AccesoPropiedades.propiedadesDinamicas();
AccesoPropiedades.desestructuracion();
```

### 🎯 **Métodos y Contexto (this)**

```javascript
// 🎯 Métodos y el contexto 'this'
class MetodosYContexto {
    
    // 🏹 DEFINICIÓN DE MÉTODOS
    static definicionMetodos() {
        const calculadora = {
            valor: 0,
            
            // Método tradicional
            sumar: function(num) {
                this.valor += num;
                return this;
            },
            
            // Método abreviado (ES6)
            restar(num) {
                this.valor -= num;
                return this;
            },
            
            // Arrow function (NO tiene su propio 'this')
            multiplicarArrow: (num) => {
                // ❌ 'this' se refiere al contexto exterior, no al objeto
                console.log("Arrow function this:", this); // Window o undefined
                // this.valor *= num; // Error
            },
            
            // Getter
            get resultado() {
                return this.valor;
            },
            
            // Setter
            set nuevoValor(val) {
                this.valor = val;
            },
            
            // Método con arrow function correcta
            reset() {
                // Aquí 'this' es correcto
                setTimeout(() => {
                    // Arrow function hereda 'this' del método
                    this.valor = 0;
                    console.log("Reset completado, valor:", this.valor);
                }, 100);
            }
        };
        
        console.log("🎯 Métodos y contexto:");
        
        // Encadenamiento de métodos (method chaining)
        calculadora.sumar(10).restar(3).sumar(5);
        console.log("Resultado después de operaciones:", calculadora.resultado);
        
        // Usar setter
        calculadora.nuevoValor = 100;
        console.log("Después de setter:", calculadora.resultado);
        
        return calculadora;
    }
    
    // 🔄 BINDING Y CONTEXTO
    static bindingContexto() {
        const persona = {
            nombre: "María",
            saludar() {
                return `Hola, soy ${this.nombre}`;
            },
            saludarAsincrono() {
                setTimeout(function() {
                    // ❌ 'this' se pierde en funciones normales
                    console.log("Función normal:", this); // Window o undefined
                }, 100);
                
                setTimeout(() => {
                    // ✅ Arrow function mantiene 'this'
                    console.log("Arrow function:", `Hola desde ${this.nombre}`);
                }, 200);
            }
        };
        
        console.log("🔄 Binding y contexto:");
        
        // Contexto directo
        console.log("Directo:", persona.saludar());
        
        // Contexto perdido
        const metodoSuelto = persona.saludar;
        // console.log("Suelto:", metodoSuelto()); // Error: this es undefined
        
        // Soluciones para mantener contexto
        
        // 1. bind()
        const metodoBind = persona.saludar.bind(persona);
        console.log("Con bind:", metodoBind());
        
        // 2. call()
        console.log("Con call:", persona.saludar.call(persona));
        
        // 3. apply()
        console.log("Con apply:", persona.saludar.apply(persona));
        
        // 4. Arrow function wrapper
        const metodoWrapper = () => persona.saludar();
        console.log("Con wrapper:", metodoWrapper());
        
        persona.saludarAsincrono();
        
        return persona;
    }
    
    // 🎛️ CALL, APPLY Y BIND
    static callApplyBind() {
        const persona1 = { nombre: "Ana", edad: 25 };
        const persona2 = { nombre: "Carlos", edad: 30 };
        
        function presentarse(trabajo, ciudad) {
            return `Soy ${this.nombre}, tengo ${this.edad} años, trabajo como ${trabajo} en ${ciudad}`;
        }
        
        console.log("🎛️ Call, Apply y Bind:");
        
        // call() - argumentos separados
        console.log("Call:", presentarse.call(persona1, "Desarrolladora", "Madrid"));
        console.log("Call:", presentarse.call(persona2, "Diseñador", "Barcelona"));
        
        // apply() - argumentos en array
        const argumentosAna = ["Desarrolladora", "Madrid"];
        const argumentosCarlos = ["Diseñador", "Barcelona"];
        console.log("Apply:", presentarse.apply(persona1, argumentosAna));
        console.log("Apply:", presentarse.apply(persona2, argumentosCarlos));
        
        // bind() - crear nueva función con contexto fijo
        const presentarseAna = presentarse.bind(persona1);
        const presentarseCarlos = presentarse.bind(persona2, "Diseñador"); // Partial application
        
        console.log("Bind Ana:", presentarseAna("Desarrolladora", "Madrid"));
        console.log("Bind Carlos:", presentarseCarlos("Barcelona"));
        
        // Ejemplo práctico: evento con contexto
        class Contador {
            constructor() {
                this.valor = 0;
            }
            
            incrementar() {
                this.valor++;
                console.log(`Contador: ${this.valor}`);
            }
            
            configurarBoton() {
                // Simular addEventListener
                const simularClick = (callback) => {
                    setTimeout(callback, 1000);
                };
                
                // ❌ Perdería el contexto
                // simularClick(this.incrementar);
                
                // ✅ Mantener contexto con bind
                simularClick(this.incrementar.bind(this));
            }
        }
        
        const contador = new Contador();
        contador.configurarBoton();
        
        return { persona1, persona2, contador };
    }
    
    // 🏭 FACTORY FUNCTIONS
    static factoryFunctions() {
        // Factory function para crear objetos similares
        function crearUsuario(nombre, email, rol = "usuario") {
            return {
                nombre,
                email,
                rol,
                activo: true,
                
                // Método privado (closure)
                getId: (() => {
                    const id = Math.random().toString(36).substr(2, 9);
                    return () => id;
                })(),
                
                // Métodos públicos
                activar() {
                    this.activo = true;
                    return `${this.nombre} ha sido activado`;
                },
                
                desactivar() {
                    this.activo = false;
                    return `${this.nombre} ha sido desactivado`;
                },
                
                cambiarRol(nuevoRol) {
                    const rolAnterior = this.rol;
                    this.rol = nuevoRol;
                    return `${this.nombre}: ${rolAnterior} → ${nuevoRol}`;
                },
                
                // Método toString personalizado
                toString() {
                    return `Usuario: ${this.nombre} (${this.rol}) - ${this.activo ? 'Activo' : 'Inactivo'}`;
                }
            };
        }
        
        // Factory con herencia
        function crearAdministrador(nombre, email) {
            const admin = crearUsuario(nombre, email, "administrador");
            
            // Agregar métodos específicos
            admin.gestionarUsuarios = function(accion, usuario) {
                return `${this.nombre} está ${accion} al usuario ${usuario}`;
            };
            
            admin.accederSistema = function() {
                return `${this.nombre} tiene acceso completo al sistema`;
            };
            
            return admin;
        }
        
        console.log("🏭 Factory Functions:");
        
        const usuario1 = crearUsuario("Elena", "elena@email.com");
        const usuario2 = crearUsuario("Pedro", "pedro@email.com", "editor");
        const admin = crearAdministrador("Admin", "admin@email.com");
        
        console.log("Usuario 1:", usuario1.toString());
        console.log("ID usuario 1:", usuario1.getId());
        console.log("Cambio rol:", usuario2.cambiarRol("moderador"));
        console.log("Admin gestiona:", admin.gestionarUsuarios("activando", "Elena"));
        
        return { crearUsuario, crearAdministrador, usuario1, admin };
    }
}

// 🚀 Demostraciones
console.log("🎯 MÉTODOS Y CONTEXTO");
MetodosYContexto.definicionMetodos();
MetodosYContexto.bindingContexto();
MetodosYContexto.callApplyBind();
MetodosYContexto.factoryFunctions();
```

### 🔒 **Descriptores de Propiedades**

```javascript
// 🔒 Control avanzado de propiedades con descriptores
class DescriptoresPropiedades {
    
    // 📋 DESCRIPTORES BÁSICOS
    static descriptoresBasicos() {
        const objeto = {};
        
        // Definir propiedad con descriptor completo
        Object.defineProperty(objeto, 'nombre', {
            value: 'JavaScript',
            writable: true,      // ¿Se puede modificar?
            enumerable: true,    // ¿Aparece en for...in?
            configurable: true   // ¿Se puede reconfigurar/eliminar?
        });
        
        // Propiedad de solo lectura
        Object.defineProperty(objeto, 'version', {
            value: '2024',
            writable: false,     // ❌ No se puede modificar
            enumerable: true,
            configurable: true
        });
        
        // Propiedad no enumerable
        Object.defineProperty(objeto, 'secreto', {
            value: 'valor oculto',
            writable: true,
            enumerable: false,   // ❌ No aparece en iteraciones
            configurable: true
        });
        
        // Propiedad no configurable
        Object.defineProperty(objeto, 'constante', {
            value: 'inmutable',
            writable: false,
            enumerable: true,
            configurable: false  // ❌ No se puede eliminar ni reconfigurar
        });
        
        console.log("🔒 Descriptores básicos:");
        console.log("Objeto:", objeto);
        
        // Intentar modificaciones
        objeto.nombre = "TypeScript"; // ✅ Funciona
        objeto.version = "2025";      // ❌ No funciona (writable: false)
        
        console.log("Después de modificaciones:", objeto);
        console.log("Nombre:", objeto.nombre);
        console.log("Versión:", objeto.version); // Sigue siendo '2024'
        
        // Enumerar propiedades
        console.log("Propiedades enumerables:");
        for (const key in objeto) {
            console.log(`  ${key}: ${objeto[key]}`);
        }
        
        console.log("Todas las propiedades:", Object.getOwnPropertyNames(objeto));
        
        return objeto;
    }
    
    // 🎛️ GETTERS Y SETTERS AVANZADOS
    static gettersSettersAvanzados() {
        const cuenta = {
            _saldo: 1000,  // Propiedad "privada" por convención
            _historial: [],
            
            // Getter para saldo (solo lectura)
            get saldo() {
                return this._saldo;
            },
            
            // Setter con validación
            set deposito(cantidad) {
                if (cantidad <= 0) {
                    throw new Error("El depósito debe ser positivo");
                }
                this._saldo += cantidad;
                this._historial.push({ tipo: 'depósito', cantidad, fecha: new Date() });
            },
            
            // Getter para historial formateado
            get historial() {
                return this._historial.map(transaccion => 
                    `${transaccion.tipo}: $${transaccion.cantidad} (${transaccion.fecha.toLocaleString()})`
                );
            }
        };
        
        // Definir propiedad con getter/setter usando descriptor
        Object.defineProperty(cuenta, 'retiro', {
            set(cantidad) {
                if (cantidad <= 0) {
                    throw new Error("El retiro debe ser positivo");
                }
                if (cantidad > this._saldo) {
                    throw new Error("Saldo insuficiente");
                }
                this._saldo -= cantidad;
                this._historial.push({ tipo: 'retiro', cantidad, fecha: new Date() });
            },
            enumerable: false,
            configurable: true
        });
        
        console.log("🎛️ Getters y Setters avanzados:");
        console.log("Saldo inicial:", cuenta.saldo);
        
        // Usar setters
        cuenta.deposito = 500;
        cuenta.retiro = 200;
        
        console.log("Saldo final:", cuenta.saldo);
        console.log("Historial:", cuenta.historial);
        
        return cuenta;
    }
    
    // 🔐 PROPIEDADES PRIVADAS Y PROTEGIDAS
    static propiedadesPrivadas() {
        // Usando WeakMap para propiedades privadas
        const datosPrivados = new WeakMap();
        
        class UsuarioSeguro {
            constructor(nombre, password) {
                // Datos privados en WeakMap
                datosPrivados.set(this, {
                    password: this.#hashPassword(password),
                    loginAttempts: 0,
                    lastLogin: null
                });
                
                this.nombre = nombre;
                this.createdAt = new Date();
            }
            
            // Método privado (usando # - ES2022)
            #hashPassword(password) {
                // Simulación de hash
                return `hash_${password.split('').reverse().join('')}`;
            }
            
            // Verificar password
            verificarPassword(password) {
                const datos = datosPrivados.get(this);
                const hashedInput = this.#hashPassword(password);
                
                if (hashedInput === datos.password) {
                    datos.lastLogin = new Date();
                    datos.loginAttempts = 0;
                    return true;
                } else {
                    datos.loginAttempts++;
                    return false;
                }
            }
            
            // Getter para datos seguros
            get loginInfo() {
                const datos = datosPrivados.get(this);
                return {
                    lastLogin: datos.lastLogin,
                    failedAttempts: datos.loginAttempts
                };
            }
            
            // Cambiar password
            cambiarPassword(passwordActual, passwordNuevo) {
                if (this.verificarPassword(passwordActual)) {
                    const datos = datosPrivados.get(this);
                    datos.password = this.#hashPassword(passwordNuevo);
                    return "Password actualizado correctamente";
                }
                return "Password actual incorrecto";
            }
        }
        
        console.log("🔐 Propiedades privadas:");
        
        const usuario = new UsuarioSeguro("admin", "secreto123");
        console.log("Usuario creado:", usuario.nombre);
        
        // Intentar acceder a datos privados
        console.log("Datos privados accesibles:", datosPrivados.has(usuario)); // true para el objeto
        // console.log("Password directo:", usuario.password); // undefined
        
        // Usar métodos públicos
        console.log("Login correcto:", usuario.verificarPassword("secreto123"));
        console.log("Login incorrecto:", usuario.verificarPassword("wrong"));
        console.log("Info login:", usuario.loginInfo);
        
        console.log("Cambio password:", usuario.cambiarPassword("secreto123", "nuevoSecreto"));
        console.log("Verificar nuevo:", usuario.verificarPassword("nuevoSecreto"));
        
        return usuario;
    }
    
    // ⚡ PROPIEDADES DINÁMICAS Y PROXY
    static propiedadesDinamicas() {
        // Crear objeto que responde a cualquier propiedad
        const objetoDinamico = new Proxy({}, {
            get(target, prop) {
                if (!(prop in target)) {
                    // Crear propiedad dinámicamente
                    if (prop.startsWith('get')) {
                        const campo = prop.slice(3).toLowerCase();
                        return () => `Obteniendo valor de ${campo}`;
                    }
                    if (prop.startsWith('set')) {
                        const campo = prop.slice(3).toLowerCase();
                        return (valor) => {
                            target[campo] = valor;
                            return `${campo} establecido a: ${valor}`;
                        };
                    }
                    return `Propiedad ${prop} no definida`;
                }
                return target[prop];
            },
            
            set(target, prop, value) {
                // Validar antes de establecer
                if (prop.startsWith('_')) {
                    console.warn(`Advertencia: ${prop} parece ser privada`);
                }
                
                target[prop] = value;
                console.log(`✅ ${prop} = ${value}`);
                return true;
            },
            
            has(target, prop) {
                // Personalizar comportamiento de 'in'
                return true; // Cualquier propiedad "existe"
            },
            
            ownKeys(target) {
                // Personalizar Object.keys()
                return [...Object.keys(target), 'propiedadFantasma'];
            }
        });
        
        console.log("⚡ Propiedades dinámicas con Proxy:");
        
        // Usar propiedades dinámicas
        console.log("getNombre():", objetoDinamico.getNombre());
        console.log("setEdad():", objetoDinamico.setEdad(25));
        console.log("Edad establecida:", objetoDinamico.edad);
        
        // Propiedad no definida
        console.log("Propiedad inexistente:", objetoDinamico.cualquierCosa);
        
        // Verificar existencia
        console.log("'inexistente' in objeto:", 'inexistente' in objetoDinamico);
        
        // Establecer propiedad privada
        objetoDinamico._privada = "valor secreto";
        
        return objetoDinamico;
    }
}

// 🚀 Demostraciones
console.log("🔒 DESCRIPTORES DE PROPIEDADES");
DescriptoresPropiedades.descriptoresBasicos();
DescriptoresPropiedades.gettersSettersAvanzados();
DescriptoresPropiedades.propiedadesPrivadas();
DescriptoresPropiedades.propiedadesDinamicas();
```

---

## 8. 🔗 **Objetos Anidados y Estructuras Complejas**

### 🌟 **Introducción a Estructuras Complejas**

Los objetos anidados son la realidad del desarrollo moderno. Desde APIs REST hasta configuraciones complejas, necesitas dominar la navegación y manipulación de estructuras profundas.

```javascript
// 🔗 Ejemplo de estructura compleja real
const aplicacionCompleja = {
    // 👤 INFORMACIÓN DEL USUARIO
    usuario: {
        id: 12345,
        perfil: {
            nombre: "Ana García",
            email: "ana@empresa.com",
            configuracion: {
                tema: "oscuro",
                idioma: "es",
                notificaciones: {
                    email: true,
                    push: false,
                    sms: {
                        habilitado: true,
                        numero: "+34-123-456-789"
                    }
                }
            },
            direcciones: [
                {
                    tipo: "principal",
                    calle: "Calle Mayor 123",
                    ciudad: "Madrid",
                    pais: "España",
                    coordenadas: { lat: 40.416775, lng: -3.703790 }
                },
                {
                    tipo: "trabajo",
                    calle: "Av. Castellana 200",
                    ciudad: "Madrid",
                    pais: "España",
                    coordenadas: { lat: 40.450772, lng: -3.692487 }
                }
            ]
        },
        permisos: ["leer", "escribir", "admin"],
        sesiones: {
            actual: { inicio: "2024-01-15T09:00:00Z", ip: "192.168.1.100" },
            historial: [
                { inicio: "2024-01-14T08:30:00Z", fin: "2024-01-14T17:45:00Z" },
                { inicio: "2024-01-13T09:15:00Z", fin: "2024-01-13T16:30:00Z" }
            ]
        }
    },
    
    // 📊 DATOS DE LA APLICACIÓN
    aplicacion: {
        metadata: {
            version: "2.1.0",
            build: "20240115.1",
            entorno: "produccion"
        },
        configuracion: {
            api: {
                baseUrl: "https://api.empresa.com",
                endpoints: {
                    usuarios: "/users",
                    pedidos: "/orders",
                    productos: "/products"
                },
                timeouts: { conexion: 5000, respuesta: 30000 }
            },
            cache: {
                habilitado: true,
                ttl: 300000,
                estrategia: "LRU"
            }
        }
    }
};

console.log("🔗 Estructura compleja lista para explorar");
```

### 🌳 **Navegación en Estructuras Profundas**

```javascript
// 🌳 Técnicas para navegar estructuras anidadas
class NavegacionProfunda {
    
    // 🗺️ NAVEGACIÓN BÁSICA
    static navegacionBasica() {
        const empresa = {
            nombre: "TechCorp",
            departamentos: {
                desarrollo: {
                    jefe: "Carlos Ruiz",
                    empleados: [
                        {
                            id: 1,
                            nombre: "Ana López",
                            proyectos: [
                                { nombre: "Web App", estado: "activo", tecnologias: ["React", "Node.js"] },
                                { nombre: "Mobile App", estado: "completado", tecnologias: ["React Native"] }
                            ]
                        },
                        {
                            id: 2,
                            nombre: "Luis García",
                            proyectos: [
                                { nombre: "API REST", estado: "activo", tecnologias: ["Express", "MongoDB"] }
                            ]
                        }
                    ]
                },
                marketing: {
                    jefe: "María Sánchez",
                    empleados: [
                        {
                            id: 3,
                            nombre: "Pedro Martín",
                            campanas: [
                                { nombre: "Campaña Q1", presupuesto: 50000, estado: "activa" }
                            ]
                        }
                    ]
                }
            }
        };
        
        console.log("🗺️ Navegación básica:");
        
        // Acceso directo
        console.log("Jefe desarrollo:", empresa.departamentos.desarrollo.jefe);
        
        // Navegar arrays anidados
        const primerEmpleadoDev = empresa.departamentos.desarrollo.empleados[0];
        console.log("Primer empleado:", primerEmpleadoDev.nombre);
        console.log("Su primer proyecto:", primerEmpleadoDev.proyectos[0].nombre);
        
        // Navegación con variables
        const departamento = "desarrollo";
        const jefe = empresa.departamentos[departamento].jefe;
        console.log(`Jefe de ${departamento}:`, jefe);
        
        return empresa;
    }
    
    // 🛡️ NAVEGACIÓN SEGURA
    static navegacionSegura() {
        const datos = {
            usuario: {
                perfil: {
                    nombre: "Elena"
                    // configuracion: undefined - propiedad faltante
                }
                // social: undefined - objeto faltante
            }
        };
        
        console.log("🛡️ Navegación segura:");
        
        // ❌ Navegación peligrosa (puede fallar)
        try {
            // const tema = datos.usuario.perfil.configuracion.tema; // Error!
            console.log("❌ Esto causaría error");
        } catch (error) {
            console.log("Error capturado:", error.message);
        }
        
        // ✅ Verificación manual
        const temaSeguro = datos.usuario && 
                          datos.usuario.perfil && 
                          datos.usuario.perfil.configuracion && 
                          datos.usuario.perfil.configuracion.tema;
        console.log("Tema (verificación manual):", temaSeguro);
        
        // ✅ Optional chaining (ES2020)
        const temaModerno = datos.usuario?.perfil?.configuracion?.tema;
        console.log("Tema (optional chaining):", temaModerno);
        
        // ✅ Con valores por defecto
        const temaConDefault = datos.usuario?.perfil?.configuracion?.tema ?? "claro";
        console.log("Tema con default:", temaConDefault);
        
        // ✅ Para arrays anidados
        const primerPost = datos.usuario?.social?.posts?.[0]?.titulo;
        console.log("Primer post:", primerPost);
        
        // ✅ Para métodos
        const saludo = datos.usuario?.perfil?.saludar?.();
        console.log("Saludo:", saludo);
        
        return datos;
    }
    
    // 🔍 BÚSQUEDA EN ESTRUCTURAS COMPLEJAS
    static busquedaCompleja() {
        const sistemaArchivos = {
            nombre: "root",
            tipo: "carpeta",
            contenido: [
                {
                    nombre: "documentos",
                    tipo: "carpeta",
                    contenido: [
                        { nombre: "informe.pdf", tipo: "archivo", tamaño: 1024 },
                        { nombre: "presentacion.pptx", tipo: "archivo", tamaño: 2048 },
                        {
                            nombre: "proyectos",
                            tipo: "carpeta",
                            contenido: [
                                { nombre: "web-app", tipo: "carpeta", contenido: [
                                    { nombre: "index.html", tipo: "archivo", tamaño: 512 },
                                    { nombre: "styles.css", tipo: "archivo", tamaño: 256 },
                                    { nombre: "script.js", tipo: "archivo", tamaño: 1536 }
                                ]},
                                { nombre: "mobile-app", tipo: "carpeta", contenido: [
                                    { nombre: "App.js", tipo: "archivo", tamaño: 2048 }
                                ]}
                            ]
                        }
                    ]
                },
                {
                    nombre: "imagenes",
                    tipo: "carpeta",
                    contenido: [
                        { nombre: "logo.png", tipo: "archivo", tamaño: 4096 },
                        { nombre: "banner.jpg", tipo: "archivo", tamaño: 8192 }
                    ]
                }
            ]
        };
        
        // Función recursiva para buscar archivos
        function buscarArchivos(nodo, criterio) {
            let resultados = [];
            
            if (nodo.tipo === "archivo" && criterio(nodo)) {
                resultados.push(nodo);
            } else if (nodo.tipo === "carpeta" && nodo.contenido) {
                for (const hijo of nodo.contenido) {
                    resultados = resultados.concat(buscarArchivos(hijo, criterio));
                }
            }
            
            return resultados;
        }
        
        // Función para obtener ruta completa
        function obtenerRuta(nodo, nombreBuscado, rutaActual = "") {
            const rutaCompleta = rutaActual + "/" + nodo.nombre;
            
            if (nodo.nombre === nombreBuscado) {
                return rutaCompleta;
            }
            
            if (nodo.tipo === "carpeta" && nodo.contenido) {
                for (const hijo of nodo.contenido) {
                    const resultado = obtenerRuta(hijo, nombreBuscado, rutaCompleta);
                    if (resultado) return resultado;
                }
            }
            
            return null;
        }
        
        console.log("🔍 Búsqueda en estructuras complejas:");
        
        // Buscar archivos JavaScript
        const archivosJS = buscarArchivos(sistemaArchivos, 
            archivo => archivo.nombre.endsWith('.js'));
        console.log("Archivos JavaScript:", archivosJS.map(a => a.nombre));
        
        // Buscar archivos grandes (> 2KB)
        const archivosGrandes = buscarArchivos(sistemaArchivos, 
            archivo => archivo.tamaño > 2048);
        console.log("Archivos grandes:", archivosGrandes.map(a => 
            `${a.nombre} (${a.tamaño} bytes)`));
        
        // Encontrar ruta de archivo específico
        const rutaCSS = obtenerRuta(sistemaArchivos, "styles.css");
        console.log("Ruta del CSS:", rutaCSS);
        
        // Estadísticas del sistema
        function obtenerEstadisticas(nodo) {
            const stats = { carpetas: 0, archivos: 0, tamañoTotal: 0 };
            
            if (nodo.tipo === "archivo") {
                stats.archivos = 1;
                stats.tamañoTotal = nodo.tamaño;
            } else if (nodo.tipo === "carpeta") {
                stats.carpetas = 1;
                if (nodo.contenido) {
                    for (const hijo of nodo.contenido) {
                        const subStats = obtenerEstadisticas(hijo);
                        stats.carpetas += subStats.carpetas;
                        stats.archivos += subStats.archivos;
                        stats.tamañoTotal += subStats.tamañoTotal;
                    }
                }
            }
            
            return stats;
        }
        
        const estadisticas = obtenerEstadisticas(sistemaArchivos);
        console.log("📊 Estadísticas:", estadisticas);
        
        return { sistemaArchivos, buscarArchivos, obtenerRuta };
    }
    
    // 🎯 EXTRACCIÓN DE DATOS ESPECÍFICOS
    static extraccionDatos() {
        const respuestaAPI = {
            meta: {
                total: 150,
                pagina: 1,
                porPagina: 10,
                totalPaginas: 15
            },
            datos: [
                {
                    id: 1,
                    usuario: {
                        nombre: "Ana García",
                        email: "ana@empresa.com",
                        perfil: {
                            avatar: "https://api.com/avatars/1.jpg",
                            ubicacion: { ciudad: "Madrid", pais: "España" },
                            estadisticas: { posts: 45, seguidores: 120, siguiendo: 80 }
                        }
                    },
                    posts: [
                        {
                            id: 101,
                            titulo: "Introducción a JavaScript",
                            contenido: "JavaScript es un lenguaje...",
                            fecha: "2024-01-15",
                            etiquetas: ["javascript", "programacion", "web"],
                            interacciones: { likes: 25, comentarios: 8, compartidos: 3 }
                        },
                        {
                            id: 102,
                            titulo: "React vs Vue",
                            contenido: "Comparativa entre frameworks...",
                            fecha: "2024-01-10",
                            etiquetas: ["react", "vue", "frameworks"],
                            interacciones: { likes: 42, comentarios: 15, compartidos: 7 }
                        }
                    ]
                },
                {
                    id: 2,
                    usuario: {
                        nombre: "Carlos López",
                        email: "carlos@empresa.com",
                        perfil: {
                            avatar: "https://api.com/avatars/2.jpg",
                            ubicacion: { ciudad: "Barcelona", pais: "España" },
                            estadisticas: { posts: 32, seguidores: 95, siguiendo: 110 }
                        }
                    },
                    posts: [
                        {
                            id: 201,
                            titulo: "CSS Grid vs Flexbox",
                            contenido: "Guía completa sobre layouts...",
                            fecha: "2024-01-12",
                            etiquetas: ["css", "layout", "design"],
                            interacciones: { likes: 38, comentarios: 12, compartidos: 5 }
                        }
                    ]
                }
            ]
        };
        
        console.log("🎯 Extracción de datos específicos:");
        
        // Extraer todos los nombres de usuarios
        const nombresUsuarios = respuestaAPI.datos.map(item => item.usuario.nombre);
        console.log("Nombres usuarios:", nombresUsuarios);
        
        // Extraer todos los títulos de posts
        const titulosPosts = respuestaAPI.datos
            .flatMap(item => item.posts)
            .map(post => post.titulo);
        console.log("Títulos posts:", titulosPosts);
        
        // Extraer estadísticas combinadas
        const estadisticasUsuarios = respuestaAPI.datos.map(item => ({
            nombre: item.usuario.nombre,
            ciudad: item.usuario.perfil.ubicacion.ciudad,
            posts: item.usuario.perfil.estadisticas.posts,
            seguidores: item.usuario.perfil.estadisticas.seguidores,
            totalLikes: item.posts.reduce((sum, post) => sum + post.interacciones.likes, 0)
        }));
        console.log("Estadísticas usuarios:", estadisticasUsuarios);
        
        // Extraer todas las etiquetas únicas
        const todasEtiquetas = respuestaAPI.datos
            .flatMap(item => item.posts)
            .flatMap(post => post.etiquetas);
        const etiquetasUnicas = [...new Set(todasEtiquetas)];
        console.log("Etiquetas únicas:", etiquetasUnicas);
        
        // Posts más populares (por likes)
        const postsPopulares = respuestaAPI.datos
            .flatMap(item => item.posts.map(post => ({
                ...post,
                autor: item.usuario.nombre
            })))
            .sort((a, b) => b.interacciones.likes - a.interacciones.likes)
            .slice(0, 3);
        console.log("Posts más populares:", postsPopulares.map(p => 
            `"${p.titulo}" por ${p.autor} (${p.interacciones.likes} likes)`));
        
        return { respuestaAPI, estadisticasUsuarios, etiquetasUnicas };
    }
}

// 🚀 Demostraciones
console.log("🌳 NAVEGACIÓN EN ESTRUCTURAS PROFUNDAS");
NavegacionProfunda.navegacionBasica();
NavegacionProfunda.navegacionSegura();
NavegacionProfunda.busquedaCompleja();
NavegacionProfunda.extraccionDatos();
```

### 🔄 **Clonado de Objetos (Shallow vs Deep)**

```javascript
// 🔄 Clonado superficial vs profundo
class ClonadoObjetos {
    
    // 📋 CLONADO SUPERFICIAL (SHALLOW COPY)
    static clonadoSuperficial() {
        const original = {
            nombre: "Ana",
            edad: 30,
            hobbies: ["leer", "nadar", "programar"],
            trabajo: {
                empresa: "TechCorp",
                puesto: "Developer",
                salario: 50000
            }
        };
        
        console.log("📋 Clonado superficial:");
        
        // Método 1: Object.assign()
        const clon1 = Object.assign({}, original);
        
        // Método 2: Spread operator
        const clon2 = { ...original };
        
        // Método 3: Object.create() + propiedades
        const clon3 = Object.create(Object.getPrototypeOf(original));
        Object.assign(clon3, original);
        
        console.log("Original:", original);
        console.log("Clon 1 (Object.assign):", clon1);
        console.log("Clon 2 (spread):", clon2);
        
        // Verificar que son objetos diferentes
        console.log("¿Son el mismo objeto?", original === clon1); // false
        console.log("¿Tienen el mismo contenido?", 
            JSON.stringify(original) === JSON.stringify(clon1)); // true
        
        // ⚠️ PROBLEMA: Referencias compartidas en objetos anidados
        console.log("\n⚠️ Problema con objetos anidados:");
        
        // Modificar objeto anidado en el clon
        clon1.trabajo.salario = 60000;
        clon1.hobbies.push("viajar");
        
        console.log("Después de modificar clon1:");
        console.log("Original salario:", original.trabajo.salario); // ❌ 60000 (¡cambió!)
        console.log("Original hobbies:", original.hobbies); // ❌ incluye "viajar"
        console.log("Clon1 salario:", clon1.trabajo.salario); // 60000
        
        // Las referencias de objetos anidados se comparten
        console.log("¿Mismo objeto trabajo?", original.trabajo === clon1.trabajo); // true
        console.log("¿Mismo array hobbies?", original.hobbies === clon1.hobbies); // true
        
        return { original, clon1, clon2 };
    }
    
    // 🏔️ CLONADO PROFUNDO (DEEP COPY)
    static clonadoProfundo() {
        const original = {
            nombre: "Carlos",
            edad: 35,
            direccion: {
                calle: "Calle Mayor 123",
                ciudad: "Madrid",
                coordenadas: {
                    lat: 40.416775,
                    lng: -3.703790
                }
            },
            proyectos: [
                {
                    nombre: "Web App",
                    tecnologias: ["React", "Node.js"],
                    equipo: {
                        lider: "Ana",
                        miembros: ["Luis", "María", "Pedro"]
                    }
                },
                {
                    nombre: "Mobile App",
                    tecnologias: ["React Native"],
                    equipo: {
                        lider: "Elena",
                        miembros: ["Javi", "Carmen"]
                    }
                }
            ],
            fecha: new Date("2024-01-15"),
            activo: true
        };
        
        console.log("🏔️ Clonado profundo:");
        
        // Método 1: JSON.parse(JSON.stringify()) - Limitado pero rápido
        const clonJSON = JSON.parse(JSON.stringify(original));
        
        // Método 2: Función recursiva personalizada
        function clonarProfundo(obj) {
            // Casos base
            if (obj === null || typeof obj !== "object") return obj;
            if (obj instanceof Date) return new Date(obj.getTime());
            if (obj instanceof Array) return obj.map(item => clonarProfundo(item));
            if (obj instanceof RegExp) return new RegExp(obj);
            
            // Objeto regular
            const clonado = {};
            for (const key in obj) {
                if (obj.hasOwnProperty(key)) {
                    clonado[key] = clonarProfundo(obj[key]);
                }
            }
            return clonado;
        }
        
        const clonRecursivo = clonarProfundo(original);
        
        // Método 3: structuredClone (ES2022 - moderno)
        // const clonModerno = structuredClone(original); // No disponible en todos los entornos
        
        console.log("Original:", original);
        console.log("Clon JSON:", clonJSON);
        console.log("Clon recursivo:", clonRecursivo);
        
        // Verificar independencia
        console.log("\n✅ Verificar independencia:");
        
        // Modificar clon sin afectar original
        clonRecursivo.direccion.calle = "Nueva Calle 456";
        clonRecursivo.proyectos[0].equipo.miembros.push("Roberto");
        clonRecursivo.nombre = "Carlos Modificado";
        
        console.log("Después de modificar clon recursivo:");
        console.log("Original calle:", original.direccion.calle); // "Calle Mayor 123"
        console.log("Clon calle:", clonRecursivo.direccion.calle); // "Nueva Calle 456"
        console.log("Original equipo:", original.proyectos[0].equipo.miembros.length); // 3
        console.log("Clon equipo:", clonRecursivo.proyectos[0].equipo.miembros.length); // 4
        
        // ⚠️ Limitaciones del método JSON
        console.log("\n⚠️ Limitaciones JSON.parse/stringify:");
        console.log("Original fecha tipo:", typeof original.fecha); // object (Date)
        console.log("Clon JSON fecha tipo:", typeof clonJSON.fecha); // string
        console.log("Clon recursivo fecha tipo:", typeof clonRecursivo.fecha); // object (Date)
        
        return { original, clonJSON, clonRecursivo, clonarProfundo };
    }
    
    // 🔧 CLONADO SELECTIVO Y OPTIMIZADO
    static clonadoSelectivo() {
        const configuracion = {
            usuario: {
                id: 12345,
                nombre: "Elena",
                preferencias: {
                    tema: "oscuro",
                    idioma: "es",
                    notificaciones: {
                        email: true,
                        push: false,
                        frecuencia: "diaria"
                    }
                }
            },
            aplicacion: {
                version: "2.1.0",
                cache: {
                    habilitado: true,
                    tamaño: 100,
                    datos: new Map([["key1", "value1"], ["key2", "value2"]]) // Estructura compleja
                },
                logs: [], // Array que puede ser muy grande
                temporal: {
                    sessionId: "abc123",
                    timestamp: Date.now()
                }
            }
        };
        
        // Función para clonar solo ciertas propiedades
        function clonarSelectivo(obj, incluir = [], excluir = []) {
            function debeIncluir(ruta) {
                if (incluir.length > 0) {
                    return incluir.some(patron => ruta.startsWith(patron));
                }
                if (excluir.length > 0) {
                    return !excluir.some(patron => ruta.startsWith(patron));
                }
                return true;
            }
            
            function clonar(objeto, rutaActual = "") {
                if (objeto === null || typeof objeto !== "object") return objeto;
                if (objeto instanceof Date) return new Date(objeto.getTime());
                if (objeto instanceof Map) return new Map(objeto);
                if (objeto instanceof Set) return new Set(objeto);
                
                if (Array.isArray(objeto)) {
                    return objeto.map((item, index) => 
                        clonar(item, `${rutaActual}[${index}]`)
                    );
                }
                
                const resultado = {};
                for (const [key, value] of Object.entries(objeto)) {
                    const nuevaRuta = rutaActual ? `${rutaActual}.${key}` : key;
                    if (debeIncluir(nuevaRuta)) {
                        resultado[key] = clonar(value, nuevaRuta);
                    }
                }
                return resultado;
            }
            
            return clonar(obj);
        }
        
        console.log("🔧 Clonado selectivo:");
        
        // Clonar solo configuración de usuario
        const soloUsuario = clonarSelectivo(configuracion, ["usuario"]);
        console.log("Solo usuario:", soloUsuario);
        
        // Clonar excluyendo datos temporales y logs
        const sinTemporales = clonarSelectivo(configuracion, [], ["aplicacion.logs", "aplicacion.temporal"]);
        console.log("Sin temporales:", sinTemporales);
        
        // Clonar solo preferencias específicas
        const soloPreferencias = clonarSelectivo(configuracion, ["usuario.preferencias"]);
        console.log("Solo preferencias:", soloPreferencias);
        
        // Función para clonar con transformación
        function clonarConTransformacion(obj, transformadores = {}) {
            function clonar(objeto, rutaActual = "") {
                // Aplicar transformador específico si existe
                if (transformadores[rutaActual]) {
                    return transformadores[rutaActual](objeto);
                }
                
                if (objeto === null || typeof objeto !== "object") return objeto;
                if (objeto instanceof Date) return new Date(objeto.getTime());
                
                if (Array.isArray(objeto)) {
                    return objeto.map((item, index) => 
                        clonar(item, `${rutaActual}[${index}]`)
                    );
                }
                
                const resultado = {};
                for (const [key, value] of Object.entries(objeto)) {
                    const nuevaRuta = rutaActual ? `${rutaActual}.${key}` : key;
                    resultado[key] = clonar(value, nuevaRuta);
                }
                return resultado;
            }
            
            return clonar(obj);
        }
        
        // Ejemplo con transformaciones
        const configTransformada = clonarConTransformacion(configuracion, {
            "usuario.id": (id) => `USER_${id}`, // Prefijo al ID
            "aplicacion.version": (version) => version.toUpperCase(), // Versión en mayúsculas
            "aplicacion.cache": () => ({ limpio: true }) // Resetear cache
        });
        
        console.log("Con transformaciones:", configTransformada);
        
        return { configuracion, clonarSelectivo, clonarConTransformacion };
    }
    
    // ⚡ RENDIMIENTO EN CLONADO
    static rendimientoClonado() {
        // Crear objeto de prueba grande
        const crearObjetoGrande = (profundidad, anchura) => {
            if (profundidad === 0) {
                return Math.random();
            }
            
            const obj = {};
            for (let i = 0; i < anchura; i++) {
                obj[`prop${i}`] = crearObjetoGrande(profundidad - 1, anchura);
            }
            return obj;
        };
        
        const objetoGrande = crearObjetoGrande(4, 5); // Profundidad 4, anchura 5
        
        console.log("⚡ Comparación de rendimiento:");
        
        // Spread operator (shallow)
        console.time("Spread operator");
        const spreadClon = { ...objetoGrande };
        console.timeEnd("Spread operator");
        
        // JSON.parse/stringify
        console.time("JSON parse/stringify");
        const jsonClon = JSON.parse(JSON.stringify(objetoGrande));
        console.timeEnd("JSON parse/stringify");
        
        // Función recursiva
        function clonRecursivo(obj) {
            if (obj === null || typeof obj !== "object") return obj;
            if (Array.isArray(obj)) return obj.map(clonRecursivo);
            
            const clonado = {};
            for (const key in obj) {
                if (obj.hasOwnProperty(key)) {
                    clonado[key] = clonRecursivo(obj[key]);
                }
            }
            return clonado;
        }
        
        console.time("Recursivo personalizado");
        const recursivoClón = clonRecursivo(objetoGrande);
        console.timeEnd("Recursivo personalizado");
        
        // Verificar tamaños
        const calcularTamaño = (obj) => JSON.stringify(obj).length;
        console.log("Tamaño objeto original:", calcularTamaño(objetoGrande), "caracteres");
        
        return { objetoGrande, jsonClon, recursivoClón };
    }
}

// 🚀 Demostraciones
console.log("🔄 CLONADO DE OBJETOS");
ClonadoObjetos.clonadoSuperficial();
ClonadoObjetos.clonadoProfundo();
ClonadoObjetos.clonadoSelectivo();
ClonadoObjetos.rendimientoClonado();
```

### 🎯 **Manipulación de Datos JSON**

```javascript
// 🎯 Manipulación avanzada de datos JSON
class ManipulacionJSON {
    
    // 📥 PARSING Y SERIALIZACIÓN SEGURA
    static parsingSeguro() {
        console.log("📥 Parsing y serialización segura:");
        
        // JSON válido
        const jsonValido = '{"nombre": "Ana", "edad": 30, "activo": true}';
        
        // JSON inválido
        const jsonInvalido = '{"nombre": "Ana", "edad": 30, "activo":}';
        
        // JSON con valores especiales
        const jsonEspecial = '{"fecha": "2024-01-15T10:30:00Z", "numero": null, "indefinido": undefined}';
        
        // Función de parsing seguro
        function parsearSeguro(jsonString, valorDefault = null) {
            try {
                return JSON.parse(jsonString);
            } catch (error) {
                console.warn("Error al parsear JSON:", error.message);
                return valorDefault;
            }
        }
        
        console.log("JSON válido parseado:", parsearSeguro(jsonValido));
        console.log("JSON inválido parseado:", parsearSeguro(jsonInvalido, {}));
        
        // Parsing con validación
        function parsearConValidacion(jsonString, esquema) {
            const objeto = parsearSeguro(jsonString);
            if (!objeto) return null;
            
            // Validación simple de esquema
            for (const [campo, tipo] of Object.entries(esquema)) {
                if (!(campo in objeto)) {
                    console.warn(`Campo requerido '${campo}' no encontrado`);
                    return null;
                }
                if (typeof objeto[campo] !== tipo) {
                    console.warn(`Campo '${campo}' debe ser de tipo '${tipo}'`);
                    return null;
                }
            }
            
            return objeto;
        }
        
        const esquemaUsuario = { nombre: "string", edad: "number", activo: "boolean" };
        const usuarioValido = parsearConValidacion(jsonValido, esquemaUsuario);
        console.log("Usuario validado:", usuarioValido);
        
        // Serialización con replacer
        const objeto = {
            nombre: "Carlos",
            password: "secreto123",
            edad: 35,
            fecha: new Date(),
            configuracion: {
                tema: "oscuro",
                token: "abc123xyz"
            }
        };
        
        // Excluir campos sensibles
        const jsonSinSecretos = JSON.stringify(objeto, (key, value) => {
            if (key === "password" || key === "token") {
                return "[OCULTO]";
            }
            return value;
        }, 2);
        
        console.log("JSON sin secretos:", jsonSinSecretos);
        
        return { parsearSeguro, parsearConValidacion };
    }
    
    // 🔄 TRANSFORMACIÓN DE DATOS
    static transformacionDatos() {
        const datosAPI = {
            status: "success",
            data: {
                users: [
                    {
                        id: 1,
                        full_name: "Ana García López",
                        email_address: "ana@empresa.com",
                        birth_date: "1990-05-15",
                        is_active: true,
                        profile_settings: {
                            display_name: "Ana G.",
                            theme_preference: "dark",
                            notification_settings: {
                                email_notifications: true,
                                push_notifications: false
                            }
                        },
                        account_balance: "1250.50",
                        last_login: "2024-01-15T14:30:00Z"
                    },
                    {
                        id: 2,
                        full_name: "Carlos Ruiz Martín",
                        email_address: "carlos@empresa.com",
                        birth_date: "1985-09-22",
                        is_active: false,
                        profile_settings: {
                            display_name: "Carlos R.",
                            theme_preference: "light",
                            notification_settings: {
                                email_notifications: false,
                                push_notifications: true
                            }
                        },
                        account_balance: "750.25",
                        last_login: "2024-01-10T09:15:00Z"
                    }
                ]
            }
        };
        
        console.log("🔄 Transformación de datos:");
        
        // Transformar snake_case a camelCase
        function toCamelCase(str) {
            return str.replace(/_([a-z])/g, (match, letter) => letter.toUpperCase());
        }
        
        function transformarObjeto(obj) {
            if (Array.isArray(obj)) {
                return obj.map(transformarObjeto);
            }
            
            if (obj !== null && typeof obj === "object") {
                const transformado = {};
                for (const [key, value] of Object.entries(obj)) {
                    const nuevaKey = toCamelCase(key);
                    transformado[nuevaKey] = transformarObjeto(value);
                }
                return transformado;
            }
            
            return obj;
        }
        
        const datosCamelCase = transformarObjeto(datosAPI);
        console.log("Datos en camelCase:", JSON.stringify(datosCamelCase, null, 2));
        
        // Transformar y normalizar datos
        function normalizarUsuarios(datosAPI) {
            return datosAPI.data.users.map(user => ({
                id: user.id,
                nombre: user.full_name,
                email: user.email_address,
                edad: new Date().getFullYear() - new Date(user.birth_date).getFullYear(),
                activo: user.is_active,
                configuracion: {
                    nombreMostrado: user.profile_settings.display_name,
                    tema: user.profile_settings.theme_preference,
                    notificaciones: user.profile_settings.notification_settings
                },
                balance: parseFloat(user.account_balance),
                ultimoLogin: new Date(user.last_login),
                // Campos calculados
                tieneBalance: parseFloat(user.account_balance) > 0,
                diasDesdeLogin: Math.floor((new Date() - new Date(user.last_login)) / (1000 * 60 * 60 * 24))
            }));
        }
        
        const usuariosNormalizados = normalizarUsuarios(datosAPI);
        console.log("Usuarios normalizados:", usuariosNormalizados);
        
        // Agrupar y resumir datos
        const resumen = usuariosNormalizados.reduce((acc, usuario) => {
            acc.total++;
            acc.activos += usuario.activo ? 1 : 0;
            acc.balanceTotal += usuario.balance;
            acc.edadPromedio += usuario.edad;
            
            // Agrupar por tema
            if (!acc.porTema[usuario.configuracion.tema]) {
                acc.porTema[usuario.configuracion.tema] = 0;
            }
            acc.porTema[usuario.configuracion.tema]++;
            
            return acc;
        }, {
            total: 0,
            activos: 0,
            balanceTotal: 0,
            edadPromedio: 0,
            porTema: {}
        });
        
        resumen.edadPromedio = Math.round(resumen.edadPromedio / resumen.total);
        
        console.log("Resumen de usuarios:", resumen);
        
        return { datosCamelCase, usuariosNormalizados, resumen };
    }
    
    // 🔍 BÚSQUEDA Y FILTRADO EN JSON
    static busquedaFiltrado() {
        const biblioteca = {
            nombre: "Biblioteca Central",
            ubicacion: { ciudad: "Madrid", direccion: "Calle del Libro 123" },
            categorias: [
                {
                    nombre: "Programación",
                    libros: [
                        {
                            id: 1,
                            titulo: "JavaScript: The Good Parts",
                            autor: "Douglas Crockford",
                            año: 2008,
                            isbn: "978-0596517748",
                            disponible: true,
                            etiquetas: ["javascript", "web", "programming"],
                            prestamos: [
                                { usuario: "Ana", fecha: "2024-01-10", devuelto: true },
                                { usuario: "Carlos", fecha: "2024-01-05", devuelto: true }
                            ]
                        },
                        {
                            id: 2,
                            titulo: "Clean Code",
                            autor: "Robert C. Martin",
                            año: 2008,
                            isbn: "978-0132350884",
                            disponible: false,
                            etiquetas: ["clean-code", "programming", "best-practices"],
                            prestamos: [
                                { usuario: "María", fecha: "2024-01-12", devuelto: false }
                            ]
                        }
                    ]
                },
                {
                    nombre: "Ciencia Ficción",
                    libros: [
                        {
                            id: 3,
                            titulo: "Dune",
                            autor: "Frank Herbert",
                            año: 1965,
                            isbn: "978-0441013593",
                            disponible: true,
                            etiquetas: ["sci-fi", "space", "epic"],
                            prestamos: []
                        }
                    ]
                }
            ]
        };
        
        console.log("🔍 Búsqueda y filtrado en JSON:");
        
        // Función de búsqueda por texto
        function buscarPorTexto(objeto, texto, incluirCampos = []) {
            const textoLower = texto.toLowerCase();
            const resultados = [];
            
            function buscarEnObjeto(obj, ruta = "") {
                if (Array.isArray(obj)) {
                    obj.forEach((item, index) => {
                        buscarEnObjeto(item, `${ruta}[${index}]`);
                    });
                } else if (obj && typeof obj === "object") {
                    for (const [key, value] of Object.entries(obj)) {
                        const nuevaRuta = ruta ? `${ruta}.${key}` : key;
                        
                        if (typeof value === "string" && value.toLowerCase().includes(textoLower)) {
                            if (incluirCampos.length === 0 || incluirCampos.includes(key)) {
                                resultados.push({
                                    ruta: nuevaRuta,
                                    campo: key,
                                    valor: value,
                                    objeto: obj
                                });
                            }
                        } else {
                            buscarEnObjeto(value, nuevaRuta);
                        }
                    }
                }
            }
            
            buscarEnObjeto(objeto);
            return resultados;
        }
        
        // Buscar "JavaScript" en títulos
        const resultadosJS = buscarPorTexto(biblioteca, "javascript", ["titulo", "etiquetas"]);
        console.log("Búsqueda 'JavaScript':", resultadosJS.map(r => r.valor));
        
        // Función para extraer todos los libros
        function extraerLibros(biblioteca) {
            return biblioteca.categorias.flatMap(categoria => 
                categoria.libros.map(libro => ({
                    ...libro,
                    categoria: categoria.nombre
                }))
            );
        }
        
        const todosLosLibros = extraerLibros(biblioteca);
        
        // Filtros complejos
        const filtros = {
            disponibles: (libros) => libros.filter(libro => libro.disponible),
            porAño: (libros, añoMin, añoMax) => libros.filter(libro => 
                libro.año >= añoMin && libro.año <= añoMax),
            porEtiqueta: (libros, etiqueta) => libros.filter(libro => 
                libro.etiquetas.includes(etiqueta)),
            conPrestamos: (libros) => libros.filter(libro => 
                libro.prestamos.length > 0),
            porAutor: (libros, autor) => libros.filter(libro => 
                libro.autor.toLowerCase().includes(autor.toLowerCase()))
        };
        
        console.log("Libros disponibles:", filtros.disponibles(todosLosLibros).length);
        console.log("Libros modernos (2000+):", filtros.porAño(todosLosLibros, 2000, 2024).length);
        console.log("Libros de programación:", filtros.porEtiqueta(todosLosLibros, "programming").length);
        
        // Función de búsqueda avanzada con múltiples criterios
        function busquedaAvanzada(libros, criterios) {
            return libros.filter(libro => {
                return Object.entries(criterios).every(([campo, condicion]) => {
                    const valor = libro[campo];
                    
                    if (typeof condicion === "function") {
                        return condicion(valor);
                    } else if (typeof condicion === "object" && condicion.includes) {
                        return Array.isArray(valor) ? 
                            valor.some(v => condicion.includes.includes(v)) :
                            condicion.includes.includes(valor);
                    } else {
                        return valor === condicion;
                    }
                });
            });
        }
        
        // Ejemplo de búsqueda avanzada
        const librosProgramacionDisponibles = busquedaAvanzada(todosLosLibros, {
            disponible: true,
            etiquetas: { includes: ["programming", "javascript"] },
            año: (año) => año >= 2000
        });
        
        console.log("Libros programación disponibles:", 
            librosProgramacionDisponibles.map(l => l.titulo));
        
        return { biblioteca, extraerLibros, buscarPorTexto, busquedaAvanzada };
    }
    
    // 📊 ESTADÍSTICAS Y AGREGACIONES
    static estadisticasAgregaciones() {
        const ventasData = {
            empresa: "TechStore",
            año: 2024,
            trimestres: [
                {
                    numero: 1,
                    meses: [
                        {
                            nombre: "Enero",
                            ventas: [
                                { producto: "Laptop", cantidad: 15, precio: 1200, categoria: "Hardware" },
                                { producto: "Mouse", cantidad: 45, precio: 25, categoria: "Accesorios" },
                                { producto: "Teclado", cantidad: 30, precio: 75, categoria: "Accesorios" }
                            ]
                        },
                        {
                            nombre: "Febrero", 
                            ventas: [
                                { producto: "Laptop", cantidad: 12, precio: 1200, categoria: "Hardware" },
                                { producto: "Monitor", cantidad: 8, precio: 300, categoria: "Hardware" },
                                { producto: "Mouse", cantidad: 52, precio: 25, categoria: "Accesorios" }
                            ]
                        },
                        {
                            nombre: "Marzo",
                            ventas: [
                                { producto: "Laptop", cantidad: 18, precio: 1200, categoria: "Hardware" },
                                { producto: "Tablet", cantidad: 25, precio: 500, categoria: "Hardware" },
                                { producto: "Teclado", cantidad: 35, precio: 75, categoria: "Accesorios" }
                            ]
                        }
                    ]
                }
            ]
        };
        
        console.log("📊 Estadísticas y agregaciones:");
        
        // Función para aplanar todas las ventas
        function extraerTodasVentas(data) {
            return data.trimestres.flatMap(trimestre => 
                trimestre.meses.flatMap(mes => 
                    mes.ventas.map(venta => ({
                        ...venta,
                        mes: mes.nombre,
                        trimestre: trimestre.numero,
                        ingresoTotal: venta.cantidad * venta.precio
                    }))
                )
            );
        }
        
        const todasVentas = extraerTodasVentas(ventasData);
        console.log("Total registros de ventas:", todasVentas.length);
        
        // Calcular estadísticas básicas
        const estadisticas = {
            // Ingresos totales
            ingresoTotal: todasVentas.reduce((sum, venta) => sum + venta.ingresoTotal, 0),
            
            // Cantidad total de productos vendidos
            cantidadTotal: todasVentas.reduce((sum, venta) => sum + venta.cantidad, 0),
            
            // Producto más vendido
            productoMasVendido: (() => {
                const porProducto = todasVentas.reduce((acc, venta) => {
                    acc[venta.producto] = (acc[venta.producto] || 0) + venta.cantidad;
                    return acc;
                }, {});
                
                return Object.entries(porProducto)
                    .sort(([,a], [,b]) => b - a)[0];
            })(),
            
            // Ingresos por categoría
            ingresosPorCategoria: todasVentas.reduce((acc, venta) => {
                acc[venta.categoria] = (acc[venta.categoria] || 0) + venta.ingresoTotal;
                return acc;
            }, {}),
            
            // Promedio de ingresos por mes
            promedioPorMes: (() => {
                const porMes = todasVentas.reduce((acc, venta) => {
                    acc[venta.mes] = (acc[venta.mes] || 0) + venta.ingresoTotal;
                    return acc;
                }, {});
                
                const valores = Object.values(porMes);
                return valores.reduce((sum, val) => sum + val, 0) / valores.length;
            })(),
            
            // Top 3 productos por ingresos
            top3Productos: (() => {
                const porProducto = todasVentas.reduce((acc, venta) => {
                    if (!acc[venta.producto]) {
                        acc[venta.producto] = {
                            producto: venta.producto,
                            cantidad: 0,
                            ingresos: 0,
                            categoria: venta.categoria
                        };
                    }
                    acc[venta.producto].cantidad += venta.cantidad;
                    acc[venta.producto].ingresos += venta.ingresoTotal;
                    return acc;
                }, {});
                
                return Object.values(porProducto)
                    .sort((a, b) => b.ingresos - a.ingresos)
                    .slice(0, 3);
            })()
        };
        
        console.log("💰 Estadísticas de ventas:");
        console.log("Ingreso total:", estadisticas.ingresoTotal.toLocaleString());
        console.log("Cantidad total vendida:", estadisticas.cantidadTotal);
        console.log("Producto más vendido:", estadisticas.productoMasVendido);
        console.log("Ingresos por categoría:", estadisticas.ingresosPorCategoria);
        console.log("Promedio mensual:", Math.round(estadisticas.promedioPorMes).toLocaleString());
        console.log("Top 3 productos:", estadisticas.top3Productos.map(p => 
            `${p.producto}: ${p.ingresos.toLocaleString()}`));
        
        // Función para generar reporte personalizable
        function generarReporte(ventas, configuracion) {
            const { 
                agruparPor = [], 
                metricas = ["cantidad", "ingresos"], 
                filtros = {},
                ordenPor = "ingresos",
                limite = null 
            } = configuracion;
            
            // Aplicar filtros
            let ventasFiltradas = ventas.filter(venta => {
                return Object.entries(filtros).every(([campo, valor]) => {
                    if (Array.isArray(valor)) {
                        return valor.includes(venta[campo]);
                    }
                    return venta[campo] === valor;
                });
            });
            
            // Agrupar datos
            const agrupados = ventasFiltradas.reduce((acc, venta) => {
                const clave = agruparPor.map(campo => venta[campo]).join("|");
                
                if (!acc[clave]) {
                    acc[clave] = {
                        grupo: agruparPor.reduce((obj, campo) => {
                            obj[campo] = venta[campo];
                            return obj;
                        }, {}),
                        cantidad: 0,
                        ingresos: 0,
                        registros: 0
                    };
                }
                
                acc[clave].cantidad += venta.cantidad;
                acc[clave].ingresos += venta.ingresoTotal;
                acc[clave].registros += 1;
                
                return acc;
            }, {});
            
            // Convertir a array y ordenar
            let resultado = Object.values(agrupados);
            resultado.sort((a, b) => b[ordenPor] - a[ordenPor]);
            
            // Aplicar límite
            if (limite) {
                resultado = resultado.slice(0, limite);
            }
            
            return resultado;
        }
        
        // Ejemplo de reporte personalizado
        const reportePorCategoria = generarReporte(todasVentas, {
            agruparPor: ["categoria"],
            metricas: ["cantidad", "ingresos"],
            ordenPor: "ingresos",
            limite: 5
        });
        
        console.log("📋 Reporte por categoría:", reportePorCategoria);
        
        return { ventasData, estadisticas, generarReporte };
    }
}

// 🚀 Demostraciones
console.log("🎯 MANIPULACIÓN DE DATOS JSON");
ManipulacionJSON.parsingSeguro();
ManipulacionJSON.transformacionDatos();
ManipulacionJSON.busquedaFiltrado();
ManipulacionJSON.estadisticasAgregaciones();
```

**✅ CAPÍTULO 8 COMPLETADO**

### 🎯 **Lo que acabamos de cubrir:**

1. **🌳 Navegación Profunda** - Acceso seguro, optional chaining, búsqueda recursiva
2. **🔄 Clonado de Objetos** - Shallow vs Deep copy, clonado selectivo, rendimiento
3. **🎯 Manipulación JSON** - Parsing seguro, transformaciones, búsqueda avanzada
4. **📊 Estadísticas y Agregaciones** - Análisis de datos, reportes personalizables

---

## 9. 🛠️ **Estructuras de Datos Avanzadas - PARTE 1**

### 🌟 **Introducción a Estructuras Avanzadas**

JavaScript moderno ofrece estructuras de datos especializadas que van más allá de arrays y objetos. Maps, Sets, WeakMaps y WeakSets proporcionan funcionalidades específicas para casos de uso avanzados.

```javascript
// 🛠️ Panorama de estructuras avanzadas
const ejemploEstructuras = {
    // 🗺️ MAP - Clave-valor con cualquier tipo de clave
    miMapa: new Map([
        ['string', 'valor string'],
        [42, 'valor numérico'],
        [true, 'valor booleano'],
        [{obj: true}, 'objeto como clave']
    ]),
    
    // 🎯 SET - Valores únicos
    miSet: new Set([1, 2, 3, 3, 4, 4, 5]), // Solo [1, 2, 3, 4, 5]
    
    // 💾 WEAKMAP - Referencias débiles para claves objeto
    miWeakMap: new WeakMap(),
    
    // 🔗 WEAKSET - Referencias débiles para valores objeto
    miWeakSet: new WeakSet()
};

console.log("🛠️ Estructuras avanzadas disponibles");
console.log("Map tamaño:", ejemploEstructuras.miMapa.size);
console.log("Set tamaño:", ejemploEstructuras.miSet.size);
```

### �️ **Maps - Mapas Clave-Valor Avanzados**

```javascript
// 🗺️ Maps - La evolución de los objetos
class MapsAvanzados {
    
    // 🎯 CREACIÓN Y OPERACIONES BÁSICAS
    static operacionesBasicas() {
        console.log("🗺️ Maps - Operaciones básicas:");
        
        // Crear Maps de diferentes formas
        const mapaVacio = new Map();
        
        const mapaConDatos = new Map([
            ['nombre', 'Ana'],
            ['edad', 30],
            ['activo', true]
        ]);
        
        const mapaDeObjeto = new Map(Object.entries({
            ciudad: 'Madrid',
            pais: 'España',
            codigo: 28001
        }));
        
        // Operaciones básicas
        const usuario = new Map();
        
        // set() - Agregar/actualizar
        usuario.set('id', 12345);
        usuario.set('nombre', 'Carlos');
        usuario.set('email', 'carlos@email.com');
        usuario.set('registro', new Date());
        
        // get() - Obtener valor
        console.log("Nombre:", usuario.get('nombre'));
        console.log("Email:", usuario.get('email'));
        console.log("Inexistente:", usuario.get('telefono')); // undefined
        
        // has() - Verificar existencia
        console.log("¿Tiene email?", usuario.has('email')); // true
        console.log("¿Tiene telefono?", usuario.has('telefono')); // false
        
        // delete() - Eliminar
        usuario.delete('registro');
        console.log("Después de eliminar registro:", usuario.has('registro')); // false
        
        // size - Tamaño
        console.log("Tamaño del mapa:", usuario.size);
        
        // clear() - Limpiar todo
        const mapaTemporal = new Map([['a', 1], ['b', 2]]);
        console.log("Antes clear:", mapaTemporal.size); // 2
        mapaTemporal.clear();
        console.log("Después clear:", mapaTemporal.size); // 0
        
        return { mapaVacio, mapaConDatos, usuario };
    }
    
    // 🔑 CLAVES DE CUALQUIER TIPO
    static clavesAvanzadas() {
        console.log("🔑 Claves de cualquier tipo:");
        
        const mapaFlexible = new Map();
        
        // Claves primitivas
        mapaFlexible.set('string', 'Clave string');
        mapaFlexible.set(42, 'Clave número');
        mapaFlexible.set(true, 'Clave boolean');
        mapaFlexible.set(null, 'Clave null');
        mapaFlexible.set(undefined, 'Clave undefined');
        
        // Claves objeto
        const objetoClave = { tipo: 'configuracion' };
        const arraysClave = [1, 2, 3];
        const funcionClave = () => 'hola';
        const fechaClave = new Date();
        
        mapaFlexible.set(objetoClave, 'Valor para objeto');
        mapaFlexible.set(arraysClave, 'Valor para array');
        mapaFlexible.set(funcionClave, 'Valor para función');
        mapaFlexible.set(fechaClave, 'Valor para fecha');
        
        console.log("Valores por clave:");
        console.log("String:", mapaFlexible.get('string'));
        console.log("Número:", mapaFlexible.get(42));
        console.log("Objeto:", mapaFlexible.get(objetoClave));
        console.log("Array:", mapaFlexible.get(arraysClave));
        console.log("Función:", mapaFlexible.get(funcionClave));
        
        // ⚠️ Importante: Las claves objeto se comparen por referencia
        const otroObjeto = { tipo: 'configuracion' }; // Mismo contenido, diferente referencia
        console.log("¿Tiene otro objeto?", mapaFlexible.has(otroObjeto)); // false
        console.log("¿Tiene objeto original?", mapaFlexible.has(objetoClave)); // true
        
        // Ejemplo práctico: Cache con objetos como claves
        const cache = new Map();
        
        function obtenerDatosUsuario(usuario) {
            if (cache.has(usuario)) {
                console.log("📄 Datos desde cache para:", usuario.nombre);
                return cache.get(usuario);
            }
            
            // Simular obtención de datos
            const datos = {
                perfil: `Perfil de ${usuario.nombre}`,
                configuracion: { tema: 'claro', idioma: 'es' },
                timestamp: new Date()
            };
            
            cache.set(usuario, datos);
            console.log("🆕 Datos calculados para:", usuario.nombre);
            return datos;
        }
        
        const usuario1 = { id: 1, nombre: 'Ana' };
        const usuario2 = { id: 2, nombre: 'Pedro' };
        
        // Primera llamada - se calcula
        obtenerDatosUsuario(usuario1);
        obtenerDatosUsuario(usuario2);
        
        // Segunda llamada - desde cache
        obtenerDatosUsuario(usuario1);
        obtenerDatosUsuario(usuario2);
        
        console.log("Tamaño del cache:", cache.size);
        
        return { mapaFlexible, cache, obtenerDatosUsuario };
    }
    
    // 🔄 ITERACIÓN Y TRANSFORMACIÓN
    static iteracionTransformacion() {
        console.log("🔄 Iteración y transformación:");
        
        const productos = new Map([
            ['laptop', { precio: 1200, categoria: 'electronics', stock: 15 }],
            ['mouse', { precio: 25, categoria: 'electronics', stock: 50 }],
            ['libro', { precio: 20, categoria: 'books', stock: 30 }],
            ['camiseta', { precio: 15, categoria: 'clothing', stock: 100 }]
        ]);
        
        console.log("📦 Productos disponibles:");
        
        // Iterar con for...of
        console.log("\n🔄 Iteración con for...of:");
        for (const [nombre, info] of productos) {
            console.log(`${nombre}: €${info.precio} (${info.stock} disponibles)`);
        }
        
        // Iterar solo claves
        console.log("\n🔑 Solo nombres:");
        for (const nombre of productos.keys()) {
            console.log(`- ${nombre}`);
        }
        
        // Iterar solo valores
        console.log("\n💰 Solo precios:");
        for (const info of productos.values()) {
            console.log(`€${info.precio}`);
        }
        
        // forEach()
        console.log("\n📋 Resumen con forEach:");
        productos.forEach((info, nombre) => {
            const total = info.precio * info.stock;
            console.log(`${nombre}: valor total €${total}`);
        });
        
        // Convertir a Array para usar métodos de array
        const productosArray = [...productos];
        console.log("\n📊 Como array:", productosArray);
        
        // Filtrar productos caros (precio > 20)
        const productosCaros = new Map(
            [...productos].filter(([nombre, info]) => info.precio > 20)
        );
        console.log("\n💎 Productos caros:");
        productosCaros.forEach((info, nombre) => {
            console.log(`${nombre}: €${info.precio}`);
        });
        
        // Transformar precios (aplicar descuento 10%)
        const productosConDescuento = new Map();
        productos.forEach((info, nombre) => {
            const infoConDescuento = {
                ...info,
                precio: Math.round(info.precio * 0.9),
                precioOriginal: info.precio
            };
            productosConDescuento.set(nombre, infoConDescuento);
        });
        
        console.log("\n🏷️ Con descuento 10%:");
        productosConDescuento.forEach((info, nombre) => {
            console.log(`${nombre}: €${info.precio} (era €${info.precioOriginal})`);
        });
        
        // Agrupar por categoría
        const porCategoria = new Map();
        productos.forEach((info, nombre) => {
            const categoria = info.categoria;
            if (!porCategoria.has(categoria)) {
                porCategoria.set(categoria, []);
            }
            porCategoria.get(categoria).push({ nombre, ...info });
        });
        
        console.log("\n📂 Agrupados por categoría:");
        porCategoria.forEach((items, categoria) => {
            console.log(`${categoria}:`, items.map(item => item.nombre).join(', '));
        });
        
        return { productos, productosCaros, productosConDescuento, porCategoria };
    }
    
    // 🆚 MAP VS OBJECT
    static mapVsObject() {
        console.log("🆚 Map vs Object:");
        
        // Crear datos de prueba
        const datosTest = [];
        for (let i = 0; i < 1000; i++) {
            datosTest.push([`key${i}`, `value${i}`]);
        }
        
        // Object tradicional
        console.time("⏱️ Object - Creación");
        const objeto = {};
        datosTest.forEach(([key, value]) => {
            objeto[key] = value;
        });
        console.timeEnd("⏱️ Object - Creación");
        
        // Map
        console.time("⏱️ Map - Creación");
        const mapa = new Map(datosTest);
        console.timeEnd("⏱️ Map - Creación");
        
        // Acceso a elementos
        const keyTest = 'key500';
        
        console.time("⏱️ Object - Acceso");
        const valorObjeto = objeto[keyTest];
        console.timeEnd("⏱️ Object - Acceso");
        
        console.time("⏱️ Map - Acceso");
        const valorMapa = mapa.get(keyTest);
        console.timeEnd("⏱️ Map - Acceso");
        
        // Iteración
        console.time("⏱️ Object - Iteración");
        let contadorObjeto = 0;
        for (const key in objeto) {
            contadorObjeto++;
        }
        console.timeEnd("⏱️ Object - Iteración");
        
        console.time("⏱️ Map - Iteración");
        let contadorMapa = 0;
        for (const [key, value] of mapa) {
            contadorMapa++;
        }
        console.timeEnd("⏱️ Map - Iteración");
        
        // Comparación de características
        console.log("\n📊 Comparación de características:");
        
        const comparacion = {
            'Tamaño': {
                'Object': `${Object.keys(objeto).length} (calculado)`,
                'Map': `${mapa.size} (propiedad)`
            },
            'Claves': {
                'Object': 'Solo strings/symbols',
                'Map': 'Cualquier tipo'
            },
            'Orden': {
                'Object': 'No garantizado (< ES2015)',
                'Map': 'Orden de inserción'
            },
            'Iteración': {
                'Object': 'for...in, Object.keys()',
                'Map': 'for...of, forEach()'
            },
            'Rendimiento': {
                'Object': 'Optimizado para propiedades',
                'Map': 'Optimizado para inserción/eliminación'
            },
            'Prototipo': {
                'Object': 'Hereda de Object.prototype',
                'Map': 'Sin claves por defecto'
            }
        };
        
        console.table(comparacion);
        
        // Casos de uso recomendados
        console.log("\n✅ Cuándo usar cada uno:");
        console.log("📦 Usar OBJECT cuando:");
        console.log("  - Las claves son strings conocidos");
        console.log("  - Necesitas JSON.stringify()");
        console.log("  - Trabajas con propiedades como métodos");
        console.log("  - Rendimiento de acceso es crítico");
        
        console.log("\n🗺️ Usar MAP cuando:");
        console.log("  - Las claves pueden ser cualquier tipo");
        console.log("  - Necesitas el tamaño frecuentemente");
        console.log("  - Inserción/eliminación frecuente");
        console.log("  - Necesitas iteración ordenada");
        console.log("  - Evitar colisiones con prototype");
        
        return { objeto, mapa, comparacion };
    }
}

// 🚀 Demostraciones Maps
console.log("🗺️ MAPS AVANZADOS");
MapsAvanzados.operacionesBasicas();
MapsAvanzados.clavesAvanzadas();
MapsAvanzados.iteracionTransformacion();
MapsAvanzados.mapVsObject();
```

### 🎯 **Sets - Colecciones de Valores Únicos**

```javascript
// 🎯 Sets - Colecciones sin duplicados
class SetsAvanzados {
    
    // 🎯 OPERACIONES BÁSICAS
    static operacionesBasicas() {
        console.log("🎯 Sets - Operaciones básicas:");
        
        // Crear Sets de diferentes formas
        const setVacio = new Set();
        
        const setConDatos = new Set([1, 2, 3, 4, 5]);
        
        const setConDuplicados = new Set([1, 1, 2, 2, 3, 3]);
        console.log("Set con duplicados:", [...setConDuplicados]); // [1, 2, 3]
        
        const setDeString = new Set('hello');
        console.log("Set de string:", [...setDeString]); // ['h', 'e', 'l', 'o']
        
        // Operaciones básicas
        const frutas = new Set();
        
        // add() - Agregar elementos
        frutas.add('manzana');
        frutas.add('banana');
        frutas.add('naranja');
        frutas.add('manzana'); // Duplicado - no se agrega
        
        console.log("Frutas únicas:", frutas.size); // 3
        
        // has() - Verificar existencia
        console.log("¿Tiene manzana?", frutas.has('manzana')); // true
        console.log("¿Tiene pera?", frutas.has('pera')); // false
        
        // delete() - Eliminar
        frutas.delete('banana');
        console.log("Después de eliminar banana:", [...frutas]); // ['manzana', 'naranja']
        
        // Agregar múltiples elementos
        const nuevasFrutas = ['pera', 'uva', 'fresa'];
        nuevasFrutas.forEach(fruta => frutas.add(fruta));
        console.log("Con nuevas frutas:", [...frutas]);
        
        // clear() - Limpiar todo
        const setTemporal = new Set([1, 2, 3]);
        console.log("Antes clear:", setTemporal.size); // 3
        setTemporal.clear();
        console.log("Después clear:", setTemporal.size); // 0
        
        return { frutas, setConDatos, setDeString };
    }
    
    // 🔄 ITERACIÓN Y VALORES
    static iteracionValores() {
        console.log("🔄 Iteración en Sets:");
        
        const numeros = new Set([10, 20, 30, 40, 50]);
        
        // for...of
        console.log("Con for...of:");
        for (const numero of numeros) {
            console.log(`Número: ${numero}`);
        }
        
        // forEach()
        console.log("\nCon forEach:");
        numeros.forEach((valor, valorCopia, set) => {
            // En Sets, valor === valorCopia (por compatibilidad con Maps)
            console.log(`Valor: ${valor}, Set size: ${set.size}`);
        });
        
        // Convertir a Array
        const numerosArray = [...numeros];
        console.log("Como array:", numerosArray);
        
        // values() y keys() (son idénticos en Sets)
        console.log("Values iterator:", [...numeros.values()]);
        console.log("Keys iterator:", [...numeros.keys()]); // Mismo resultado
        
        // entries() - devuelve [valor, valor]
        console.log("Entries iterator:");
        for (const [key, value] of numeros.entries()) {
            console.log(`[${key}, ${value}]`); // key === value
        }
        
        return numeros;
    }
    
    // 🧮 OPERACIONES MATEMÁTICAS DE CONJUNTOS
    static operacionesConjuntos() {
        console.log("🧮 Operaciones matemáticas de conjuntos:");
        
        const setA = new Set([1, 2, 3, 4, 5]);
        const setB = new Set([4, 5, 6, 7, 8]);
        const setC = new Set([1, 2, 3]);
        
        console.log("Set A:", [...setA]);
        console.log("Set B:", [...setB]);
        console.log("Set C:", [...setC]);
        
        // 🤝 UNIÓN (A ∪ B)
        const union = new Set([...setA, ...setB]);
        console.log("A ∪ B (Unión):", [...union]); // [1,2,3,4,5,6,7,8]
        
        // 🔗 INTERSECCIÓN (A ∩ B)
        const interseccion = new Set([...setA].filter(x => setB.has(x)));
        console.log("A ∩ B (Intersección):", [...interseccion]); // [4,5]
        
        // ➖ DIFERENCIA (A - B)
        const diferencia = new Set([...setA].filter(x => !setB.has(x)));
        console.log("A - B (Diferencia):", [...diferencia]); // [1,2,3]
        
        // ⚡ DIFERENCIA SIMÉTRICA (A ⊕ B)
        const diferenciaSimetrica = new Set([
            ...[...setA].filter(x => !setB.has(x)),
            ...[...setB].filter(x => !setA.has(x))
        ]);
        console.log("A ⊕ B (Dif. Simétrica):", [...diferenciaSimetrica]); // [1,2,3,6,7,8]
        
        // 📊 RELACIONES DE CONJUNTOS
        
        // ¿Es subconjunto? (C ⊆ A)
        const esSubconjunto = [...setC].every(x => setA.has(x));
        console.log("¿C es subconjunto de A?", esSubconjunto); // true
        
        // ¿Es superconjunto? (A ⊇ C)
        const esSuperconjunto = [...setC].every(x => setA.has(x));
        console.log("¿A es superconjunto de C?", esSuperconjunto); // true
        
        // ¿Son disjuntos? (A ∩ B = ∅)
        const sonDisjuntos = [...setA].every(x => !setB.has(x));
        console.log("¿A y B son disjuntos?", sonDisjuntos); // false
        
        // Funciones utilitarias para operaciones
        const OperacionesSet = {
            union: (setA, setB) => new Set([...setA, ...setB]),
            interseccion: (setA, setB) => new Set([...setA].filter(x => setB.has(x))),
            diferencia: (setA, setB) => new Set([...setA].filter(x => !setB.has(x))),
            diferenciaSimetrica: (setA, setB) => new Set([
                ...[...setA].filter(x => !setB.has(x)),
                ...[...setB].filter(x => !setA.has(x))
            ]),
            esSubconjunto: (setA, setB) => [...setA].every(x => setB.has(x)),
            esSuperconjunto: (setA, setB) => [...setB].every(x => setA.has(x)),
            sonDisjuntos: (setA, setB) => [...setA].every(x => !setB.has(x))
        };
        
        // Ejemplos prácticos
        console.log("\n🔧 Ejemplos prácticos:");
        
        const usuariosOnline = new Set(['ana', 'carlos', 'elena', 'pedro']);
        const usuariosVIP = new Set(['carlos', 'elena', 'sofia', 'miguel']);
        
        const vipOnline = OperacionesSet.interseccion(usuariosOnline, usuariosVIP);
        console.log("Usuarios VIP online:", [...vipOnline]);
        
        const todosUsuarios = OperacionesSet.union(usuariosOnline, usuariosVIP);
        console.log("Todos los usuarios:", [...todosUsuarios]);
        
        const soloOnline = OperacionesSet.diferencia(usuariosOnline, usuariosVIP);
        console.log("Solo online (no VIP):", [...soloOnline]);
        
        return { setA, setB, setC, OperacionesSet, union, interseccion };
    }
    
    // 🎯 CASOS DE USO PRÁCTICOS
    static casosUsoPracticos() {
        console.log("🎯 Casos de uso prácticos:");
        
        // 1. ELIMINAR DUPLICADOS DE ARRAYS
        console.log("1️⃣ Eliminar duplicados:");
        const numerosConDuplicados = [1, 2, 2, 3, 3, 3, 4, 4, 5];
        const numerosUnicos = [...new Set(numerosConDuplicados)];
        console.log("Original:", numerosConDuplicados);
        console.log("Sin duplicados:", numerosUnicos);
        
        // 2. VALIDAR UNICIDAD EN FORMULARIOS
        console.log("\n2️⃣ Validar emails únicos:");
        const emailsFormulario = [
            'ana@email.com',
            'carlos@email.com',
            'ana@email.com', // Duplicado
            'elena@email.com'
        ];
        
        const emailsUnicos = new Set(emailsFormulario);
        if (emailsUnicos.size !== emailsFormulario.length) {
            console.log(`❌ Hay ${emailsFormulario.length - emailsUnicos.size} email(s) duplicado(s)`);
        } else {
            console.log("✅ Todos los emails son únicos");
        }
        
        // 3. TRACKING DE ELEMENTOS VISITADOS
        console.log("\n3️⃣ Tracking de páginas visitadas:");
        const paginasVisitadas = new Set();
        
        function visitarPagina(url) {
            if (paginasVisitadas.has(url)) {
                console.log(`🔄 Revisitando: ${url}`);
            } else {
                console.log(`🆕 Primera visita: ${url}`);
                paginasVisitadas.add(url);
            }
        }
        
        visitarPagina('/home');
        visitarPagina('/products');
        visitarPagina('/home'); // Revisita
        visitarPagina('/contact');
        visitarPagina('/products'); // Revisita
        
        console.log(`� Total páginas únicas visitadas: ${paginasVisitadas.size}`);
        
        // 4. FILTRAR ELEMENTOS ÚNICOS EN OBJETOS
        console.log("\n4️⃣ IDs únicos de objetos:");
        const productos = [
            { id: 1, nombre: 'Laptop' },
            { id: 2, nombre: 'Mouse' },
            { id: 1, nombre: 'Laptop Pro' }, // ID duplicado
            { id: 3, nombre: 'Teclado' },
            { id: 2, nombre: 'Mouse Gamer' } // ID duplicado
        ];
        
        const idsUnicos = new Set(productos.map(p => p.id));
        console.log("IDs únicos:", [...idsUnicos]);
        
        // Filtrar productos con IDs únicos (primer encontrado)
        const productosUnicos = productos.filter((producto, index) => {
            return productos.findIndex(p => p.id === producto.id) === index;
        });
        console.log("Productos únicos:", productosUnicos);
        
        // 5. CACHE DE RESULTADOS ÚNICOS
        console.log("\n5️⃣ Cache de búsquedas únicas:");
        const busquedasRealizadas = new Set();
        const resultadosCache = new Map();
        
        function buscar(termino) {
            if (busquedasRealizadas.has(termino)) {
                console.log(`📄 Término ya buscado: "${termino}"`);
                return resultadosCache.get(termino);
            }
            
            // Simular búsqueda costosa
            console.log(`🔍 Buscando por primera vez: "${termino}"`);
            const resultados = [`Resultado 1 para ${termino}`, `Resultado 2 para ${termino}`];
            
            busquedasRealizadas.add(termino);
            resultadosCache.set(termino, resultados);
            
            return resultados;
        }
        
        buscar('javascript');
        buscar('python');
        buscar('javascript'); // Cache hit
        buscar('react');
        buscar('python'); // Cache hit
        
        console.log(`📊 Búsquedas únicas realizadas: ${busquedasRealizadas.size}`);
        console.log("Términos buscados:", [...busquedasRealizadas]);
        
        return { 
            numerosUnicos, 
            emailsUnicos, 
            paginasVisitadas, 
            productosUnicos,
            busquedasRealizadas 
        };
    }
}

// 🚀 Demostraciones Sets
console.log("🎯 SETS AVANZADOS");
SetsAvanzados.operacionesBasicas();
SetsAvanzados.iteracionValores();
SetsAvanzados.operacionesConjuntos();
SetsAvanzados.casosUsoPracticos();
```
---

## 9.2 🛠️ **Estructuras de Datos Avanzadas - PARTE 2**

### 💾 **WeakMaps - Referencias Débiles Básicas**

```javascript
// 💾 WeakMaps - Introducción y conceptos fundamentales
class WeakMapsBasicos {
    
    // 🎯 CONCEPTOS ESENCIALES
    static conceptosEsenciales() {
        console.log("💾 WeakMaps - Conceptos esenciales:");
        
        const weakMap = new WeakMap();
        
        // ✅ Solo objetos como claves
        const usuario1 = { id: 1, nombre: 'Ana' };
        const usuario2 = { id: 2, nombre: 'Carlos' };
        
        // Agregar datos asociados
        weakMap.set(usuario1, {
            ultimoLogin: new Date(),
            preferencias: { tema: 'oscuro' }
        });
        
        weakMap.set(usuario2, {
            ultimoLogin: new Date('2024-01-10'),
            preferencias: { tema: 'claro' }
        });
        
        console.log("¿Tiene usuario1?", weakMap.has(usuario1)); // true
        console.log("Datos usuario1:", weakMap.get(usuario1));
        
        // Características especiales
        console.log("\n⚠️ Características WeakMap:");
        console.log("- No tiene .size");
        console.log("- No es iterable");
        console.log("- Referencias débiles (GC automático)");
        console.log("- Solo métodos: get(), set(), has(), delete()");
        
        return { weakMap, usuario1, usuario2 };
    }
    
    // 🔐 DATOS PRIVADOS SIMPLES
    static datosPrivados() {
        console.log("🔐 Datos privados con WeakMap:");
        
        const datosPrivados = new WeakMap();
        
        class Usuario {
            constructor(nombre, email) {
                this.nombre = nombre;
                this.email = email;
                
                // Datos privados en WeakMap
                datosPrivados.set(this, {
                    id: Math.random().toString(36).substr(2, 9),
                    fechaCreacion: new Date(),
                    activo: true
                });
            }
            
            obtenerInfo() {
                const privados = datosPrivados.get(this);
                return {
                    nombre: this.nombre,
                    email: this.email,
                    id: privados.id,
                    activo: privados.activo
                };
            }
            
            activar() {
                const privados = datosPrivados.get(this);
                privados.activo = true;
                return "Usuario activado";
            }
            
            desactivar() {
                const privados = datosPrivados.get(this);
                privados.activo = false;
                return "Usuario desactivado";
            }
        }
        
        const usuario = new Usuario("Elena", "elena@email.com");
        console.log("Info usuario:", usuario.obtenerInfo());
        console.log(usuario.desactivar());
        console.log("Info después:", usuario.obtenerInfo());
        
        return { Usuario, usuario };
    }
    
    // 📄 CACHE CON LIMPIEZA AUTOMÁTICA
    static cacheAutomatico() {
        console.log("📄 Cache con limpieza automática:");
        
        const cache = new WeakMap();
        
        function procesarObjeto(objeto) {
            // Verificar cache
            if (cache.has(objeto)) {
                console.log("📄 Desde cache");
                return cache.get(objeto);
            }
            
            // Procesar (simular trabajo pesado)
            console.log("🔄 Procesando...");
            const resultado = {
                procesado: true,
                datos: Object.keys(objeto).length,
                timestamp: new Date()
            };
            
            // Guardar en cache
            cache.set(objeto, resultado);
            return resultado;
        }
        
        const obj1 = { a: 1, b: 2, c: 3 };
        const obj2 = { x: 10, y: 20 };
        
        // Primera vez - se procesa
        console.log("Primera llamada obj1:", procesarObjeto(obj1));
        // Segunda vez - desde cache
        console.log("Segunda llamada obj1:", procesarObjeto(obj1));
        
        console.log("Primera llamada obj2:", procesarObjeto(obj2));
        
        return { procesarObjeto, cache };
    }
}

// 🚀 Demostraciones WeakMaps
console.log("💾 WEAKMAPS BÁSICOS");
WeakMapsBasicos.conceptosEsenciales();
WeakMapsBasicos.datosPrivados();
WeakMapsBasicos.cacheAutomatico();
```

### 🔗 **WeakSets - Referencias Débiles para Colecciones**

```javascript
// 🔗 WeakSets - Colecciones con referencias débiles
class WeakSetsBasicos {
    
    // 🎯 CONCEPTOS BÁSICOS
    static conceptosBasicos() {
        console.log("🔗 WeakSets - Conceptos básicos:");
        
        const weakSet = new WeakSet();
        
        // ✅ Solo objetos
        const obj1 = { id: 1, tipo: 'usuario' };
        const obj2 = { id: 2, tipo: 'admin' };
        
        weakSet.add(obj1);
        weakSet.add(obj2);
        
        console.log("¿Tiene obj1?", weakSet.has(obj1)); // true
        console.log("¿Tiene obj2?", weakSet.has(obj2)); // true
        
        // Eliminar
        weakSet.delete(obj2);
        console.log("¿Tiene obj2 después de delete?", weakSet.has(obj2)); // false
        
        console.log("\n⚠️ Características WeakSet:");
        console.log("- No tiene .size");
        console.log("- No es iterable");
        console.log("- Solo métodos: add(), has(), delete()");
        console.log("- Referencias débiles");
        
        return { weakSet, obj1 };
    }
    
    // 🔐 TRACKING DE OBJETOS
    static trackingObjetos() {
        console.log("🔐 Tracking de objetos:");
        
        const objetosProcessados = new WeakSet();
        const objetosValidados = new WeakSet();
        
        function procesar(objeto) {
            if (objetosProcessados.has(objeto)) {
                console.log("✅ Ya procesado");
                return "procesado_anteriormente";
            }
            
            console.log("🔄 Procesando...");
            objetosProcessados.add(objeto);
            return "procesado_ahora";
        }
        
        function validar(objeto) {
            if (!objetosProcessados.has(objeto)) {
                return "error_no_procesado";
            }
            
            if (objetosValidados.has(objeto)) {
                console.log("✅ Ya validado");
                return "validado_anteriormente";
            }
            
            console.log("🔍 Validando...");
            objetosValidados.add(objeto);
            return "validado_ahora";
        }
        
        const datos1 = { nombre: "Test 1" };
        const datos2 = { nombre: "Test 2" };
        
        console.log("Procesar datos1:", procesar(datos1));
        console.log("Validar datos1:", validar(datos1));
        console.log("Procesar datos1 otra vez:", procesar(datos1));
        console.log("Validar datos2 sin procesar:", validar(datos2));
        
        return { procesar, validar, objetosProcessados, objetosValidados };
    }
    
    // 🛡️ CONTROL DE ACCESO
    static controlAcceso() {
        console.log("🛡️ Control de acceso simple:");
        
        const usuariosAutorizados = new WeakSet();
        const usuariosBloqueados = new WeakSet();
        
        function autorizar(usuario) {
            usuariosAutorizados.add(usuario);
            usuariosBloqueados.delete(usuario);
            console.log(`✅ ${usuario.nombre} autorizado`);
        }
        
        function bloquear(usuario) {
            usuariosBloqueados.add(usuario);
            usuariosAutorizados.delete(usuario);
            console.log(`🚫 ${usuario.nombre} bloqueado`);
        }
        
        function tieneAcceso(usuario) {
            if (usuariosBloqueados.has(usuario)) {
                return false;
            }
            return usuariosAutorizados.has(usuario);
        }
        
        const usuario1 = { nombre: "Ana" };
        const usuario2 = { nombre: "Carlos" };
        
        autorizar(usuario1);
        autorizar(usuario2);
        
        console.log("Ana tiene acceso:", tieneAcceso(usuario1));
        console.log("Carlos tiene acceso:", tieneAcceso(usuario2));
        
        bloquear(usuario2);
        console.log("Carlos después de bloqueo:", tieneAcceso(usuario2));
        
        return { autorizar, bloquear, tieneAcceso };
    }
}

// 🚀 Demostraciones WeakSets
console.log("🔗 WEAKSETS BÁSICOS");
WeakSetsBasicos.conceptosBasicos();
WeakSetsBasicos.trackingObjetos();
WeakSetsBasicos.controlAcceso();
```

### 🆚 **Comparación Rápida: Strong vs Weak**

```javascript
// 🆚 Comparación esencial entre estructuras
class ComparacionRapida {
    
    static comparacionEsencial() {
        console.log("🆚 Comparación esencial:");
        
        // Estructuras normales (fuertes)
        const map = new Map();
        const set = new Set();
        
        // Estructuras débiles
        const weakMap = new WeakMap();
        const weakSet = new WeakSet();
        
        let obj = { test: true };
        
        // Agregar a todas
        map.set(obj, "valor");
        set.add(obj);
        weakMap.set(obj, "valor");
        weakSet.add(obj);
        
        console.log("📊 Estado inicial:");
        console.log("Map size:", map.size);
        console.log("Set size:", set.size);
        console.log("WeakMap tiene obj:", weakMap.has(obj));
        console.log("WeakSet tiene obj:", weakSet.has(obj));
        
        // Tabla comparativa simple
        const comparacion = {
            'Referencia': {
                'Map/Set': 'Fuerte - impide GC',
                'WeakMap/WeakSet': 'Débil - permite GC'
            },
            'Iteración': {
                'Map/Set': '✅ for...of, forEach',
                'WeakMap/WeakSet': '❌ No iterable'
            },
            'Tamaño': {
                'Map/Set': '✅ .size disponible',
                'WeakMap/WeakSet': '❌ No disponible'
            },
            'Claves': {
                'Map/Set': 'Cualquier tipo',
                'WeakMap/WeakSet': 'Solo objetos'
            }
        };
        
        console.table(comparacion);
        
        // Cuándo usar cada una
        console.log("\n🎯 Cuándo usar:");
        console.log("📦 Map/Set:");
        console.log("  - Necesitas iterar");
        console.log("  - Quieres conocer el tamaño");
        console.log("  - Control manual del ciclo de vida");
        
        console.log("💾 WeakMap/WeakSet:");
        console.log("  - Metadata de objetos");
        console.log("  - Datos privados");
        console.log("  - Cache temporal");
        console.log("  - Evitar memory leaks");
        
        return { map, set, weakMap, weakSet, obj };
    }
    
    // 🧠 GESTIÓN DE MEMORIA
    static gestionMemoria() {
        console.log("🧠 Gestión de memoria:");
        
        // Problema con Map (memory leak)
        const problemaMap = new Map();
        function crearObjetos() {
            for (let i = 0; i < 3; i++) {
                const obj = { id: i, data: `objeto${i}` };
                problemaMap.set(obj, `valor${i}`);
            }
        }
        crearObjetos();
        console.log("Map después de crear objetos:", problemaMap.size);
        // Los objetos permanecen en memoria aunque no los usemos
        
        // Solución con WeakMap
        const solucionWeakMap = new WeakMap();
        function crearObjetosSeguro() {
            const objetos = [];
            for (let i = 0; i < 3; i++) {
                const obj = { id: i, data: `objeto${i}` };
                solucionWeakMap.set(obj, `valor${i}`);
                objetos.push(obj);
            }
            return objetos;
        }
        
        let objetosTemp = crearObjetosSeguro();
        console.log("WeakMap tiene primer objeto:", solucionWeakMap.has(objetosTemp[0]));
        
        // Eliminar referencias
        objetosTemp = null;
        console.log("Referencias eliminadas - GC limpiará WeakMap automáticamente");
        
        return { problemaMap, solucionWeakMap };
    }
}

// 🚀 Demostración final
console.log("🆚 COMPARACIÓN ESTRUCTURAS");
ComparacionRapida.comparacionEsencial();
ComparacionRapida.gestionMemoria();
```
---

## 9.3 🛠️ **Estructuras de Datos Avanzadas - PARTE 3**

### 🌟 **Patrones Avanzados con WeakMaps**

```javascript
// 🌟 Patrones avanzados y casos reales con WeakMaps
class WeakMapPatronesAvanzados {
    
    // 🏗️ PATRÓN: FACTORY CON DATOS PRIVADOS
    static factoryDatosPrivados() {
        console.log("🏗️ Factory con datos privados:");
        
        const datosPrivados = new WeakMap();
        const metodosPrivados = new WeakMap();
        
        function CrearUsuario(nombre, email, rol = 'usuario') {
            const instancia = {};
            
            // Datos completamente privados
            datosPrivados.set(instancia, {
                id: Math.random().toString(36).substr(2, 9),
                password: null,
                intentosLogin: 0,
                bloqueado: false,
                ultimoAcceso: null
            });
            
            // Métodos privados
            metodosPrivados.set(instancia, {
                validarPassword: (password) => {
                    const datos = datosPrivados.get(instancia);
                    return datos.password === password;
                },
                incrementarIntentos: () => {
                    const datos = datosPrivados.get(instancia);
                    datos.intentosLogin++;
                    if (datos.intentosLogin >= 3) {
                        datos.bloqueado = true;
                    }
                },
                resetearIntentos: () => {
                    const datos = datosPrivados.get(instancia);
                    datos.intentosLogin = 0;
                    datos.bloqueado = false;
                }
            });
            
            // API pública
            instancia.nombre = nombre;
            instancia.email = email;
            instancia.rol = rol;
            
            instancia.establecerPassword = function(nuevaPassword) {
                if (nuevaPassword.length < 6) {
                    return { exito: false, error: "Password muy corta" };
                }
                datosPrivados.get(this).password = nuevaPassword;
                return { exito: true };
            };
            
            instancia.login = function(password) {
                const datos = datosPrivados.get(this);
                const metodos = metodosPrivados.get(this);
                
                if (datos.bloqueado) {
                    return { exito: false, error: "Usuario bloqueado" };
                }
                
                if (metodos.validarPassword(password)) {
                    metodos.resetearIntentos();
                    datos.ultimoAcceso = new Date();
                    return { exito: true, mensaje: "Login exitoso" };
                } else {
                    metodos.incrementarIntentos();
                    return { 
                        exito: false, 
                        error: `Password incorrecto. Intentos: ${datos.intentosLogin}/3` 
                    };
                }
            };
            
            instancia.obtenerEstado = function() {
                const datos = datosPrivados.get(this);
                return {
                    id: datos.id,
                    intentosLogin: datos.intentosLogin,
                    bloqueado: datos.bloqueado,
                    ultimoAcceso: datos.ultimoAcceso
                };
            };
            
            return instancia;
        }
        
        // Demostración
        const usuario = CrearUsuario("Elena", "elena@email.com", "admin");
        console.log("Usuario creado:", usuario.nombre, usuario.email);
        
        console.log(usuario.establecerPassword("123456"));
        console.log("Login correcto:", usuario.login("123456"));
        console.log("Estado:", usuario.obtenerEstado());
        
        console.log("Login incorrecto:", usuario.login("wrong"));
        console.log("Login incorrecto 2:", usuario.login("wrong"));
        console.log("Login incorrecto 3:", usuario.login("wrong"));
        console.log("Estado final:", usuario.obtenerEstado());
        
        return { CrearUsuario, usuario };
    }
    
    // 🔄 PATRÓN: OBSERVER CON WEAKMAP
    static observerPattern() {
        console.log("🔄 Patrón Observer:");
        
        const observadores = new WeakMap();
        const estadoPrivado = new WeakMap();
        
        class Observable {
            constructor() {
                observadores.set(this, new Set());
                estadoPrivado.set(this, {});
            }
            
            suscribir(observer, eventos = ['*']) {
                const obs = observadores.get(this);
                eventos.forEach(evento => {
                    if (!obs.has(evento)) {
                        obs.add({ evento, callback: observer });
                    }
                });
            }
            
            desuscribir(observer) {
                const obs = observadores.get(this);
                const toDelete = [];
                obs.forEach(item => {
                    if (item.callback === observer) {
                        toDelete.push(item);
                    }
                });
                toDelete.forEach(item => obs.delete(item));
            }
            
            notificar(evento, datos) {
                const obs = observadores.get(this);
                obs.forEach(item => {
                    if (item.evento === evento || item.evento === '*') {
                        item.callback(evento, datos, this);
                    }
                });
            }
            
            establecerEstado(clave, valor) {
                const estado = estadoPrivado.get(this);
                const valorAnterior = estado[clave];
                estado[clave] = valor;
                
                this.notificar('cambioEstado', {
                    clave, 
                    valorAnterior, 
                    valorNuevo: valor
                });
            }
            
            obtenerEstado(clave) {
                const estado = estadoPrivado.get(this);
                return clave ? estado[clave] : { ...estado };
            }
        }
        
        // Uso del patrón
        const modelo = new Observable();
        
        const observer1 = (evento, datos) => {
            console.log(`🔔 Observer 1 - ${evento}:`, datos);
        };
        
        const observer2 = (evento, datos) => {
            console.log(`🔔 Observer 2 - ${evento}:`, datos);
        };
        
        modelo.suscribir(observer1);
        modelo.suscribir(observer2, ['cambioEstado']);
        
        modelo.establecerEstado('nombre', 'Juan');
        modelo.establecerEstado('edad', 30);
        
        modelo.desuscribir(observer1);
        modelo.establecerEstado('activo', true);
        
        return { Observable, modelo };
    }
    
    // 📊 PATRÓN: MEMOIZACIÓN AVANZADA
    static memoizacionAvanzada() {
        console.log("📊 Memoización avanzada:");
        
        const cache = new WeakMap();
        const estadisticas = new WeakMap();
        
        function memoizar(fn, opciones = {}) {
            const { 
                maxSize = 100,
                ttl = null, // Time to live en ms
                keyGenerator = (...args) => JSON.stringify(args)
            } = opciones;
            
            return function memoizada(...args) {
                // Usar el objeto function como clave
                if (!cache.has(memoizada)) {
                    cache.set(memoizada, new Map());
                    estadisticas.set(memoizada, {
                        hits: 0,
                        misses: 0,
                        totalCalls: 0
                    });
                }
                
                const funcionCache = cache.get(memoizada);
                const stats = estadisticas.get(memoizada);
                const key = keyGenerator(...args);
                
                stats.totalCalls++;
                
                // Verificar si existe en cache
                if (funcionCache.has(key)) {
                    const entrada = funcionCache.get(key);
                    
                    // Verificar TTL si está configurado
                    if (ttl && Date.now() - entrada.timestamp > ttl) {
                        funcionCache.delete(key);
                        stats.misses++;
                        console.log(`⏰ Cache expirado para: ${key}`);
                    } else {
                        stats.hits++;
                        console.log(`📄 Cache hit para: ${key}`);
                        return entrada.valor;
                    }
                }
                
                // Cache miss - calcular valor
                stats.misses++;
                console.log(`🔄 Cache miss para: ${key}`);
                const resultado = fn.apply(this, args);
                
                // Limpiar cache si está lleno
                if (funcionCache.size >= maxSize) {
                    const primeraKey = funcionCache.keys().next().value;
                    funcionCache.delete(primeraKey);
                    console.log(`🧹 Cache limpiado, removido: ${primeraKey}`);
                }
                
                // Guardar en cache
                funcionCache.set(key, {
                    valor: resultado,
                    timestamp: Date.now()
                });
                
                return resultado;
            };
        }
        
        // Función costosa para demostraciones
        function fibonacci(n) {
            if (n < 2) return n;
            return fibonacci(n - 1) + fibonacci(n - 2);
        }
        
        function buscarDatos(id, categoria) {
            // Simular operación costosa
            const tiempo = Math.random() * 100;
            return {
                id,
                categoria,
                datos: `Datos para ${id} en ${categoria}`,
                procesadoEn: tiempo.toFixed(2) + 'ms'
            };
        }
        
        // Crear versiones memoizadas
        const fibMemo = memoizar(fibonacci);
        const buscarMemo = memoizar(buscarDatos, { 
            maxSize: 5, 
            ttl: 2000 // 2 segundos
        });
        
        // Demostración
        console.log("Fibonacci 10:", fibMemo(10));
        console.log("Fibonacci 10 otra vez:", fibMemo(10)); // Cache hit
        
        console.log("Buscar datos:", buscarMemo(1, "usuarios"));
        console.log("Buscar datos otra vez:", buscarMemo(1, "usuarios")); // Cache hit
        
        // Mostrar estadísticas
        setTimeout(() => {
            const stats = estadisticas.get(buscarMemo);
            console.log("📊 Estadísticas cache:", stats);
        }, 100);
        
        return { memoizar, fibMemo, buscarMemo };
    }
}

// 🚀 Demostraciones WeakMap Avanzados
console.log("🌟 WEAKMAP - PATRONES AVANZADOS");
WeakMapPatronesAvanzados.factoryDatosPrivados();
WeakMapPatronesAvanzados.observerPattern();
WeakMapPatronesAvanzados.memoizacionAvanzada();
```

### 🎯 **Patrones Avanzados con WeakSets**

```javascript
// 🎯 Patrones avanzados con WeakSets
class WeakSetPatronesAvanzados {
    
    // 🔐 PATRÓN: CONTROL DE ACCESO MULTINIVEL
    static controlAccesoMultinivel() {
        console.log("🔐 Control de acceso multinivel:");
        
        const nivelesAcceso = {
            admin: new WeakSet(),
            moderador: new WeakSet(),
            usuario: new WeakSet(),
            invitado: new WeakSet()
        };
        
        const usuariosBloqueados = new WeakSet();
        const sesionesActivas = new WeakSet();
        
        class SistemaAcceso {
            static asignarRol(usuario, rol) {
                // Limpiar roles anteriores
                Object.values(nivelesAcceso).forEach(set => set.delete(usuario));
                
                // Asignar nuevo rol
                if (nivelesAcceso[rol]) {
                    nivelesAcceso[rol].add(usuario);
                    console.log(`✅ ${usuario.nombre} asignado como ${rol}`);
                    return true;
                }
                return false;
            }
            
            static obtenerRol(usuario) {
                for (const [rol, set] of Object.entries(nivelesAcceso)) {
                    if (set.has(usuario)) return rol;
                }
                return null;
            }
            
            static puedeAcceder(usuario, recurso) {
                if (usuariosBloqueados.has(usuario)) {
                    return { acceso: false, razon: "Usuario bloqueado" };
                }
                
                if (!sesionesActivas.has(usuario)) {
                    return { acceso: false, razon: "Sesión no activa" };
                }
                
                const rol = this.obtenerRol(usuario);
                const permisos = {
                    admin: ['dashboard', 'usuarios', 'configuracion', 'reportes'],
                    moderador: ['dashboard', 'usuarios', 'reportes'],
                    usuario: ['dashboard', 'perfil'],
                    invitado: ['dashboard']
                };
                
                if (permisos[rol]?.includes(recurso)) {
                    return { acceso: true, rol };
                }
                
                return { acceso: false, razon: `Rol ${rol} sin permisos` };
            }
            
            static iniciarSesion(usuario) {
                if (!usuariosBloqueados.has(usuario)) {
                    sesionesActivas.add(usuario);
                    console.log(`🔑 Sesión iniciada: ${usuario.nombre}`);
                    return true;
                }
                return false;
            }
            
            static cerrarSesion(usuario) {
                sesionesActivas.delete(usuario);
                console.log(`🚪 Sesión cerrada: ${usuario.nombre}`);
            }
            
            static bloquearUsuario(usuario) {
                usuariosBloqueados.add(usuario);
                sesionesActivas.delete(usuario);
                console.log(`🚫 Usuario bloqueado: ${usuario.nombre}`);
            }
        }
        
        // Demostración
        const admin = { nombre: "Ana", id: 1 };
        const moderador = { nombre: "Carlos", id: 2 };
        const usuario = { nombre: "Elena", id: 3 };
        
        SistemaAcceso.asignarRol(admin, "admin");
        SistemaAcceso.asignarRol(moderador, "moderador");
        SistemaAcceso.asignarRol(usuario, "usuario");
        
        SistemaAcceso.iniciarSesion(admin);
        SistemaAcceso.iniciarSesion(usuario);
        
        console.log("Admin acceso config:", 
            SistemaAcceso.puedeAcceder(admin, "configuracion"));
        console.log("Usuario acceso config:", 
            SistemaAcceso.puedeAcceder(usuario, "configuracion"));
        console.log("Usuario acceso dashboard:", 
            SistemaAcceso.puedeAcceder(usuario, "dashboard"));
        
        return { SistemaAcceso, nivelesAcceso };
    }
    
    // 🔄 PATRÓN: ESTADO DE OBJETOS
    static estadoObjetos() {
        console.log("🔄 Estado de objetos:");
        
        const estados = {
            procesando: new WeakSet(),
            completado: new WeakSet(),
            error: new WeakSet(),
            pendiente: new WeakSet()
        };
        
        const metadatos = new WeakMap();
        
        class GestorEstados {
            static cambiarEstado(objeto, nuevoEstado) {
                // Remover de todos los estados
                Object.values(estados).forEach(set => set.delete(objeto));
                
                // Agregar al nuevo estado
                if (estados[nuevoEstado]) {
                    estados[nuevoEstado].add(objeto);
                    
                    // Actualizar metadatos
                    if (!metadatos.has(objeto)) {
                        metadatos.set(objeto, { historial: [] });
                    }
                    
                    const meta = metadatos.get(objeto);
                    meta.historial.push({
                        estado: nuevoEstado,
                        timestamp: new Date()
                    });
                    meta.estadoActual = nuevoEstado;
                    
                    console.log(`🔄 ${objeto.id}: ${nuevoEstado}`);
                    return true;
                }
                return false;
            }
            
            static obtenerEstado(objeto) {
                for (const [estado, set] of Object.entries(estados)) {
                    if (set.has(objeto)) return estado;
                }
                return 'desconocido';
            }
            
            static obtenerObjetosPorEstado(estado) {
                const objetos = [];
                if (estados[estado]) {
                    // Como WeakSet no es iterable, necesitamos otra forma
                    // En la práctica, mantendrías una referencia externa
                    console.log(`📊 Estado ${estado}: [No iterable directamente]`);
                }
                return objetos;
            }
            
            static esValido(objeto) {
                const estado = this.obtenerEstado(objeto);
                return estado !== 'error' && estado !== 'desconocido';
            }
            
            static puedeTransicionar(objeto, nuevoEstado) {
                const estadoActual = this.obtenerEstado(objeto);
                
                const transicionesValidas = {
                    pendiente: ['procesando', 'error'],
                    procesando: ['completado', 'error'],
                    completado: ['pendiente'], // Re-procesar
                    error: ['pendiente', 'procesando']
                };
                
                return transicionesValidas[estadoActual]?.includes(nuevoEstado) || false;
            }
        }
        
        // Demostración
        const tarea1 = { id: "T001", descripcion: "Procesar datos" };
        const tarea2 = { id: "T002", descripcion: "Generar reporte" };
        const tarea3 = { id: "T003", descripcion: "Enviar email" };
        
        GestorEstados.cambiarEstado(tarea1, "pendiente");
        GestorEstados.cambiarEstado(tarea2, "pendiente");
        GestorEstados.cambiarEstado(tarea3, "pendiente");
        
        console.log("Tarea1 estado:", GestorEstados.obtenerEstado(tarea1));
        console.log("Puede procesando?", 
            GestorEstados.puedeTransicionar(tarea1, "procesando"));
        
        GestorEstados.cambiarEstado(tarea1, "procesando");
        GestorEstados.cambiarEstado(tarea1, "completado");
        
        GestorEstados.cambiarEstado(tarea2, "procesando");
        GestorEstados.cambiarEstado(tarea2, "error");
        
        console.log("Tarea1 válida:", GestorEstados.esValido(tarea1));
        console.log("Tarea2 válida:", GestorEstados.esValido(tarea2));
        
        return { GestorEstados, estados, metadatos };
    }
    
    // ✅ PATRÓN: VALIDACIÓN Y TRACKING
    static validacionTracking() {
        console.log("✅ Validación y tracking:");
        
        const objetosValidados = new WeakSet();
        const objetosEnProceso = new WeakSet();
        const objetosConError = new WeakSet();
        const reglasValidacion = new WeakMap();
        
        class ValidadorAvanzado {
            static definirReglas(objeto, reglas) {
                reglasValidacion.set(objeto, reglas);
                console.log(`📋 Reglas definidas para objeto ${objeto.id || 'sin-id'}`);
            }
            
            static async validar(objeto) {
                if (objetosEnProceso.has(objeto)) {
                    return { valido: false, error: "Ya en proceso de validación" };
                }
                
                if (objetosValidados.has(objeto)) {
                    return { valido: true, mensaje: "Ya validado anteriormente" };
                }
                
                objetosEnProceso.add(objeto);
                objetosConError.delete(objeto);
                
                try {
                    const reglas = reglasValidacion.get(objeto) || [];
                    console.log(`🔍 Validando objeto con ${reglas.length} reglas...`);
                    
                    for (const regla of reglas) {
                        const resultado = await regla.validador(objeto);
                        if (!resultado.valido) {
                            objetosConError.add(objeto);
                            objetosEnProceso.delete(objeto);
                            return {
                                valido: false,
                                error: `Regla '${regla.nombre}': ${resultado.error}`
                            };
                        }
                    }
                    
                    objetosValidados.add(objeto);
                    objetosEnProceso.delete(objeto);
                    console.log(`✅ Objeto validado exitosamente`);
                    
                    return { valido: true, mensaje: "Validación exitosa" };
                    
                } catch (error) {
                    objetosConError.add(objeto);
                    objetosEnProceso.delete(objeto);
                    return { valido: false, error: error.message };
                }
            }
            
            static esValido(objeto) {
                return objetosValidados.has(objeto) && !objetosConError.has(objeto);
            }
            
            static tieneErrores(objeto) {
                return objetosConError.has(objeto);
            }
            
            static estaEnProceso(objeto) {
                return objetosEnProceso.has(objeto);
            }
            
            static limpiarEstado(objeto) {
                objetosValidados.delete(objeto);
                objetosEnProceso.delete(objeto);
                objetosConError.delete(objeto);
                console.log(`🧹 Estado limpiado para objeto`);
            }
        }
        
        // Reglas de validación de ejemplo
        const reglasUsuario = [
            {
                nombre: "email-valido",
                validador: async (obj) => {
                    const emailRegex = /^[^\s@]+@[^\s@]+\.[^\s@]+$/;
                    return {
                        valido: emailRegex.test(obj.email),
                        error: "Email no válido"
                    };
                }
            },
            {
                nombre: "edad-minima",
                validador: async (obj) => {
                    return {
                        valido: obj.edad >= 18,
                        error: "Edad debe ser mayor a 18"
                    };
                }
            }
        ];
        
        // Demostración
        const usuario1 = { id: 1, email: "ana@email.com", edad: 25 };
        const usuario2 = { id: 2, email: "email-invalido", edad: 16 };
        
        ValidadorAvanzado.definirReglas(usuario1, reglasUsuario);
        ValidadorAvanzado.definirReglas(usuario2, reglasUsuario);
        
        // Validaciones asíncronas
        (async () => {
            console.log("Usuario1:", await ValidadorAvanzado.validar(usuario1));
            console.log("Usuario2:", await ValidadorAvanzado.validar(usuario2));
            
            console.log("Usuario1 válido:", ValidadorAvanzado.esValido(usuario1));
            console.log("Usuario2 válido:", ValidadorAvanzado.esValido(usuario2));
            console.log("Usuario2 con errores:", ValidadorAvanzado.tieneErrores(usuario2));
        })();
        
        return { ValidadorAvanzado, reglasUsuario };
    }
}

// 🚀 Demostraciones WeakSet Avanzados
console.log("🎯 WEAKSET - PATRONES AVANZADOS");
WeakSetPatronesAvanzados.controlAccesoMultinivel();
WeakSetPatronesAvanzados.estadoObjetos();
WeakSetPatronesAvanzados.validacionTracking();
```

### 🌐 **Casos de Uso del Mundo Real**

```javascript
// 🌐 Casos de uso reales y prácticos
class CasosUsoReales {
    
    // 📱 SISTEMA DE NOTIFICACIONES
    static sistemaNotificaciones() {
        console.log("📱 Sistema de notificaciones:");
        
        const suscriptores = new WeakMap();
        const notificacionesLeidas = new WeakSet();
        const notificacionesSilenciadas = new WeakSet();
        
        class SistemaNotificaciones {
            constructor() {
                this.notificaciones = [];
                this.contadorId = 1;
            }
            
            suscribir(usuario, tipos = ['todas']) {
                if (!suscriptores.has(usuario)) {
                    suscriptores.set(usuario, {
                        tipos: new Set(tipos),
                        preferencias: {
                            email: true,
                            push: true,
                            sms: false
                        }
                    });
                }
                console.log(`🔔 ${usuario.nombre} suscrito a: ${tipos.join(', ')}`);
            }
            
            enviarNotificacion(tipo, mensaje, datos = {}) {
                const notificacion = {
                    id: this.contadorId++,
                    tipo,
                    mensaje,
                    datos,
                    timestamp: new Date()
                };
                
                this.notificaciones.push(notificacion);
                
                // Enviar a suscriptores
                this._notificarSuscriptores(notificacion);
                
                return notificacion;
            }
            
            _notificarSuscriptores(notificacion) {
                console.log(`📤 Enviando: ${notificacion.mensaje}`);
                // En una implementación real, aquí iterarías sobre usuarios
                // Como WeakMap no es iterable, mantendrías referencias por separado
            }
            
            marcarLeida(usuario, notificacion) {
                notificacionesLeidas.add(notificacion);
                console.log(`👁️ ${usuario.nombre} leyó: ${notificacion.mensaje}`);
            }
            
            silenciar(usuario, notificacion) {
                notificacionesSilenciadas.add(notificacion);
                console.log(`🔇 ${usuario.nombre} silenció notificación`);
            }
            
            obtenerNotificacionesUsuario(usuario) {
                const config = suscriptores.get(usuario);
                if (!config) return [];
                
                return this.notificaciones.filter(notif => {
                    // Verificar si está suscrito al tipo
                    if (!config.tipos.has('todas') && !config.tipos.has(notif.tipo)) {
                        return false;
                    }
                    
                    // Excluir silenciadas
                    if (notificacionesSilenciadas.has(notif)) {
                        return false;
                    }
                    
                    return true;
                }).map(notif => ({
                    ...notif,
                    leida: notificacionesLeidas.has(notif)
                }));
            }
        }
        
        // Demostración
        const sistema = new SistemaNotificaciones();
        const usuario1 = { nombre: "Ana", id: 1 };
        const usuario2 = { nombre: "Carlos", id: 2 };
        
        sistema.suscribir(usuario1, ['sistema', 'mensajes']);
        sistema.suscribir(usuario2, ['todas']);
        
        const notif1 = sistema.enviarNotificacion('sistema', 'Sistema actualizado');
        const notif2 = sistema.enviarNotificacion('mensajes', 'Nuevo mensaje recibido');
        
        sistema.marcarLeida(usuario1, notif1);
        sistema.silenciar(usuario2, notif2);
        
        console.log("Notificaciones usuario1:", 
            sistema.obtenerNotificacionesUsuario(usuario1));
        
        return { sistema, SistemaNotificaciones };
    }
    
    // 🛡️ SISTEMA DE PERMISOS EMPRESARIALES
    static sistemaPermisosEmpresas() {
        console.log("🛡️ Sistema permisos empresariales:");
        
        const empleadosActivos = new WeakSet();
        const sesionesSeguras = new WeakSet();
        const recursosProtegidos = new WeakMap();
        const auditoria = new WeakMap();
        
        class SistemaPermisosEmpresa {
            static activarEmpleado(empleado) {
                empleadosActivos.add(empleado);
                
                if (!auditoria.has(empleado)) {
                    auditoria.set(empleado, []);
                }
                
                auditoria.get(empleado).push({
                    accion: 'empleado_activado',
                    timestamp: new Date(),
                    ip: '192.168.1.100' // En real, obtener IP actual
                });
                
                console.log(`✅ Empleado activado: ${empleado.nombre}`);
            }
            
            static iniciarSesionSegura(empleado, requiere2FA = true) {
                if (!empleadosActivos.has(empleado)) {
                    return { exito: false, error: "Empleado no activo" };
                }
                
                if (requiere2FA && !empleado.verificado2FA) {
                    return { exito: false, error: "Requiere verificación 2FA" };
                }
                
                sesionesSeguras.add(empleado);
                auditoria.get(empleado).push({
                    accion: 'sesion_iniciada',
                    timestamp: new Date(),
                    metodo: requiere2FA ? '2FA' : 'normal'
                });
                
                console.log(`🔐 Sesión segura iniciada: ${empleado.nombre}`);
                return { exito: true };
            }
            
            static configurarRecurso(recurso, config) {
                recursosProtegidos.set(recurso, {
                    nivelSeguridad: config.nivelSeguridad || 'medio',
                    rolesPermitidos: new Set(config.rolesPermitidos || []),
                    requiereSesionSegura: config.requiereSesionSegura || false,
                    auditCompleta: config.auditCompleta || false
                });
                
                console.log(`⚙️ Recurso configurado: ${recurso.nombre}`);
            }
            
            static verificarAcceso(empleado, recurso) {
                // Verificar empleado activo
                if (!empleadosActivos.has(empleado)) {
                    return { acceso: false, razon: "Empleado no activo" };
                }
                
                const configRecurso = recursosProtegidos.get(recurso);
                if (!configRecurso) {
                    return { acceso: false, razon: "Recurso no configurado" };
                }
                
                // Verificar sesión segura si es requerida
                if (configRecurso.requiereSesionSegura && !sesionesSeguras.has(empleado)) {
                    return { acceso: false, razon: "Requiere sesión segura" };
                }
                
                // Verificar rol
                if (!configRecurso.rolesPermitidos.has(empleado.rol)) {
                    return { acceso: false, razon: `Rol ${empleado.rol} no permitido` };
                }
                
                // Auditoría
                auditoria.get(empleado).push({
                    accion: 'acceso_recurso',
                    recurso: recurso.nombre,
                    timestamp: new Date(),
                    resultado: 'permitido'
                });
                
                return { 
                    acceso: true, 
                    nivelSeguridad: configRecurso.nivelSeguridad 
                };
            }
            
            static obtenerAuditoria(empleado) {
                return auditoria.get(empleado) || [];
            }
        }
        
        // Demostración
        const empleado1 = { 
            nombre: "Elena", 
            id: "E001", 
            rol: "admin",
            verificado2FA: true 
        };
        
        const empleado2 = { 
            nombre: "Pedro", 
            id: "E002", 
            rol: "usuario",
            verificado2FA: false 
        };
        
        const recursoSensible = { 
            nombre: "Base de Datos Financiera",
            id: "BD001" 
        };
        
        // Configurar sistema
        SistemaPermisosEmpresa.activarEmpleado(empleado1);
        SistemaPermisosEmpresa.activarEmpleado(empleado2);
        
        SistemaPermisosEmpresa.configurarRecurso(recursoSensible, {
            nivelSeguridad: 'alto',
            rolesPermitidos: ['admin', 'finanzas'],
            requiereSesionSegura: true,
            auditCompleta: true
        });
        
        SistemaPermisosEmpresa.iniciarSesionSegura(empleado1);
        
        console.log("Acceso empleado1:", 
            SistemaPermisosEmpresa.verificarAcceso(empleado1, recursoSensible));
        console.log("Acceso empleado2:", 
            SistemaPermisosEmpresa.verificarAcceso(empleado2, recursoSensible));
        
        console.log("Auditoría empleado1:", 
            SistemaPermisosEmpresa.obtenerAuditoria(empleado1));
        
        return { SistemaPermisosEmpresa, empleado1, recursoSensible };
    }
}

// 🚀 Demostraciones Casos Reales
console.log("🌐 CASOS DE USO DEL MUNDO REAL");
CasosUsoReales.sistemaNotificaciones();
CasosUsoReales.sistemaPermisosEmpresas();
```

**✅ CAPÍTULO 9 COMPLETADO**

### 🎯 **Resumen Completo del Capítulo 9:**

#### **PARTE 1 - Fundamentos:**
1. **🗺️ Maps Avanzados** - Operaciones, claves flexibles, iteración, comparación con Object
2. **🎯 Sets Avanzados** - Operaciones básicas, matemáticas de conjuntos, casos prácticos

#### **PARTE 2 - Estructuras Débiles:**
3. **💾 WeakMaps Básicos** - Conceptos, datos privados, cache automático
4. **🔗 WeakSets Básicos** - Tracking, control de acceso, comparación

#### **PARTE 3 - Patrones Avanzados:**
5. **🌟 WeakMap Avanzado** - Factory privado, Observer, memoización
6. **🎯 WeakSet Avanzado** - Control multinivel, estados, validación
7. **🌐 Casos Reales** - Notificaciones, permisos empresariales

### 💡 **Cuándo usar cada estructura:**

- **Map**: Claves de cualquier tipo, iteración frecuente, tamaño conocido
- **Set**: Valores únicos, operaciones matemáticas, validación duplicados  
- **WeakMap**: Metadatos de objetos, datos privados, cache temporal
- **WeakSet**: Estados de objetos, tracking, control de acceso

---

## 🔄 **PRÓXIMO CAPÍTULO**

---

## 10. 📈 **Algoritmos y Rendimiento - PARTE 1**

### 🌟 **Introducción a la Análisis de Algoritmos**

El rendimiento no es solo velocidad: es eficiencia, escalabilidad y uso inteligente de recursos. Comprender cómo analizar y optimizar algoritmos es fundamental para crear aplicaciones que funcionen bien tanto con 10 como con 10 millones de elementos.

```javascript
// 📈 La importancia del análisis de algoritmos
console.log("🚀 ¿Por qué importa el rendimiento?");

// Ejemplo: Diferencias dramáticas en rendimiento
const ejemploRendimiento = {
    // ❌ Algoritmo ineficiente - O(n²)
    busquedaIneficiente: (array, objetivo) => {
        let comparaciones = 0;
        for (let i = 0; i < array.length; i++) {
            for (let j = 0; j < array.length; j++) {
                comparaciones++;
                if (array[j] === objetivo) {
                    return { encontrado: true, comparaciones };
                }
            }
        }
        return { encontrado: false, comparaciones };
    },
    
    // ✅ Algoritmo eficiente - O(n)
    busquedaEficiente: (array, objetivo) => {
        let comparaciones = 0;
        for (let i = 0; i < array.length; i++) {
            comparaciones++;
            if (array[i] === objetivo) {
                return { encontrado: true, comparaciones };
            }
        }
        return { encontrado: false, comparaciones };
    }
};

// Comparación con datos reales
const datos = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10];
const objetivo = 8;

console.log("Ineficiente:", ejemploRendimiento.busquedaIneficiente(datos, objetivo));
console.log("Eficiente:", ejemploRendimiento.busquedaEficiente(datos, objetivo));
```

### 📊 **Notación Big O - Análisis de Complejidad**

```javascript
// 📊 Big O Notation - Midiendo la eficiencia
class AnalisisBigO {
    
    // 🎯 COMPLEJIDADES BÁSICAS
    static complejidadesBasicas() {
        console.log("📊 Complejidades de tiempo más comunes:");
        
        // O(1) - Constante
        const constanteO1 = (array) => {
            console.time("⚡ O(1)");
            const resultado = array[0]; // Siempre 1 operación
            console.timeEnd("⚡ O(1)");
            return resultado;
        };
        
        // O(log n) - Logarítmica
        const logaritmicaOLogN = (array, objetivo) => {
            console.time("📈 O(log n)");
            let inicio = 0;
            let fin = array.length - 1;
            let operaciones = 0;
            
            while (inicio <= fin) {
                operaciones++;
                const medio = Math.floor((inicio + fin) / 2);
                
                if (array[medio] === objetivo) {
                    console.timeEnd("📈 O(log n)");
                    return { encontrado: true, operaciones, indice: medio };
                }
                
                if (array[medio] < objetivo) {
                    inicio = medio + 1;
                } else {
                    fin = medio - 1;
                }
            }
            
            console.timeEnd("📈 O(log n)");
            return { encontrado: false, operaciones };
        };
        
        // O(n) - Lineal
        const linealOn = (array, objetivo) => {
            console.time("📏 O(n)");
            let operaciones = 0;
            
            for (let i = 0; i < array.length; i++) {
                operaciones++;
                if (array[i] === objetivo) {
                    console.timeEnd("📏 O(n)");
                    return { encontrado: true, operaciones, indice: i };
                }
            }
            
            console.timeEnd("📏 O(n)");
            return { encontrado: false, operaciones };
        };
        
        // O(n log n) - Log-lineal
        const logLinealOnLogN = (array) => {
            console.time("🔄 O(n log n)");
            let operaciones = 0;
            
            // Merge Sort simplificado para demostración
            const mergeSort = (arr) => {
                if (arr.length <= 1) return arr;
                
                operaciones++;
                const medio = Math.floor(arr.length / 2);
                const izquierda = mergeSort(arr.slice(0, medio));
                const derecha = mergeSort(arr.slice(medio));
                
                return merge(izquierda, derecha);
            };
            
            const merge = (izq, der) => {
                const resultado = [];
                let i = 0, j = 0;
                
                while (i < izq.length && j < der.length) {
                    operaciones++;
                    if (izq[i] <= der[i]) {
                        resultado.push(izq[i]);
                        i++;
                    } else {
                        resultado.push(der[j]);
                        j++;
                    }
                }
                
                return resultado.concat(izq.slice(i)).concat(der.slice(j));
            };
            
            const resultado = mergeSort([...array]);
            console.timeEnd("🔄 O(n log n)");
            return { resultado, operaciones };
        };
        
        // O(n²) - Cuadrática
        const cuadraticaOn2 = (array) => {
            console.time("⚠️ O(n²)");
            let operaciones = 0;
            const pares = [];
            
            for (let i = 0; i < array.length; i++) {
                for (let j = i + 1; j < array.length; j++) {
                    operaciones++;
                    pares.push([array[i], array[j]]);
                }
            }
            
            console.timeEnd("⚠️ O(n²)");
            return { pares: pares.length, operaciones };
        };
        
        // O(2^n) - Exponencial
        const exponencialO2n = (n) => {
            console.time("💥 O(2^n)");
            let operaciones = 0;
            
            const fibonacci = (num) => {
                operaciones++;
                if (num <= 1) return num;
                return fibonacci(num - 1) + fibonacci(num - 2);
            };
            
            const resultado = fibonacci(n);
            console.timeEnd("💥 O(2^n)");
            return { resultado, operaciones };
        };
        
        // Datos de prueba
        const datosTest = Array.from({length: 1000}, (_, i) => i + 1);
        const objetivo = 750;
        
        console.log("🧪 Pruebas con 1000 elementos:");
        
        console.log("⚡ O(1) - Acceso directo:");
        console.log(constanteO1(datosTest));
        
        console.log("\n📈 O(log n) - Búsqueda binaria:");
        console.log(logaritmicaOLogN(datosTest, objetivo));
        
        console.log("\n📏 O(n) - Búsqueda lineal:");
        console.log(linealOn(datosTest, objetivo));
        
        console.log("\n⚠️ O(n²) - Pares de elementos:");
        const datosChicos = datosTest.slice(0, 50); // Menos datos para O(n²)
        console.log(cuadraticaOn2(datosChicos));
        
        console.log("\n💥 O(2^n) - Fibonacci recursivo:");
        console.log("Fibonacci(20):", exponencialO2n(20));
        
        // Tabla comparativa
        const comparacionComplejidades = {
            "O(1)": "Constante - Siempre mismo tiempo",
            "O(log n)": "Logarítmica - Crece muy lentamente",
            "O(n)": "Lineal - Proporcional al tamaño",
            "O(n log n)": "Log-lineal - Algoritmos eficientes",
            "O(n²)": "Cuadrática - Crece rápidamente",
            "O(2^n)": "Exponencial - ¡Evitar a toda costa!"
        };
        
        console.log("\n📋 Comparación de complejidades:");
        console.table(comparacionComplejidades);
        
        return {
            constanteO1,
            logaritmicaOLogN,
            linealOn,
            logLinealOnLogN,
            cuadraticaOn2,
            exponencialO2n
        };
    }
    
    // 🎯 ANÁLISIS PRÁCTICO DE CÓDIGO
    static analisisPractico() {
        console.log("🎯 Análisis práctico de código:");
        
        // Función para medir tiempo y operaciones
        const medirRendimiento = (func, nombre, ...args) => {
            const inicio = performance.now();
            const resultado = func(...args);
            const fin = performance.now();
            
            console.log(`${nombre}: ${(fin - inicio).toFixed(2)}ms`);
            return resultado;
        };
        
        // Ejemplo 1: Loops anidados - ¿Siempre O(n²)?
        const ejemploLoopsAnidados = {
            // ❌ Verdadero O(n²) - todos con todos
            todoConTodos: (array) => {
                let operaciones = 0;
                for (let i = 0; i < array.length; i++) {
                    for (let j = 0; j < array.length; j++) {
                        operaciones++;
                        // Operación cualquiera
                    }
                }
                return operaciones;
            },
            
            // ✅ O(n²/2) - sin repeticiones
            sinRepeticiones: (array) => {
                let operaciones = 0;
                for (let i = 0; i < array.length; i++) {
                    for (let j = i + 1; j < array.length; j++) {
                        operaciones++;
                        // Operación cualquiera
                    }
                }
                return operaciones;
            },
            
            // ✅ O(n) - loop interno constante
            loopInternoConstante: (array) => {
                let operaciones = 0;
                for (let i = 0; i < array.length; i++) {
                    for (let j = 0; j < 10; j++) { // Constante
                        operaciones++;
                        // Operación cualquiera
                    }
                }
                return operaciones;
            }
        };
        
        // Ejemplo 2: Algoritmos de búsqueda comunes
        const algoritmosBusqueda = {
            // O(n) - Búsqueda lineal
            busquedaLineal: (array, objetivo) => {
                for (let i = 0; i < array.length; i++) {
                    if (array[i] === objetivo) {
                        return { encontrado: true, indice: i, comparaciones: i + 1 };
                    }
                }
                return { encontrado: false, comparaciones: array.length };
            },
            
            // O(log n) - Búsqueda binaria (requiere array ordenado)
            busquedaBinaria: (array, objetivo) => {
                let inicio = 0;
                let fin = array.length - 1;
                let comparaciones = 0;
                
                while (inicio <= fin) {
                    comparaciones++;
                    const medio = Math.floor((inicio + fin) / 2);
                    
                    if (array[medio] === objetivo) {
                        return { encontrado: true, indice: medio, comparaciones };
                    }
                    
                    if (array[medio] < objetivo) {
                        inicio = medio + 1;
                    } else {
                        fin = medio - 1;
                    }
                }
                
                return { encontrado: false, comparaciones };
            },
            
            // O(1) - Búsqueda con hash (usando Map)
            busquedaHash: (array, objetivo) => {
                // Preparar hash una vez
                const mapa = new Map();
                array.forEach((valor, indice) => {
                    mapa.set(valor, indice);
                });
                
                // Búsqueda O(1)
                if (mapa.has(objetivo)) {
                    return { encontrado: true, indice: mapa.get(objetivo), comparaciones: 1 };
                }
                return { encontrado: false, comparaciones: 1 };
            }
        };
        
        // Pruebas de rendimiento
        const datosTest = Array.from({length: 10000}, (_, i) => i);
        const objetivo = 7500;
        
        console.log("🔍 Comparación algoritmos de búsqueda:");
        console.log("Datos: 10,000 elementos, buscando: 7500");
        
        const resultadoLineal = medirRendimiento(
            algoritmosBusqueda.busquedaLineal, 
            "📏 Búsqueda Lineal O(n)", 
            datosTest, objetivo
        );
        
        const resultadoBinaria = medirRendimiento(
            algoritmosBusqueda.busquedaBinaria, 
            "📈 Búsqueda Binaria O(log n)", 
            datosTest, objetivo
        );
        
        const resultadoHash = medirRendimiento(
            algoritmosBusqueda.busquedaHash, 
            "⚡ Búsqueda Hash O(1)", 
            datosTest, objetivo
        );
        
        console.log("\n📊 Resultados:");
        console.log("Lineal:", resultadoLineal);
        console.log("Binaria:", resultadoBinaria);
        console.log("Hash:", resultadoHash);
        
        // Ejemplo 3: Identificar cuellos de botella
        const identificarCuellosBottle = {
            // ❌ Problema: Operación costosa en loop
            problematicoO1: (array) => {
                let resultado = [];
                for (let i = 0; i < array.length; i++) {
                    // ❌ JSON.stringify en cada iteración
                    const copia = JSON.parse(JSON.stringify(array[i]));
                    resultado.push(copia);
                }
                return resultado;
            },
            
            // ✅ Optimizado: Operación eficiente
            optimizadoO2: (array) => {
                let resultado = [];
                for (let i = 0; i < array.length; i++) {
                    // ✅ Copia eficiente con spread
                    const copia = { ...array[i] };
                    resultado.push(copia);
                }
                return resultado;
            }
        };
        
        // Prueba con objetos
        const objetosTest = Array.from({length: 1000}, (_, i) => ({
            id: i,
            nombre: `Usuario${i}`,
            datos: { activo: true, score: i * 10 }
        }));
        
        console.log("\n🚨 Identificando cuellos de botella:");
        medirRendimiento(
            identificarCuellosBottle.problematicoO1,
            "❌ JSON.parse/stringify",
            objetosTest.slice(0, 100) // Solo 100 para que no tarde mucho
        );
        
        medirRendimiento(
            identificarCuellosBottle.optimizadoO2,
            "✅ Spread operator",
            objetosTest.slice(0, 100)
        );
        
        return {
            ejemploLoopsAnidados,
            algoritmosBusqueda,
            identificarCuellosBottle
        };
    }
    
    // 🎯 COMPLEJIDAD ESPACIAL
    static complejidadEspacial() {
        console.log("💾 Análisis de complejidad espacial:");
        
        const ejemplosEspacio = {
            // O(1) - Espacio constante
            espacioConstante: (array) => {
                let suma = 0; // Solo una variable
                let maximo = array[0]; // Una variable más
                
                for (let i = 0; i < array.length; i++) {
                    suma += array[i];
                    if (array[i] > maximo) {
                        maximo = array[i];
                    }
                }
                
                return { suma, maximo };
            },
            
            // O(n) - Espacio lineal
            espacioLineal: (array) => {
                // Crear nueva array del mismo tamaño
                const duplicados = [];
                const cuadrados = [];
                
                for (let i = 0; i < array.length; i++) {
                    duplicados.push(array[i] * 2);
                    cuadrados.push(array[i] ** 2);
                }
                
                return { duplicados, cuadrados };
            },
            
            // O(n²) - Espacio cuadrático
            espacioCuadratico: (array) => {
                // Matriz n x n
                const matriz = [];
                
                for (let i = 0; i < array.length; i++) {
                    matriz[i] = [];
                    for (let j = 0; j < array.length; j++) {
                        matriz[i][j] = array[i] + array[j];
                    }
                }
                
                return matriz;
            },
            
            // Ejemplo práctico: Memoización
            fibonacciConMemoria: (n, memo = {}) => {
                if (n in memo) return memo[n];
                if (n <= 2) return 1;
                
                memo[n] = this.fibonacciConMemoria(n - 1, memo) + 
                         this.fibonacciConMemoria(n - 2, memo);
                
                return memo[n];
            }
        };
        
        // Medición de uso de memoria (aproximada)
        const medirMemoria = (func, nombre, ...args) => {
            const antesMemoria = performance.memory?.usedJSHeapSize || 0;
            const resultado = func(...args);
            const despuesMemoria = performance.memory?.usedJSHeapSize || 0;
            
            if (performance.memory) {
                console.log(`${nombre}: ~${(despuesMemoria - antesMemoria)} bytes`);
            } else {
                console.log(`${nombre}: Memoria no disponible en este entorno`);
            }
            
            return resultado;
        };
        
        const datosTest = Array.from({length: 100}, (_, i) => i + 1);
        
        console.log("💾 Comparación uso de memoria:");
        
        medirMemoria(
            ejemplosEspacio.espacioConstante,
            "⚡ O(1) Espacio constante",
            datosTest
        );
        
        medirMemoria(
            ejemplosEspacio.espacioLineal,
            "📏 O(n) Espacio lineal",
            datosTest
        );
        
        medirMemoria(
            ejemplosEspacio.espacioCuadratico,
            "⚠️ O(n²) Espacio cuadrático",
            datosTest.slice(0, 10) // Solo 10 elementos para O(n²)
        );
        
        // Trade-offs tiempo vs espacio
        console.log("\n⚖️ Trade-offs tiempo vs espacio:");
        
        console.log("🐌 Fibonacci sin memoria - O(2^n) tiempo, O(1) espacio:");
        console.time("Sin memoria");
        const fibSinMemoria = (n) => n <= 2 ? 1 : fibSinMemoria(n-1) + fibSinMemoria(n-2);
        fibSinMemoria(30);
        console.timeEnd("Sin memoria");
        
        console.log("⚡ Fibonacci con memoria - O(n) tiempo, O(n) espacio:");
        console.time("Con memoria");
        ejemplosEspacio.fibonacciConMemoria(30);
        console.timeEnd("Con memoria");
        
        return ejemplosEspacio;
    }
}

// 🚀 Demostraciones Big O
console.log("📊 ANÁLISIS BIG O");
AnalisisBigO.complejidadesBasicas();
AnalisisBigO.analisisPractico();
AnalisisBigO.complejidadEspacial();
```

### 🔍 **Algoritmos de Búsqueda Avanzados**

```javascript
// 🔍 Algoritmos de búsqueda especializados
class AlgoritmosBusquedaAvanzados {
    
    // 🎯 BÚSQUEDA LINEAL OPTIMIZADA
    static busquedaLinealOptimizada() {
        console.log("🔍 Búsqueda lineal con optimizaciones:");
        
        const busquedaOptimizada = {
            // Básica - O(n)
            basica: (array, objetivo) => {
                let comparaciones = 0;
                for (let i = 0; i < array.length; i++) {
                    comparaciones++;
                    if (array[i] === objetivo) {
                        return { encontrado: true, indice: i, comparaciones };
                    }
                }
                return { encontrado: false, comparaciones };
            },
            
            // Con centinela - menos comparaciones por iteración
            conCentinela: (array, objetivo) => {
                let comparaciones = 0;
                const ultimo = array[array.length - 1];
                array[array.length - 1] = objetivo; // Centinela
                
                let i = 0;
                while (array[i] !== objetivo) {
                    comparaciones++;
                    i++;
                }
                
                array[array.length - 1] = ultimo; // Restaurar
                
                if (i < array.length - 1 || ultimo === objetivo) {
                    return { encontrado: true, indice: i, comparaciones };
                }
                
                return { encontrado: false, comparaciones };
            },
            
            // Búsqueda desde ambos extremos
            bidireccional: (array, objetivo) => {
                let comparaciones = 0;
                let inicio = 0;
                let fin = array.length - 1;
                
                while (inicio <= fin) {
                    comparaciones += 2;
                    
                    if (array[inicio] === objetivo) {
                        return { encontrado: true, indice: inicio, comparaciones };
                    }
                    if (array[fin] === objetivo) {
                        return { encontrado: true, indice: fin, comparaciones };
                    }
                    
                    inicio++;
                    fin--;
                }
                
                return { encontrado: false, comparaciones };
            },
            
            // Con salto adaptativo
            saltoAdaptativo: (array, objetivo) => {
                let comparaciones = 0;
                const n = array.length;
                let salto = Math.floor(Math.sqrt(n));
                let anterior = 0;
                
                // Encontrar el bloque donde podría estar
                while (array[Math.min(salto, n) - 1] < objetivo) {
                    comparaciones++;
                    anterior = salto;
                    salto += Math.floor(Math.sqrt(n));
                    if (anterior >= n) {
                        return { encontrado: false, comparaciones };
                    }
                }
                
                // Búsqueda lineal en el bloque
                while (array[anterior] < objetivo) {
                    comparaciones++;
                    anterior++;
                    if (anterior === Math.min(salto, n)) {
                        return { encontrado: false, comparaciones };
                    }
                }
                
                if (array[anterior] === objetivo) {
                    comparaciones++;
                    return { encontrado: true, indice: anterior, comparaciones };
                }
                
                return { encontrado: false, comparaciones };
            }
        };
        
        // Pruebas de rendimiento
        const datosTest = Array.from({length: 10000}, (_, i) => i * 2);
        const objetivo = 15000;
        
        console.log("🧪 Comparación búsquedas lineales:");
        console.log("Datos: 10,000 elementos ordenados");
        console.log("Objetivo:", objetivo);
        
        const resultados = {};
        
        console.time("Básica");
        resultados.basica = busquedaOptimizada.basica(datosTest, objetivo);
        console.timeEnd("Básica");
        
        console.time("Con centinela");
        resultados.centinela = busquedaOptimizada.conCentinela([...datosTest], objetivo);
        console.timeEnd("Con centinela");
        
        console.time("Bidireccional");
        resultados.bidireccional = busquedaOptimizada.bidireccional(datosTest, objetivo);
        console.timeEnd("Bidireccional");
        
        console.time("Salto adaptativo");
        resultados.saltoAdaptativo = busquedaOptimizada.saltoAdaptativo(datosTest, objetivo);
        console.timeEnd("Salto adaptativo");
        
        console.log("\n📊 Comparaciones realizadas:");
        Object.entries(resultados).forEach(([tipo, resultado]) => {
            console.log(`${tipo}: ${resultado.comparaciones} comparaciones`);
        });
        
        return { busquedaOptimizada, resultados };
    }
    
    // 📈 BÚSQUEDA BINARIA Y VARIANTES
    static busquedaBinariaVariantes() {
        console.log("📈 Búsqueda binaria y sus variantes:");
        
        const busquedaBinaria = {
            // Básica - encontrar elemento
            basica: (array, objetivo) => {
                let inicio = 0;
                let fin = array.length - 1;
                let iteraciones = 0;
                
                while (inicio <= fin) {
                    iteraciones++;
                    const medio = Math.floor((inicio + fin) / 2);
                    
                    if (array[medio] === objetivo) {
                        return { encontrado: true, indice: medio, iteraciones };
                    }
                    
                    if (array[medio] < objetivo) {
                        inicio = medio + 1;
                    } else {
                        fin = medio - 1;
                    }
                }
                
                return { encontrado: false, iteraciones, puntoInsercion: inicio };
            },
            
            // Encontrar primera ocurrencia
            primeraOcurrencia: (array, objetivo) => {
                let inicio = 0;
                let fin = array.length - 1;
                let resultado = -1;
                let iteraciones = 0;
                
                while (inicio <= fin) {
                    iteraciones++;
                    const medio = Math.floor((inicio + fin) / 2);
                    
                    if (array[medio] === objetivo) {
                        resultado = medio;
                        fin = medio - 1; // Continuar buscando a la izquierda
                    } else if (array[medio] < objetivo) {
                        inicio = medio + 1;
                    } else {
                        fin = medio - 1;
                    }
                }
                
                return { 
                    encontrado: resultado !== -1, 
                    indice: resultado, 
                    iteraciones 
                };
            },
            
            // Encontrar última ocurrencia
            ultimaOcurrencia: (array, objetivo) => {
                let inicio = 0;
                let fin = array.length - 1;
                let resultado = -1;
                let iteraciones = 0;
                
                while (inicio <= fin) {
                    iteraciones++;
                    const medio = Math.floor((inicio + fin) / 2);
                    
                    if (array[medio] === objetivo) {
                        resultado = medio;
                        inicio = medio + 1; // Continuar buscando a la derecha
                    } else if (array[medio] < objetivo) {
                        inicio = medio + 1;
                    } else {
                        fin = medio - 1;
                    }
                }
                
                return { 
                    encontrado: resultado !== -1, 
                    indice: resultado, 
                    iteraciones 
                };
            },
            
            // Búsqueda por rango
            busquedaRango: (array, inicio, fin) => {
                const primera = busquedaBinaria.primeraOcurrencia(array, inicio);
                const ultima = busquedaBinaria.ultimaOcurrencia(array, fin);
                
                if (primera.encontrado && ultima.encontrado) {
                    const elementos = array.slice(primera.indice, ultima.indice + 1);
                    return {
                        encontrado: true,
                        indiceInicio: primera.indice,
                        indiceFin: ultima.indice,
                        elementos: elementos,
                        cantidad: elementos.length
                    };
                }
                
                return { encontrado: false };
            },
            
            // Búsqueda exponencial (para arrays no acotados)
            busquedaExponencial: (array, objetivo) => {
                let iteraciones = 0;
                
                // Encontrar rango donde podría estar el elemento
                if (array[0] === objetivo) {
                    return { encontrado: true, indice: 0, iteraciones: 1 };
                }
                
                let i = 1;
                while (i < array.length && array[i] <= objetivo) {
                    iteraciones++;
                    i *= 2;
                }
                
                // Búsqueda binaria en el rango encontrado
                const resultado = busquedaBinaria.basica(
                    array.slice(i / 2, Math.min(i, array.length)),
                    objetivo
                );
                
                if (resultado.encontrado) {
                    resultado.indice += i / 2;
                }
                
                resultado.iteraciones += iteraciones;
                return resultado;
            }
        };
        
        // Datos de prueba con duplicados
        const datosConDuplicados = [1, 2, 2, 2, 3, 4, 4, 5, 6, 7, 8, 8, 8, 9, 10];
        const datosGrandes = Array.from({length: 10000}, (_, i) => Math.floor(i / 10));
        
        console.log("🧪 Pruebas con búsqueda binaria:");
        console.log("Datos con duplicados:", datosConDuplicados);
        
        // Prueba básica
        console.log("\n📈 Búsqueda básica del 8:");
        console.log(busquedaBinaria.basica(datosConDuplicados, 8));
        
        // Prueba primera y última ocurrencia
        console.log("\n🎯 Primera ocurrencia del 8:");
        console.log(busquedaBinaria.primeraOcurrencia(datosConDuplicados, 8));
        
        console.log("🎯 Última ocurrencia del 8:");
        console.log(busquedaBinaria.ultimaOcurrencia(datosConDuplicados, 8));
        
        // Prueba búsqueda por rango
        console.log("\n📊 Búsqueda por rango (2 a 4):");
        console.log(busquedaBinaria.busquedaRango(datosConDuplicados, 2, 4));
        
        // Comparación de rendimiento
        console.log("\n⚡ Comparación rendimiento (10,000 elementos):");
        
        console.time("Búsqueda binaria");
        const resultadoBinaria = busquedaBinaria.basica(datosGrandes, 5000);
        console.timeEnd("Búsqueda binaria");
        
        console.time("Búsqueda exponencial");
        const resultadoExponencial = busquedaBinaria.busquedaExponencial(datosGrandes, 5000);
        console.timeEnd("Búsqueda exponencial");
        
        console.log("Binaria:", resultadoBinaria);
        console.log("Exponencial:", resultadoExponencial);
        
        return { busquedaBinaria, datosConDuplicados };
    }
    
    // 🔀 BÚSQUEDAS ESPECIALIZADAS
    static busquedasEspecializadas() {
        console.log("🔀 Algoritmos de búsqueda especializados:");
        
        const busquedasEspeciales = {
            // Búsqueda interpolada (para datos uniformemente distribuidos)
            busquedaInterpolada: (array, objetivo) => {
                let inicio = 0;
                let fin = array.length - 1;
                let iteraciones = 0;
                
                while (inicio <= fin && objetivo >= array[inicio] && objetivo <= array[fin]) {
                    iteraciones++;
                    
                    if (inicio === fin) {
                        if (array[inicio] === objetivo) {
                            return { encontrado: true, indice: inicio, iteraciones };
                        }
                        return { encontrado: false, iteraciones };
                    }
                    
                    // Estimación de posición por interpolación
                    const pos = inicio + Math.floor(
                        ((objetivo - array[inicio]) / (array[fin] - array[inicio])) * (fin - inicio)
                    );
                    
                    if (array[pos] === objetivo) {
                        return { encontrado: true, indice: pos, iteraciones };
                    }
                    
                    if (array[pos] < objetivo) {
                        inicio = pos + 1;
                    } else {
                        fin = pos - 1;
                    }
                }
                
                return { encontrado: false, iteraciones };
            },
            
            // Búsqueda ternaria
            busquedaTernaria: (array, objetivo) => {
                let inicio = 0;
                let fin = array.length - 1;
                let iteraciones = 0;
                
                while (inicio <= fin) {
                    iteraciones++;
                    
                    const mid1 = inicio + Math.floor((fin - inicio) / 3);
                    const mid2 = fin - Math.floor((fin - inicio) / 3);
                    
                    if (array[mid1] === objetivo) {
                        return { encontrado: true, indice: mid1, iteraciones };
                    }
                    if (array[mid2] === objetivo) {
                        return { encontrado: true, indice: mid2, iteraciones };
                    }
                    
                    if (objetivo < array[mid1]) {
                        fin = mid1 - 1;
                    } else if (objetivo > array[mid2]) {
                        inicio = mid2 + 1;
                    } else {
                        inicio = mid1 + 1;
                        fin = mid2 - 1;
                    }
                }
                
                return { encontrado: false, iteraciones };
            },
            
            // Búsqueda con hashing
            busquedaHash: (array) => {
                // Crear índice hash
                const indiceHash = new Map();
                array.forEach((valor, indice) => {
                    if (!indiceHash.has(valor)) {
                        indiceHash.set(valor, []);
                    }
                    indiceHash.get(valor).push(indice);
                });
                
                return {
                    buscar: (objetivo) => {
                        const indices = indiceHash.get(objetivo);
                        return {
                            encontrado: !!indices,
                            indices: indices || [],
                            comparaciones: 1 // O(1) promedio
                        };
                    },
                    indice: indiceHash
                };
            },
            
            // Búsqueda en array rotado
            busquedaArrayRotado: (array, objetivo) => {
                let inicio = 0;
                let fin = array.length - 1;
                let iteraciones = 0;
                
                while (inicio <= fin) {
                    iteraciones++;
                    const medio = Math.floor((inicio + fin) / 2);
                    
                    if (array[medio] === objetivo) {
                        return { encontrado: true, indice: medio, iteraciones };
                    }
                    
                    // Determinar qué mitad está ordenada
                    if (array[inicio] <= array[medio]) {
                        // Mitad izquierda está ordenada
                        if (objetivo >= array[inicio] && objetivo < array[medio]) {
                            fin = medio - 1;
                        } else {
                            inicio = medio + 1;
                        }
                    } else {
                        // Mitad derecha está ordenada
                        if (objetivo > array[medio] && objetivo <= array[fin]) {
                            inicio = medio + 1;
                        } else {
                            fin = medio - 1;
                        }
                    }
                }
                
                return { encontrado: false, iteraciones };
            }
        };
        
        // Datos de prueba
        const datosUniformes = Array.from({length: 1000}, (_, i) => i * 10);
        const datosRotados = [4, 5, 6, 7, 0, 1, 2, 3];
        const datosConDuplicados = [1, 2, 2, 3, 3, 3, 4, 5, 5, 6];
        
        console.log("🧪 Pruebas con algoritmos especializados:");
        
        // Búsqueda interpolada
        console.log("\n📐 Búsqueda interpolada (datos uniformes):");
        console.time("Interpolada");
        const resultadoInterpolada = busquedasEspeciales.busquedaInterpolada(datosUniformes, 7500);
        console.timeEnd("Interpolada");
        console.log(resultadoInterpolada);
        
        // Comparar con binaria
        console.time("Binaria tradicional");
        let inicio = 0, fin = datosUniformes.length - 1, iteracionesBinaria = 0;
        while (inicio <= fin) {
            iteracionesBinaria++;
            const medio = Math.floor((inicio + fin) / 2);
            if (datosUniformes[medio] === 7500) break;
            if (datosUniformes[medio] < 7500) inicio = medio + 1;
            else fin = medio - 1;
        }
        console.timeEnd("Binaria tradicional");
        console.log("Binaria iteraciones:", iteracionesBinaria);
        
        // Búsqueda ternaria
        console.log("\n🔱 Búsqueda ternaria:");
        const resultadoTernaria = busquedasEspeciales.busquedaTernaria(datosUniformes, 7500);
        console.log(resultadoTernaria);
        
        // Búsqueda con hash
        console.log("\n# Búsqueda con hashing:");
        const buscadorHash = busquedasEspeciales.busquedaHash(datosConDuplicados);
        console.log("Buscar 3:", buscadorHash.buscar(3));
        console.log("Buscar 7:", buscadorHash.buscar(7));
        
        // Array rotado
        console.log("\n🔄 Búsqueda en array rotado:");
        console.log("Array rotado:", datosRotados);
        console.log("Buscar 0:", busquedasEspeciales.busquedaArrayRotado(datosRotados, 0));
        console.log("Buscar 6:", busquedasEspeciales.busquedaArrayRotado(datosRotados, 6));
        
        return busquedasEspeciales;
    }
}

// 🚀 Demostraciones Búsqueda Avanzada
console.log("🔍 ALGORITMOS DE BÚSQUEDA AVANZADOS");
AlgoritmosBusquedaAvanzados.busquedaLinealOptimizada();
AlgoritmosBusquedaAvanzados.busquedaBinariaVariantes();
AlgoritmosBusquedaAvanzados.busquedasEspecializadas();
```

**✅ CAPÍTULO 10 - PARTE 1 COMPLETADA**

### 🎯 **Lo que cubrimos en la Parte 1:**

#### 📊 **Análisis Big O:**
1. **⚡ Complejidades Básicas** - O(1), O(log n), O(n), O(n²), O(2^n)
2. **🎯 Análisis Práctico** - Identificar cuellos de botella, medir rendimiento  
3. **💾 Complejidad Espacial** - Trade-offs tiempo vs memoria

#### 🔍 **Algoritmos de Búsqueda:**
4. **📏 Búsqueda Lineal** - Optimizaciones, centinela, bidireccional
5. **📈 Búsqueda Binaria** - Variantes, primera/última ocurrencia, rangos
6. **🔀 Búsquedas Especializadas** - Interpolada, ternaria, hash, arrays rotados

---

## 10.2 📈 **Algoritmos y Rendimiento - PARTE 2**

### � **Algoritmos de Ordenamiento Esenciales**

```javascript
// 📊 Los algoritmos de ordenamiento más importantes
class AlgoritmosOrdenamiento {
    
    // 🫧 BUBBLE SORT - O(n²) - Educativo
    static bubbleSort(array) {
        const arr = [...array];
        let operaciones = 0;
        
        for (let i = 0; i < arr.length; i++) {
            for (let j = 0; j < arr.length - i - 1; j++) {
                operaciones++;
                if (arr[j] > arr[j + 1]) {
                    [arr[j], arr[j + 1]] = [arr[j + 1], arr[j]];
                }
            }
        }
        
        return { array: arr, operaciones };
    }
    
    // ⚡ QUICK SORT - O(n log n) promedio - Eficiente
    static quickSort(array) {
        let operaciones = 0;
        
        const sort = (arr, inicio = 0, fin = arr.length - 1) => {
            if (inicio < fin) {
                operaciones++;
                const pivotIndex = partition(arr, inicio, fin);
                sort(arr, inicio, pivotIndex - 1);
                sort(arr, pivotIndex + 1, fin);
            }
        };
        
        const partition = (arr, inicio, fin) => {
            const pivot = arr[fin];
            let i = inicio - 1;
            
            for (let j = inicio; j < fin; j++) {
                operaciones++;
                if (arr[j] <= pivot) {
                    i++;
                    [arr[i], arr[j]] = [arr[j], arr[i]];
                }
            }
            
            [arr[i + 1], arr[fin]] = [arr[fin], arr[i + 1]];
            return i + 1;
        };
        
        const arr = [...array];
        sort(arr);
        return { array: arr, operaciones };
    }
    
    // 🔄 MERGE SORT - O(n log n) - Estable
    static mergeSort(array) {
        let operaciones = 0;
        
        const merge = (izq, der) => {
            const resultado = [];
            let i = 0, j = 0;
            
            while (i < izq.length && j < der.length) {
                operaciones++;
                if (izq[i] <= der[j]) {
                    resultado.push(izq[i]);
                    i++;
                } else {
                    resultado.push(der[j]);
                    j++;
                }
            }
            
            return resultado.concat(izq.slice(i)).concat(der.slice(j));
        };
        
        const sort = (arr) => {
            if (arr.length <= 1) return arr;
            
            operaciones++;
            const medio = Math.floor(arr.length / 2);
            const izquierda = sort(arr.slice(0, medio));
            const derecha = sort(arr.slice(medio));
            
            return merge(izquierda, derecha);
        };
        
        return { array: sort(array), operaciones };
    }
    
    // 📊 COMPARACIÓN DE ALGORITMOS
    static compararAlgoritmos() {
        console.log("📊 Comparación de algoritmos de ordenamiento:");
        
        const datos = [64, 34, 25, 12, 22, 11, 90, 5];
        console.log("Datos originales:", datos);
        
        // Probar cada algoritmo
        console.time("Bubble Sort");
        const bubble = this.bubbleSort(datos);
        console.timeEnd("Bubble Sort");
        
        console.time("Quick Sort");
        const quick = this.quickSort(datos);
        console.timeEnd("Quick Sort");
        
        console.time("Merge Sort");
        const merge = this.mergeSort(datos);
        console.timeEnd("Merge Sort");
        
        console.log("\n📈 Resultados:");
        console.log("Bubble:", bubble.array, `(${bubble.operaciones} ops)`);
        console.log("Quick:", quick.array, `(${quick.operaciones} ops)`);
        console.log("Merge:", merge.array, `(${merge.operaciones} ops)`);
        
        // Tabla comparativa
        const comparacion = {
            "Bubble Sort": { complejidad: "O(n²)", estable: "Sí", memoria: "O(1)" },
            "Quick Sort": { complejidad: "O(n log n)", estable: "No", memoria: "O(log n)" },
            "Merge Sort": { complejidad: "O(n log n)", estable: "Sí", memoria: "O(n)" }
        };
        
        console.table(comparacion);
        
        return { bubble, quick, merge };
    }
}

// 🚀 Demo Ordenamiento
console.log("📊 ALGORITMOS DE ORDENAMIENTO");
AlgoritmosOrdenamiento.compararAlgoritmos();
```

### ⚡ **Optimización de Rendimiento**

```javascript
// ⚡ Técnicas de optimización práticas
class OptimizacionRendimiento {
    
    // 🎯 IDENTIFICAR CUELLOS DE BOTELLA
    static identificarProblemas() {
        console.log("🎯 Identificando cuellos de botella:");
        
        // ❌ Problemático: Operaciones costosas en loops
        const problemasComunes = {
            // DOM en loops
            domEnLoop: () => {
                for (let i = 0; i < 1000; i++) {
                    // ❌ Acceso al DOM en cada iteración
                    // document.getElementById('elemento').innerHTML += i;
                }
            },
            
            // Cálculos repetitivos
            calculosRepetitivos: (array) => {
                for (let i = 0; i < array.length; i++) {
                    // ❌ Cálculo costoso repetido
                    const factor = Math.sqrt(array.length) * 2.5;
                    array[i] *= factor;
                }
            },
            
            // Clonado ineficiente
            clonadoIneficiente: (objetos) => {
                return objetos.map(obj => 
                    JSON.parse(JSON.stringify(obj)) // ❌ Muy lento
                );
            }
        };
        
        // ✅ Soluciones optimizadas
        const solucionesOptimas = {
            // Batch DOM updates
            domOptimizado: () => {
                let html = '';
                for (let i = 0; i < 1000; i++) {
                    html += i;
                }
                // ✅ Una sola actualización
                // document.getElementById('elemento').innerHTML = html;
            },
            
            // Pre-calcular valores
            calculosOptimizados: (array) => {
                const factor = Math.sqrt(array.length) * 2.5; // ✅ Calculado una vez
                for (let i = 0; i < array.length; i++) {
                    array[i] *= factor;
                }
            },
            
            // Clonado eficiente
            clonadoOptimizado: (objetos) => {
                return objetos.map(obj => ({ ...obj })); // ✅ Spread operator
            }
        };
        
        // Benchmark básico
        const datos = Array.from({length: 1000}, (_, i) => ({ id: i, valor: i * 2 }));
        
        console.time("❌ Clonado ineficiente");
        problemasComunes.clonadoIneficiente(datos.slice(0, 100));
        console.timeEnd("❌ Clonado ineficiente");
        
        console.time("✅ Clonado optimizado");
        solucionesOptimas.clonadoOptimizado(datos.slice(0, 100));
        console.timeEnd("✅ Clonado optimizado");
        
        return { problemasComunes, solucionesOptimas };
    }
    
    // 📊 MEMOIZACIÓN Y CACHE
    static memoizacionCache() {
        console.log("📊 Memoización y cache:");
        
        // Cache simple con Map
        const cache = new Map();
        
        const fibonacci = (n) => {
            if (cache.has(n)) return cache.get(n);
            
            if (n <= 1) return n;
            const resultado = fibonacci(n - 1) + fibonacci(n - 2);
            
            cache.set(n, resultado);
            return resultado;
        };
        
        // Cache con TTL
        const cacheConTTL = () => {
            const cache = new Map();
            
            return {
                get: (key) => {
                    const item = cache.get(key);
                    if (item && Date.now() < item.expira) {
                        return item.valor;
                    }
                    cache.delete(key);
                    return null;
                },
                
                set: (key, valor, ttl = 5000) => {
                    cache.set(key, {
                        valor,
                        expira: Date.now() + ttl
                    });
                }
            };
        };
        
        // Demostración
        console.time("Fibonacci con cache");
        console.log("Fib(40):", fibonacci(40));
        console.timeEnd("Fibonacci con cache");
        
        const cacheInteligente = cacheConTTL();
        cacheInteligente.set('usuario', { id: 1, nombre: 'Ana' });
        console.log("Cache get:", cacheInteligente.get('usuario'));
        
        return { fibonacci, cacheConTTL };
    }
    
    // 🎯 TÉCNICAS AVANZADAS
    static tecnicasAvanzadas() {
        console.log("🎯 Técnicas avanzadas de optimización:");
        
        // Debounce
        const debounce = (func, delay) => {
            let timeoutId;
            return (...args) => {
                clearTimeout(timeoutId);
                timeoutId = setTimeout(() => func.apply(this, args), delay);
            };
        };
        
        // Throttle
        const throttle = (func, limit) => {
            let inThrottle;
            return (...args) => {
                if (!inThrottle) {
                    func.apply(this, args);
                    inThrottle = true;
                    setTimeout(() => inThrottle = false, limit);
                }
            };
        };
        
        // Lazy loading
        const lazyLoad = (getData) => {
            let data = null;
            return () => {
                if (!data) {
                    console.log("🔄 Cargando datos...");
                    data = getData();
                }
                return data;
            };
        };
        
        // Batch processing
        const batchProcessor = (items, batchSize = 100) => {
            const batches = [];
            for (let i = 0; i < items.length; i += batchSize) {
                batches.push(items.slice(i, i + batchSize));
            }
            return batches;
        };
        
        // Demostración
        const busquedaDebounced = debounce((termino) => {
            console.log("🔍 Buscando:", termino);
        }, 300);
        
        const datos = lazyLoad(() => Array.from({length: 10000}, (_, i) => i));
        console.log("Lazy data size:", datos().length);
        
        const lotes = batchProcessor(Array.from({length: 1000}, (_, i) => i), 50);
        console.log("Batches creados:", lotes.length);
        
        return { debounce, throttle, lazyLoad, batchProcessor };
    }
}

// 🚀 Demo Optimización
console.log("⚡ OPTIMIZACIÓN DE RENDIMIENTO");
OptimizacionRendimiento.identificarProblemas();
OptimizacionRendimiento.memoizacionCache();
OptimizacionRendimiento.tecnicasAvanzadas();
```

### 🎯 **Cuándo Usar Cada Algoritmo**

```javascript
// � Guía de decisión para algoritmos
class GuiaDecision {
    
    static recomendacionesAlgoritmos() {
        console.log("🎯 Cuándo usar cada algoritmo:");
        
        const recomendaciones = {
            // Búsqueda
            busqueda: {
                "Datos pequeños (<100)": "Búsqueda lineal",
                "Datos ordenados": "Búsqueda binaria",
                "Acceso frecuente": "Hash table (Map)",
                "Datos dinámicos": "Índices con Map/Set"
            },
            
            // Ordenamiento
            ordenamiento: {
                "Datos pequeños (<50)": "Insertion sort",
                "Uso general": "Quick sort",
                "Estabilidad requerida": "Merge sort",
                "Memoria limitada": "Heap sort",
                "Datos casi ordenados": "Insertion sort"
            },
            
            // Estructuras de datos
            estructuras: {
                "Lista simple": "Array",
                "Clave-valor": "Object/Map",
                "Valores únicos": "Set",
                "Datos temporales": "WeakMap/WeakSet",
                "Cola FIFO": "Array con push/shift",
                "Pila LIFO": "Array con push/pop"
            }
        };
        
        console.table(recomendaciones.busqueda);
        console.table(recomendaciones.ordenamiento);
        console.table(recomendaciones.estructuras);
        
        return recomendaciones;
    }
    
    static ejemplosPracticos() {
        console.log("💡 Ejemplos prácticos de decisión:");
        
        // Escenario 1: E-commerce
        const ecommerce = {
            problema: "Buscar productos en catálogo de 10,000 items",
            solucion: "Map con índices por categoría + búsqueda binaria por precio",
            codigo: () => {
                const productos = new Map();
                const porCategoria = new Map();
                
                // Indexar por categoría
                return { productos, porCategoria };
            }
        };
        
        // Escenario 2: Real-time chat
        const chat = {
            problema: "Gestionar mensajes y usuarios conectados",
            solucion: "Array para mensajes + Set para usuarios online",
            codigo: () => {
                const mensajes = []; // Orden cronológico
                const usuariosOnline = new Set(); // Únicos, rápido has()
                
                return { mensajes, usuariosOnline };
            }
        };
        
        // Escenario 3: Analytics
        const analytics = {
            problema: "Procesar 1M eventos, contar únicos",
            solucion: "Set para únicos + Map para contadores",
            codigo: () => {
                const eventosUnicos = new Set();
                const contadores = new Map();
                
                return { eventosUnicos, contadores };
            }
        };
        
        console.log("🛒 E-commerce:", ecommerce.problema);
        console.log("💬 Chat:", chat.problema);
        console.log("📊 Analytics:", analytics.problema);
        
        return { ecommerce, chat, analytics };
    }
}

// 🚀 Demo Guía
console.log("🎯 GUÍA DE DECISIÓN");
GuiaDecision.recomendacionesAlgoritmos();
GuiaDecision.ejemplosPracticos();
```

**✅ CAPÍTULO 10 - PARTE 2 COMPLETADA**

### 🎯 **Lo que cubrimos en la Parte 2:**

#### 📊 **Algoritmos de Ordenamiento:**
1. **🫧 Bubble Sort** - O(n²), educativo, estable
2. **⚡ Quick Sort** - O(n log n), eficiente, inestable  
3. **🔄 Merge Sort** - O(n log n), estable, usa más memoria

#### ⚡ **Optimización de Rendimiento:**
4. **🎯 Identificar Problemas** - DOM loops, cálculos repetitivos, clonado
5. **📊 Memoización y Cache** - Cache simple, TTL, fibonacci optimizado
6. **🎯 Técnicas Avanzadas** - Debounce, throttle, lazy loading, batching

#### 🎯 **Guía de Decisión:**
7. **💡 Cuándo Usar Qué** - Recomendaciones por escenario
8. **🛒 Ejemplos Prácticos** - E-commerce, chat, analytics

### 🔄 **PRÓXIMO: CAPÍTULO 11 - FINAL**

**🏗️ Estructuras Especializadas y Proyectos** - Stack, Queue, Trees, proyecto final

**⏰ Tiempo estimado:** 6-8 minutos

**🚀 ¿Terminamos con el Capítulo 11 final?**

---

## 11. 🏗️ **Estructuras Especializadas y Proyectos**

### 🌟 **Stack - Pila LIFO**

```javascript
// 🏗️ Implementación de Stack (Pila)
class Stack {
    constructor() {
        this.items = [];
    }
    
    // Agregar elemento al tope
    push(element) {
        this.items.push(element);
        return this.size();
    }
    
    // Remover elemento del tope
    pop() {
        if (this.isEmpty()) return null;
        return this.items.pop();
    }
    
    // Ver elemento del tope sin remover
    peek() {
        if (this.isEmpty()) return null;
        return this.items[this.items.length - 1];
    }
    
    // Verificar si está vacía
    isEmpty() {
        return this.items.length === 0;
    }
    
    // Obtener tamaño
    size() {
        return this.items.length;
    }
    
    // Limpiar stack
    clear() {
        this.items = [];
    }
}

// 🚀 Ejemplo práctico: Validador de paréntesis
class ValidadorParentesis {
    static validar(expresion) {
        const stack = new Stack();
        const pares = { '(': ')', '[': ']', '{': '}' };
        
        for (let char of expresion) {
            if (char in pares) {
                stack.push(char);
            } else if (Object.values(pares).includes(char)) {
                if (stack.isEmpty()) return false;
                const ultimo = stack.pop();
                if (pares[ultimo] !== char) return false;
            }
        }
        
        return stack.isEmpty();
    }
}

console.log("Paréntesis válidos:", ValidadorParentesis.validar("({[]})"));
console.log("Paréntesis inválidos:", ValidadorParentesis.validar("({[})"));
```

### 🔄 **Queue - Cola FIFO**

```javascript
// 🔄 Implementación de Queue (Cola)
class Queue {
    constructor() {
        this.items = [];
    }
    
    // Agregar al final
    enqueue(element) {
        this.items.push(element);
        return this.size();
    }
    
    // Remover del inicio
    dequeue() {
        if (this.isEmpty()) return null;
        return this.items.shift();
    }
    
    // Ver primer elemento
    front() {
        if (this.isEmpty()) return null;
        return this.items[0];
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
}

// 🚀 Ejemplo práctico: Sistema de tareas
class SistemaTareas {
    constructor() {
        this.cola = new Queue();
        this.procesando = false;
    }
    
    agregarTarea(tarea) {
        this.cola.enqueue(tarea);
        console.log(`📋 Tarea agregada: ${tarea.nombre}`);
        
        if (!this.procesando) {
            this.procesarSiguiente();
        }
    }
    
    async procesarSiguiente() {
        if (this.cola.isEmpty()) {
            this.procesando = false;
            return;
        }
        
        this.procesando = true;
        const tarea = this.cola.dequeue();
        
        console.log(`⚡ Procesando: ${tarea.nombre}`);
        await new Promise(resolve => setTimeout(resolve, tarea.duracion));
        console.log(`✅ Completada: ${tarea.nombre}`);
        
        this.procesarSiguiente();
    }
}

// Demo
const sistema = new SistemaTareas();
sistema.agregarTarea({ nombre: "Enviar email", duracion: 1000 });
sistema.agregarTarea({ nombre: "Procesar datos", duracion: 2000 });
```

### 🌳 **Árboles Binarios Básicos**

```javascript
// 🌳 Nodo de Árbol Binario
class NodoArbol {
    constructor(valor) {
        this.valor = valor;
        this.izquierda = null;
        this.derecha = null;
    }
}

// 🌳 Árbol Binario de Búsqueda
class ArbolBinario {
    constructor() {
        this.raiz = null;
    }
    
    insertar(valor) {
        this.raiz = this._insertarRecursivo(this.raiz, valor);
    }
    
    _insertarRecursivo(nodo, valor) {
        if (nodo === null) {
            return new NodoArbol(valor);
        }
        
        if (valor < nodo.valor) {
            nodo.izquierda = this._insertarRecursivo(nodo.izquierda, valor);
        } else if (valor > nodo.valor) {
            nodo.derecha = this._insertarRecursivo(nodo.derecha, valor);
        }
        
        return nodo;
    }
    
    buscar(valor) {
        return this._buscarRecursivo(this.raiz, valor);
    }
    
    _buscarRecursivo(nodo, valor) {
        if (nodo === null || nodo.valor === valor) {
            return nodo;
        }
        
        if (valor < nodo.valor) {
            return this._buscarRecursivo(nodo.izquierda, valor);
        }
        
        return this._buscarRecursivo(nodo.derecha, valor);
    }
    
    // Recorrido inorden (izquierda, raíz, derecha)
    inorden() {
        const resultado = [];
        this._inordenRecursivo(this.raiz, resultado);
        return resultado;
    }
    
    _inordenRecursivo(nodo, resultado) {
        if (nodo !== null) {
            this._inordenRecursivo(nodo.izquierda, resultado);
            resultado.push(nodo.valor);
            this._inordenRecursivo(nodo.derecha, resultado);
        }
    }
}

// Demo
const arbol = new ArbolBinario();
[50, 30, 70, 20, 40, 60, 80].forEach(valor => arbol.insertar(valor));

console.log("Recorrido inorden:", arbol.inorden());
console.log("Buscar 40:", arbol.buscar(40) ? "Encontrado" : "No encontrado");
```

### 🎯 **Proyecto Final: Sistema de Gestión de Datos**

```javascript
// 🎯 Proyecto integrador que usa todas las estructuras
class SistemaGestionDatos {
    constructor() {
        // Diferentes estructuras para diferentes propósitos
        this.usuarios = new Map(); // ID -> Usuario
        this.sesionesActivas = new Set(); // IDs de sesiones activas
        this.historialAcciones = new Stack(); // Historial para deshacer
        this.colaTareas = new Queue(); // Tareas pendientes
        this.indiceEmails = new Map(); // Email -> ID usuario
        this.metadatos = new WeakMap(); // Datos privados de objetos
    }
    
    // 👤 Gestión de usuarios
    crearUsuario(datos) {
        const id = Date.now().toString();
        const usuario = { id, ...datos, fechaCreacion: new Date() };
        
        this.usuarios.set(id, usuario);
        this.indiceEmails.set(datos.email, id);
        
        // Acción para historial
        this.historialAcciones.push({
            tipo: 'CREAR_USUARIO',
            usuario: { ...usuario },
            timestamp: Date.now()
        });
        
        // Metadatos privados
        this.metadatos.set(usuario, {
            intentosLogin: 0,
            ultimoAcceso: null
        });
        
        console.log(`✅ Usuario creado: ${datos.nombre} (${id})`);
        return usuario;
    }
    
    // 🔐 Gestión de sesiones
    iniciarSesion(email, password) {
        const userId = this.indiceEmails.get(email);
        if (!userId) return { exito: false, mensaje: "Usuario no encontrado" };
        
        const usuario = this.usuarios.get(userId);
        const metadatos = this.metadatos.get(usuario);
        
        if (usuario.password === password) {
            this.sesionesActivas.add(userId);
            metadatos.ultimoAcceso = new Date();
            metadatos.intentosLogin = 0;
            
            console.log(`🔐 Sesión iniciada: ${usuario.nombre}`);
            return { exito: true, usuario };
        } else {
            metadatos.intentosLogin++;
            return { exito: false, mensaje: "Contraseña incorrecta" };
        }
    }
    
    // 📊 Analytics y reportes
    generarReporte() {
        const totalUsuarios = this.usuarios.size;
        const sesionesActivas = this.sesionesActivas.size;
        const accionesRecientes = [];
        
        // Obtener últimas 5 acciones
        const historialTemp = new Stack();
        for (let i = 0; i < 5 && !this.historialAcciones.isEmpty(); i++) {
            const accion = this.historialAcciones.pop();
            accionesRecientes.push(accion);
            historialTemp.push(accion);
        }
        
        // Restaurar historial
        while (!historialTemp.isEmpty()) {
            this.historialAcciones.push(historialTemp.pop());
        }
        
        const reporte = {
            totalUsuarios,
            sesionesActivas,
            accionesRecientes,
            usuariosConMasIntentos: this.obtenerUsuariosConMasIntentos(),
            fechaReporte: new Date()
        };
        
        console.log("📊 Reporte generado:", reporte);
        return reporte;
    }
    
    obtenerUsuariosConMasIntentos() {
        const usuarios = [];
        
        for (let [id, usuario] of this.usuarios) {
            const metadatos = this.metadatos.get(usuario);
            if (metadatos && metadatos.intentosLogin > 2) {
                usuarios.push({
                    id,
                    nombre: usuario.nombre,
                    intentos: metadatos.intentosLogin
                });
            }
        }
        
        return usuarios.sort((a, b) => b.intentos - a.intentos);
    }
    
    // ↩️ Deshacer última acción
    deshacerUltima() {
        if (this.historialAcciones.isEmpty()) {
            console.log("❌ No hay acciones para deshacer");
            return false;
        }
        
        const ultimaAccion = this.historialAcciones.pop();
        
        if (ultimaAccion.tipo === 'CREAR_USUARIO') {
            const usuario = ultimaAccion.usuario;
            this.usuarios.delete(usuario.id);
            this.indiceEmails.delete(usuario.email);
            this.sesionesActivas.delete(usuario.id);
            
            console.log(`↩️ Usuario eliminado: ${usuario.nombre}`);
        }
        
        return true;
    }
}

// 🚀 Demo del sistema completo
console.log("🎯 DEMO: Sistema de Gestión de Datos");

const sistema = new SistemaGestionDatos();

// Crear usuarios
const ana = sistema.crearUsuario({
    nombre: "Ana García",
    email: "ana@email.com",
    password: "123456"
});

const carlos = sistema.crearUsuario({
    nombre: "Carlos López", 
    email: "carlos@email.com",
    password: "abcdef"
});

// Iniciar sesiones
sistema.iniciarSesion("ana@email.com", "123456");
sistema.iniciarSesion("carlos@email.com", "wrong"); // Falla
sistema.iniciarSesion("carlos@email.com", "wrong"); // Falla
sistema.iniciarSesion("carlos@email.com", "wrong"); // Falla

// Generar reporte
sistema.generarReporte();

// Deshacer última acción
sistema.deshacerUltima();
```

**✅ CAPÍTULO 11 COMPLETADO**

### 🎯 **Resumen del Capítulo Final:**

1. **🏗️ Stack (Pila)** - LIFO, validación de paréntesis, historial
2. **🔄 Queue (Cola)** - FIFO, sistema de tareas, procesamiento secuencial  
3. **🌳 Árboles Binarios** - BST, búsqueda eficiente, recorridos
4. **🎯 Proyecto Integrador** - Combinación de todas las estructuras

---

## 12. 🧪 **Ejercicios Interactivos**

[🔝 Volver al Índice](#-navegación-rápida) | [⬅️ Anterior: Estructuras Especializadas](#11-🏗️-estructuras-especializadas-y-proyectos) | [➡️ Siguiente: Recursos y Referencias](#13-📚-recursos-y-referencias)

> **🧪 "Los datos sin práctica son solo teoría. Cada ejercicio es un paso hacia la maestría en estructuras de datos."**

### 🎯 **Metodología de Práctica DATOS**

Para resolver ejercicios de estructuras de datos, usa la metodología **DATOS**:

| **Paso** | **Acción** | **Descripción** |
|:---------|:-----------|:----------------|
| **📊 D**atos | Datos | Analiza qué estructura es más eficiente |
| **🎯 A**nálisis | Análisis | Evalúa complejidad temporal y espacial |
| **🧪 T**est | Test | Crea casos de prueba con diferentes tamaños |
| **⚡ O**ptimización | Optimización | Mejora rendimiento si es necesario |
| **💻 S**olución | Solución | Implementa y valida tu código |

---

### 🟢 **NIVEL BÁSICO** - *"Fundamentos de Estructuras"*

#### 🎯 **Ejercicio 1: Gestor de Lista de Compras**

**📝 Enunciado:**
Crea un sistema `ListaCompras` que permita:
- Agregar productos con cantidad y precio
- Eliminar productos por nombre
- Calcular el total de la compra
- Mostrar productos ordenados por precio
- Buscar productos que contengan una palabra clave

```javascript
// 🎯 Tu solución aquí
class ListaCompras {
    constructor() {
        // Implementa tu estructura de datos
    }
    
    agregar(nombre, cantidad, precio) {
        // Tu código aquí
    }
    
    eliminar(nombre) {
        // Tu código aquí
    }
    
    calcularTotal() {
        // Tu código aquí
    }
    
    ordenarPorPrecio() {
        // Tu código aquí
    }
    
    buscar(palabraClave) {
        // Tu código aquí
    }
}

// 🧪 Casos de prueba
const lista = new ListaCompras();
lista.agregar("Manzanas", 5, 2.5);
lista.agregar("Pan", 2, 1.8);
lista.agregar("Leche", 1, 3.2);

console.log(lista.calcularTotal()); // Total esperado
console.log(lista.buscar("man")); // Debería encontrar "Manzanas"
```

<details>
<summary>💡 <strong>Ver Solución</strong></summary>

```javascript
class ListaCompras {
    constructor() {
        this.productos = new Map(); // nombre -> {cantidad, precio}
        this.totalCalculado = 0;
    }
    
    agregar(nombre, cantidad, precio) {
        if (typeof nombre !== 'string' || cantidad <= 0 || precio <= 0) {
            throw new Error('Parámetros inválidos');
        }
        
        this.productos.set(nombre.toLowerCase(), {
            nombre: nombre,
            cantidad: cantidad,
            precio: precio,
            subtotal: cantidad * precio
        });
        
        return `✅ ${nombre} agregado exitosamente`;
    }
    
    eliminar(nombre) {
        const eliminado = this.productos.delete(nombre.toLowerCase());
        return eliminado ? `🗑️ ${nombre} eliminado` : `❌ ${nombre} no encontrado`;
    }
    
    calcularTotal() {
        this.totalCalculado = 0;
        for (let [, producto] of this.productos) {
            this.totalCalculado += producto.subtotal;
        }
        return this.totalCalculado;
    }
    
    ordenarPorPrecio() {
        return Array.from(this.productos.values())
            .sort((a, b) => a.precio - b.precio);
    }
    
    buscar(palabraClave) {
        const resultados = [];
        const busqueda = palabraClave.toLowerCase();
        
        for (let [, producto] of this.productos) {
            if (producto.nombre.toLowerCase().includes(busqueda)) {
                resultados.push(producto);
            }
        }
        
        return resultados;
    }
    
    mostrarResumen() {
        return {
            totalProductos: this.productos.size,
            total: this.calcularTotal(),
            productos: Array.from(this.productos.values())
        };
    }
}
```

**🧠 Análisis de la Solución:**
- **Estructura:** Map para búsqueda O(1) por nombre
- **Complejidad:** Agregar/eliminar O(1), ordenar O(n log n)
- **Ventajas:** Búsqueda rápida, sin duplicados de nombres
</details>

---

#### 🎯 **Ejercicio 2: Cache Inteligente**

**📝 Enunciado:**
Implementa un `CacheInteligente` con las siguientes características:
- Capacidad máxima limitada
- Eliminación de elementos menos usados (LRU)
- TTL (Time To Live) configurable por elemento
- Estadísticas de hit/miss ratio

```javascript
// 🎯 Tu solución aquí
class CacheInteligente {
    constructor(capacidadMaxima = 10) {
        // Implementa tu estructura
    }
    
    set(clave, valor, ttl = 0) {
        // Tu código aquí
    }
    
    get(clave) {
        // Tu código aquí
    }
    
    delete(clave) {
        // Tu código aquí
    }
    
    getEstadisticas() {
        // Tu código aquí
    }
}

// 🧪 Casos de prueba
const cache = new CacheInteligente(3);
cache.set('user1', {nombre: 'Ana'}, 5000);
cache.set('user2', {nombre: 'Carlos'});
console.log(cache.get('user1')); // Debería devolver el objeto
```

---

### 🟡 **NIVEL INTERMEDIO** - *"Algoritmos y Optimización"*

#### 🎯 **Ejercicio 3: Analizador de Rendimiento**

**📝 Enunciado:**
Crea un `AnalizadorRendimiento` que compare diferentes algoritmos de ordenamiento:
- Bubble Sort, Quick Sort, Merge Sort
- Mida tiempo de ejecución
- Cuente comparaciones e intercambios
- Genere reportes comparativos

#### 🎯 **Ejercicio 4: Sistema de Recomendaciones**

**📝 Enunciado:**
Implementa un sistema que use diferentes estructuras para recomendar productos:
- Set para categorías de interés del usuario
- Map para puntuaciones de productos
- Array para historial de compras
- WeakMap para datos de sesión

---

### 🔴 **NIVEL AVANZADO** - *"Estructuras Personalizadas"*

#### 🎯 **Ejercicio 5: Graph de Redes Sociales**

**📝 Enunciado:**
Crea un grafo para modelar una red social con:
- Usuarios como nodos
- Conexiones como aristas con peso (fuerza de amistad)
- Algoritmos de búsqueda BFS y DFS
- Detección de comunidades

#### 🎯 **Ejercicio 6: Base de Datos en Memoria**

**📝 Enunciado:**
Implementa una mini base de datos que combine:
- Índices con Map para búsqueda rápida
- Heap para consultas TOP-N
- Trie para búsqueda de texto
- Transacciones con rollback

---

### 🟣 **NIVEL EXPERTO** - *"Proyectos del Mundo Real"*

#### 🎯 **Ejercicio 7: Motor de Búsqueda**

**📝 Enunciado:**
Construye un motor de búsqueda que incluya:
- Índice invertido con Map anidados
- Ranking por relevancia
- Búsqueda fuzzy (tolerante a errores)
- Cache de resultados con LRU

#### 🎯 **Ejercicio 8: Sistema de Trading**

**📝 Enunciado:**
Implementa un sistema de trading con:
- Order book usando heaps min/max
- Historia de precios con circular buffer
- Indicadores técnicos con ventanas deslizantes
- Detección de patrones en tiempo real

---

### 🏆 **Desafíos de Integración**

```javascript
// 🎮 DESAFÍO FINAL: E-commerce Completo
const desafioFinal = {
    nombre: "Sistema E-commerce Integral",
    duracion: "2-3 días",
    estructuras: [
        "Map para catálogo de productos",
        "Set para filtros activos", 
        "Stack para navegación (historial)",
        "Queue para procesamiento de pedidos",
        "Tree para categorías jerárquicas",
        "Graph para recomendaciones",
        "Cache para optimización"
    ],
    funcionalidades: [
        "Catálogo con búsqueda y filtros",
        "Carrito de compras persistente",
        "Sistema de recomendaciones",
        "Gestión de inventario",
        "Analytics en tiempo real",
        "Optimización de rendimiento"
    ]
};

console.log("🚀 ¿Listo para el desafío final?");
```

---

### 📊 **Autoevaluación**

Marca tu progreso:

- [ ] **🟢 Básico**: Domino arrays y objetos básicos
- [ ] **🟡 Intermedio**: Uso Map/Set eficientemente y analizo complejidad
- [ ] **🔴 Avanzado**: Implemento estructuras personalizadas
- [ ] **🟣 Experto**: Combino múltiples estructuras en proyectos reales
- [ ] **🏆 Maestro**: Optimizo rendimiento y resuelvo problemas complejos

**🎯 Tu siguiente paso:** Si tienes menos de 3 marcas, repasa los capítulos correspondientes. ¡La práctica hace al maestro!

---

## 13. 📚 **Recursos y Referencias**

### 🎮 **Desafíos Progresivos**

```javascript
// 🎮 EJERCICIOS INTERACTIVOS
const ejerciciosEstructuras = {
    
    // 🟢 NIVEL BÁSICO
    basico: {
        ejercicio1: "Crear un array con 5 nombres y mostrar cada uno",
        ejercicio2: "Crear un objeto persona con nombre, edad y email",
        ejercicio3: "Usar map() para convertir números a su cuadrado"
    },
    
    // 🟡 NIVEL INTERMEDIO  
    intermedio: {
        ejercicio4: "Filtrar productos por precio usando filter()",
        ejercicio5: "Calcular promedio de calificaciones con reduce()",
        ejercicio6: "Crear un Set de emails únicos de usuarios"
    },
    
    // 🔴 NIVEL AVANZADO
    avanzado: {
        ejercicio7: "Implementar un cache con Map y TTL",
        ejercicio8: "Crear un Stack para calculadora RPN",
        ejercicio9: "Sistema de navegación con historial (Stack + Queue)"
    },
    
    // 🟣 NIVEL EXPERTO
    experto: {
        ejercicio10: "Árbol binario con auto-balanceo básico",
        ejercicio11: "Graph con BFS y DFS",
        ejercicio12: "Sistema completo de gestión de datos"
    }
};

console.log("🎮 ¡Elige tu nivel y comienza a practicar!");
```

### 🏆 **Proyectos de Aplicación**

1. **🛒 E-commerce Cart** - Array de productos, Map de inventarios
2. **📚 Biblioteca Digital** - Objetos anidados, búsqueda avanzada
3. **🎵 Playlist Manager** - Stack para historial, Queue para reproducción
4. **📊 Analytics Dashboard** - Agregaciones con reduce, visualización
5. **🌐 Social Network** - Grafos, Map de conexiones, Set de seguidores

---

---

## 13. 📚 **Recursos y Referencias**

[🔝 Volver al Índice](#-navegación-rápida) | [⬅️ Anterior: Ejercicios Interactivos](#12-🧪-ejercicios-interactivos)

> **📚 "El conocimiento de estructuras de datos es una inversión que paga dividendos durante toda tu carrera. Aquí tienes las mejores fuentes para seguir creciendo."**

### 🌟 **Documentación Oficial**

#### 📖 **JavaScript - Estructuras de Datos**

| **🔗 Recurso** | **📝 Descripción** | **🎯 Nivel** | **🌐 Idioma** |
|:---------------|:-------------------|:-------------|:--------------|
| [MDN Array Methods](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/Array) | 📊 Referencia completa de métodos de arrays | Todos | 🇪🇸/🇺🇸 |
| [MDN Object Reference](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/Object) | 🏛️ Documentación completa de objetos | Todos | 🇪🇸/🇺🇸 |
| [MDN Map y Set](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/Map) | 🗺️ Guía oficial de estructuras modernas | Intermedio | 🇪🇸/🇺🇸 |
| [ECMAScript Collections](https://tc39.es/ecma262/#sec-keyed-collections) | 📋 Especificación oficial de colecciones | Avanzado | 🇺🇸 Inglés |

#### 🧠 **Algoritmos y Complejidad**

| **🔗 Recurso** | **📝 Descripción** | **🎯 Especialidad** |
|:---------------|:-------------------|:-------------------|
| [Big O Cheat Sheet](https://www.bigocheatsheet.com/) | ⚡ Referencia rápida de complejidades | Análisis de rendimiento |
| [VisuAlgo](https://visualgo.net/en) | 🎮 Visualización interactiva de algoritmos | Aprendizaje visual |
| [Algorithm Visualizer](https://algorithm-visualizer.org/) | 🎯 Simulador de algoritmos paso a paso | Debugging mental |

### 🛠️ **Herramientas de Desarrollo**

#### 💻 **Editores y IDEs**

```javascript
// 🎯 Configuración recomendada para desarrollo de estructuras de datos
const herramientasEstructuras = {
    editores: {
        vscode: {
            nombre: "Visual Studio Code",
            url: "https://code.visualstudio.com/",
            extensionesEsenciales: [
                "JavaScript (ES6) code snippets",
                "Quokka.js - Live JavaScript evaluation",
                "Code Runner - Ejecutar código rápidamente",
                "Prettier - Formateo automático",
                "ESLint - Análisis de código",
                "Data Structure Visualizer",
                "Performance Monitor"
            ],
            configuracion: {
                "editor.inlineSuggest.enabled": true,
                "editor.formatOnSave": true,
                "javascript.preferences.includePackageJsonAutoImports": "auto"
            }
        },
        alternativas: {
            webstorm: "IDE potente con análisis profundo (pago)",
            sublime: "Editor ligero y rápido",
            atom: "Hackeable, pero descontinuado"
        }
    },
    
    navegadores: {
        chrome: {
            devtools: {
                performance: "Análisis de rendimiento de algoritmos",
                memory: "Monitoreo de uso de memoria",
                profiler: "Detección de memory leaks"
            },
            extensiones: [
                "JSON Viewer - Para visualizar datos",
                "Performance Monitor - Métricas en tiempo real"
            ]
        },
        firefox: {
            ventajas: "Excelente debugger y herramientas de memoria",
            devtools: "Performance profiling avanzado"
        }
    },
    
    online: {
        plataformas: {
            codepen: {
                url: "https://codepen.io/",
                uso: "Prototipos rápidos y demostraciones",
                ventaja: "Visualización inmediata"
            },
            jsfiddle: {
                url: "https://jsfiddle.net/",
                uso: "Compartir ejemplos de código",
                ventaja: "Colaboración fácil"
            },
            replit: {
                url: "https://replit.com/",
                uso: "Desarrollo completo en la nube",
                ventaja: "Entorno completo con Node.js"
            },
            codesandbox: {
                url: "https://codesandbox.io/",
                uso: "Proyectos más complejos",
                ventaja: "Integración con npm y frameworks"
            }
        }
    }
};

console.log("🚀 Herramientas configuradas para estructuras de datos");
```

#### 🧪 **Testing y Benchmarking**

```javascript
// 🧪 Herramientas para probar y medir rendimiento
const herramientasTesting = {
    testing: {
        jest: {
            uso: "Testing unitario de estructuras",
            ejemplo: "Validar comportamiento de Stack/Queue"
        },
        mocha: {
            uso: "Testing flexible con múltiples reporters",
            ventaja: "Gran ecosistema de plugins"
        }
    },
    
    benchmarking: {
        benchmark_js: {
            uso: "Medir rendimiento de algoritmos",
            ejemplo: "Comparar diferentes implementaciones de sort"
        },
        performance_now: {
            uso: "Medición básica en navegador",
            nativo: "performance.now() en DevTools"
        }
    },
    
    profiling: {
        chrome_devtools: "Memory tab para detectar leaks",
        node_profiler: "node --prof para análisis servidor",
        heap_snapshots: "Comparar uso de memoria entre ejecuciones"
    }
};
```

---

### 📚 **Libros y Cursos Recomendados**

#### 📖 **Libros Esenciales**

```javascript
const bibliotecaEstructuras = {
    principiante: [
        {
            titulo: "JavaScript: The Good Parts",
            autor: "Douglas Crockford",
            enfoque: "Fundamentos sólidos del lenguaje",
            capitulos_clave: ["Arrays", "Objects", "Functions"]
        },
        {
            titulo: "Eloquent JavaScript", 
            autor: "Marijn Haverbeke",
            enfoque: "Programación práctica con estructuras",
            online: "https://eloquentjavascript.net/"
        }
    ],
    
    intermedio: [
        {
            titulo: "Data Structures and Algorithms with JavaScript",
            autor: "Michael McMillan",
            enfoque: "Implementación práctica de estructuras",
            temas: ["Lists", "Stacks", "Queues", "Trees", "Graphs"]
        },
        {
            titulo: "Learning JavaScript Data Structures and Algorithms",
            autor: "Loiane Groner",
            enfoque: "Estructuras modernas con ES6+",
            actualizacion: "Incluye Map, Set, WeakMap"
        }
    ],
    
    avanzado: [
        {
            titulo: "Introduction to Algorithms (CLRS)",
            autor: "Cormen, Leiserson, Rivest, Stein",
            enfoque: "Teoría profunda de algoritmos",
            advertencia: "Muy matemático, pero definitivo"
        },
        {
            titulo: "Algorithm Design Manual",
            autor: "Steven Skiena",
            enfoque: "Aplicación práctica de algoritmos",
            ventaja: "War stories y casos reales"
        }
    ]
};
```

#### 🎓 **Cursos y Plataformas**

| **🎓 Plataforma** | **📝 Curso Recomendado** | **💰 Precio** | **🎯 Nivel** |
|:------------------|:-------------------------|:--------------|:-------------|
| **freeCodeCamp** | JavaScript Algorithms and Data Structures | Gratuito | Principiante-Intermedio |
| **Coursera** | Algorithms Specialization (Stanford) | $39/mes | Avanzado |
| **edX** | Introduction to Computer Science (MIT) | Gratuito/Auditoria | Todos |
| **Udemy** | JavaScript Data Structures - The Definitive Guide | $10-50 | Intermedio |
| **Pluralsight** | JavaScript Data Structures | $29/mes | Intermedio-Avanzado |

---

### 🌐 **Comunidades y Recursos Online**

#### 👥 **Comunidades de Desarrollo**

```javascript
const comunidadesRecomendadas = {
    forums: {
        stackoverflow: {
            url: "https://stackoverflow.com/questions/tagged/javascript",
            uso: "Preguntas específicas sobre implementación",
            tags_útiles: ["javascript", "algorithm", "data-structures"]
        },
        reddit: {
            subreddits: [
                "r/javascript - Comunidad general",
                "r/algorithms - Discusión de algoritmos", 
                "r/programming - Temas generales"
            ]
        }
    },
    
    discord_slack: {
        javascript: "Servidor Discord de JavaScript",
        devchat: "Slack workspace para desarrolladores",
        freecodecamp: "Comunidad muy activa y helpful"
    },
    
    github: {
        repositorios_estudio: [
            "trekhleb/javascript-algorithms",
            "yangshun/tech-interview-handbook",
            "kdn251/interviews"
        ],
        organizaciones: [
            "javascript-tutorials",
            "TheAlgorithms"
        ]
    }
};
```

#### 🎮 **Plataformas de Práctica**

| **🎮 Plataforma** | **🎯 Especialidad** | **💡 Mejor Para** |
|:------------------|:--------------------|:------------------|
| **LeetCode** | Algoritmos y estructuras | Entrevistas técnicas |
| **HackerRank** | Challenges variados | Práctica general |
| **Codewars** | Kata progresivos | Mejora gradual |
| **CodinGame** | Gamificación | Aprendizaje divertido |
| **AtCoder** | Competencia | Nivel avanzado |

---

### 🚀 **Tu Roadmap de Crecimiento**

#### 📈 **Plan de 6 Meses**

```javascript
const roadmapEstructuras = {
    mes1_2: {
        titulo: "🏗️ Consolidación de Fundamentos",
        objetivos: [
            "Dominar todos los métodos de Array",
            "Implementar Stack y Queue desde cero",
            "Resolver 20 ejercicios básicos"
        ],
        recursos: ["MDN docs", "freeCodeCamp", "JavaScript.info"]
    },
    
    mes3_4: {
        titulo: "⚡ Algoritmos y Optimización", 
        objetivos: [
            "Implementar algoritmos de ordenamiento",
            "Analizar complejidad Big O",
            "Usar Map/Set en proyectos reales"
        ],
        recursos: ["VisuAlgo", "LeetCode easy", "Proyectos personales"]
    },
    
    mes5_6: {
        titulo: "🌟 Estructuras Avanzadas",
        objetivos: [
            "Implementar árboles binarios", 
            "Crear grafos simples",
            "Completar proyecto integrador"
        ],
        recursos: ["CLRS book", "LeetCode medium", "Contribuir a open source"]
    }
};

// 🎯 Meta final
const metaFinal = {
    objetivo: "Ser desarrollador competente en estructuras de datos",
    indicadores: [
        "Elegir la estructura correcta para cada problema",
        "Implementar algoritmos eficientes",
        "Pasar entrevistas técnicas con confianza",
        "Contribuir a proyectos open source"
    ]
};

console.log("🚀 Tu journey hacia la maestría en estructuras de datos comienza aquí");
```

---

### 🎯 **Próximos Temas Recomendados**

Después de dominar estructuras de datos, tu siguiente paso natural es:

1. **🌐 JavaScript Moderno (ES6+)**
   - Async/await y Promises
   - Modules y bundling
   - Destructuring avanzado

2. **⚛️ Frameworks Frontend**
   - React con hooks
   - Vue.js composition API
   - State management (Redux, Vuex)

3. **🗄️ Bases de Datos**
   - MongoDB (documentos)
   - PostgreSQL (relacional)
   - Redis (cache/sesiones)

4. **🔧 Node.js y Backend**
   - APIs RESTful
   - GraphQL
   - Microservicios

---

### 🎊 **Mensaje Final**

```javascript
const mensajeFinal = {
    felicitaciones: "¡Has completado un journey increíble! 🎉",
    logros: [
        "Dominio de estructuras de datos fundamentales",
        "Conocimiento de algoritmos y complejidad",
        "Capacidad para resolver problemas complejos", 
        "Base sólida para tecnologías avanzadas"
    ],
    siguiente_nivel: {
        mensaje: "Las estructuras de datos son la base, pero ahora comes lo divertido",
        consejo: "Aplica lo aprendido en proyectos reales",
        mentalidad: "Nunca dejes de practicar y experimentar"
    }
};

console.log("🚀 El conocimiento que has adquirido te acompañará toda la vida");
console.log("💡 Cada problema que resuelvas te hará más fuerte");
console.log("🌟 ¡Sigue creciendo y nunca pares de aprender!");
```

---

**🎯 ¿Listo para el siguiente nivel?**

[🔜 **JavaScript Moderno**](../03-javascript-moderno/) | [🏠 **Volver al Inicio**](../../../README.md) | [📚 **Explorar Más Temas**](../../../NAVEGACION-DOCUMENTOS.md)

---

## 📚 **RECURSOS COMPLETOS**

### 🎯 **Para Profundizar tu Aprendizaje**

- **📝 [Cheatsheet Visual](./CHEATSHEET-VISUAL.md)** - Referencia rápida de estructuras de datos en JavaScript
- **🧪 [20 Ejercicios Prácticos](./ejercicios-practicos/README-EJERCICIOS.md)** - Práctica estructurada por niveles
- **🚀 [Proyectos Guiados](./proyectos-guiados/)** - Aplicación práctica de estructuras de datos
  - [📊 Gestor de Lista de Tareas](./proyectos-guiados/01-gestor-lista-tareas.md)
  - [📱 Libreta de Contactos](./proyectos-guiados/02-libreta-contactos.md)
  - [📈 Analizador de Datos](./proyectos-guiados/03-analizador-datos.md)
  - [📦 Sistema de Inventario](./proyectos-guiados/04-sistema-inventario.md)
  - [🔍 Motor de Búsqueda](./proyectos-guiados/05-motor-busqueda.md)

### 🔧 **Herramientas y Recursos Adicionales**
- **�️ Herramientas de análisis** - Chrome DevTools, Performance profilers
- **🌐 Comunidades** - Stack Overflow, JavaScript community
- **📖 Documentación especializada** - Array methods, Object techniques, Algorithm analysis

---

*�💡 Recuerda: El dominio de estructuras de datos no es un destino, es un journey continuo. ¡Cada día hay algo nuevo que aprender y optimizar!*

[🔙 **Volver al Índice Principal**](../../../README.md) | [📚 **Navegación Completa**](../../../NAVEGACION-DOCUMENTOS.md) | [📝 **Ver Cheatsheet**](CHEATSHEET-VISUAL.md) | [🧪 **Ejercicios Prácticos**](ejercicios-practicos/README-EJERCICIOS.md)
