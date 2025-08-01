[🏠 **Volver al Índice de Navegación**](../../../NAVEGACION-DOCUMENTOS.md)

---

# 🔍 Motor de Búsqueda - Proyecto de Estructuras de Datos

## 📝 **Descripción del Proyecto**
Crear un motor de búsqueda inteligente que indexe documentos, implemente algoritmos de búsqueda avanzados, calcule relevancia de resultados y optimice performance utilizando todas las estructuras de datos aprendidas.

---

## 🎯 **Objetivos de Aprendizaje**
- Dominar **algoritmos de búsqueda** (lineal, binaria, interpolación)
- Implementar **indexación avanzada** con estructuras híbridas
- Practicar **scoring y ranking** de resultados
- Usar **optimización de performance** extrema
- Combinar **todas las estructuras** en un sistema complejo

---

## 🔧 **Funcionalidades Requeridas**

### ✅ **Indexación de Documentos**
- 📄 **Procesar documentos** y extraer términos
- 🏷️ **Crear índice invertido** para búsqueda rápida
- 🔤 **Normalizar texto** (minúsculas, sin acentos, stemming)
- 📊 **Calcular frecuencias** de términos (TF-IDF)

### ✅ **Algoritmos de Búsqueda**
- 🔍 **Búsqueda exacta** en índices
- 🎯 **Búsqueda fuzzy** (tolerancia a errores)
- 📝 **Búsqueda por frase** completa
- 🔗 **Búsqueda booleana** (AND, OR, NOT)

### ✅ **Ranking y Relevancia**
- ⭐ **Calcular score** de relevancia por documento
- 📈 **Ordenar resultados** por puntuación
- 🎯 **Highlighting** de términos encontrados
- 📊 **Estadísticas de búsqueda** (tiempo, resultados)

### ✅ **Optimización Avanzada**
- ⚡ **Cache de consultas** frecuentes
- 🗂️ **Índices múltiples** para diferentes tipos de búsqueda
- 🔄 **Sugerencias automáticas** (autocompletado)
- 📱 **Paginación** de resultados

---

## 📋 **Estructura Esperada**

```javascript
// Estructuras principales del motor
const documentos = new Map();           // id → documento completo
const indiceInvertido = new Map();      // término → Set(documentos)
const frecuenciaTerminos = new Map();   // término → Map(docId → frecuencia)
const metadatosDoc = new WeakMap();     // documento → metadatos

// Estructuras de optimización
const cacheConsultas = new Map();      // consulta → resultados
const indicePrefijos = new Map();       // prefijo → Set(términos)
const sugerencias = new Map();         // término → Array(sugerencias)

// Arrays para algoritmos de ordenamiento
let documentosOrdenados = [];          // Para búsqueda binaria
let terminosPopulares = [];            // Para autocompletado

// Funciones de indexación
function agregarDocumento(id, titulo, contenido, metadatos) { /* tu código */ }
function procesarTexto(texto) { /* tu código */ }
function construirIndiceInvertido() { /* tu código */ }
function calcularTFIDF(termino, documentoId) { /* tu código */ }

// Funciones de búsqueda básica
function busquedaExacta(termino) { /* tu código */ }
function busquedaFuzzy(termino, distancia = 2) { /* tu código */ }
function busquedaFrase(frase) { /* tu código */ }
function busquedaBooleana(expresion) { /* tu código */ }

// Funciones de ranking
function calcularScore(terminos, documentoId) { /* tu código */ }
function ordenarResultados(resultados) { /* tu código */ }
function resaltarTerminos(texto, terminos) { /* tu código */ }
function paginarResultados(resultados, pagina, tamano) { /* tu código */ }

// Funciones de optimización
function buscarEnCache(consulta) { /* tu código */ }
function guardarEnCache(consulta, resultados) { /* tu código */ }
function generarSugerencias(prefijo) { /* tu código */ }
function autocompletar(texto) { /* tu código */ }

// Algoritmos de búsqueda avanzados
function busquedaBinariaPorScore(minScore) { /* tu código */ }
function busquedaInterpolada(termino) { /* tu código */ }
function distanciaLevenshtein(str1, str2) { /* tu código */ }

// Función principal del motor
function motorBusqueda() {
    // Cargar documentos de ejemplo
    // Construir todos los índices
    // Mostrar interfaz de búsqueda
    // Procesar consultas del usuario
}

// Ejecutar motor
motorBusqueda();
```

---

## 🧪 **Casos de Prueba**

Asegúrate de que tu motor maneje estos casos:

```javascript
// Indexación de documentos
agregarDocumento("DOC001", "JavaScript Avanzado", 
    "JavaScript es un lenguaje de programación versátil para desarrollo web",
    {autor: "Juan Pérez", fecha: "2024-01-15"}
) → Documento indexado correctamente

procesamrTexto("JavaScript es genial!") → ["javascript", "es", "genial"]
indiceInvertido.get("javascript") → Set(["DOC001", "DOC002", ...])

// Búsquedas básicas
busquedaExacta("javascript") → Array de documentos que contienen "javascript"
busquedaFuzzy("javscript", 2) → Encuentra "javascript" (error de 1 carácter)
busquedaFrase("lenguaje de programación") → Documentos con esa frase exacta

// Búsqueda booleana
busquedaBooleana("javascript AND web") → Documentos con ambos términos
busquedaBooleana("python OR javascript") → Documentos con cualquier término
busquedaBooleana("web NOT php") → Documentos con "web" pero sin "php"

// Ranking y relevancia
calcularScore(["javascript", "web"], "DOC001") → 0.85 (score de relevancia)
ordenarResultados(resultados) → Array ordenado por score descendente
resaltarTerminos("JavaScript es genial", ["javascript"]) → "<mark>JavaScript</mark> es genial"

// Optimización
buscarEnCache("javascript web") → Resultados del cache si existen
generarSugerencias("java") → ["javascript", "java", "javadoc"]
autocompletar("progra") → ["programación", "programador", "programa"]

// Algoritmos avanzados
distanciaLevenshtein("javascript", "javscript") → 1 (una diferencia)
busquedaBinariaPorScore(0.5) → Documentos con score >= 0.5
busquedaInterpolada("web") → Posición estimada en índice ordenado

// Estadísticas
obtenerEstadisticas() → {
    totalDocumentos: 100,
    totalTerminos: 5000,
    consultasCache: 25,
    tiempoPromedio: "15ms"
}

// Casos especiales
busquedaExacta("") → "Error: Consulta vacía"
busquedaFuzzy("x", 0) → Solo coincidencias exactas
busquedaBooleana("(web AND") → "Error: Expresión booleana inválida"
```

---

## 💾 **Estructura de Datos Sugerida**

```javascript
// Estructura de documento
const documentoEjemplo = {
    id: "DOC001",
    titulo: "JavaScript Avanzado",
    contenido: "JavaScript es un lenguaje de programación...",
    autor: "Juan Pérez",
    fecha: new Date("2024-01-15"),
    url: "https://ejemplo.com/js-avanzado",
    categoria: "Programming",
    idioma: "es",
    longitudPalabras: 150
};

// Estructura del índice invertido
const indiceEjemplo = new Map([
    ["javascript", new Set(["DOC001", "DOC003", "DOC007"])],
    ["programacion", new Set(["DOC001", "DOC002", "DOC005"])],
    ["web", new Set(["DOC001", "DOC004", "DOC006"])]
]);

// Estructura TF-IDF
const tfidfEjemplo = new Map([
    ["javascript", new Map([
        ["DOC001", 0.85],
        ["DOC003", 0.72],
        ["DOC007", 0.91]
    ])]
]);

// Estructura de resultado
const resultadoEjemplo = {
    documento: documentoEjemplo,
    score: 0.85,
    terminosEncontrados: ["javascript", "web"],
    fragmentos: ["...JavaScript es un <mark>lenguaje</mark> de..."],
    posicionesTerminos: [0, 25, 67]
};

// Cache de consultas
const cacheEjemplo = new Map([
    ["javascript web", {
        resultados: [resultadoEjemplo],
        timestamp: Date.now(),
        numeroResultados: 1
    }]
]);
```

---

## ⏱️ **Tiempo Estimado**
**4-5 horas** (dependiendo de tu nivel)

## 🎓 **Nivel de Dificultad**
🟣 **DESAFÍO** - Integra todos los conceptos del curso en un proyecto complejo

---

## 💡 **Pistas para Empezar**

1. **Comienza con indexación simple**: Un Map de término → Array de documentos
2. **Normaliza el texto**: Convierte a minúsculas, elimina acentos y puntuación
3. **Implementa TF-IDF gradualmente**: Empieza con frecuencia simple
4. **Usa Set para intersecciones**: Perfecto para búsquedas AND/OR
5. **Cache las consultas frecuentes**: Map con timestamp para invalidación
6. **Implementa paginación**: No retornes miles de resultados de una vez
7. **Optimiza incrementalmente**: Primero que funcione, luego que sea rápido

---

## 🎯 **Conceptos Clave que Practicarás**

- **Índice invertido** - Map de términos a documentos
- **TF-IDF scoring** - Cálculo de relevancia estadística
- **Set operations** - Intersecciones, uniones para búsqueda booleana
- **Binary search** - Búsqueda en arrays ordenados por score
- **Levenshtein distance** - Algoritmo para búsqueda fuzzy
- **Caching strategies** - Map con TTL para optimización
- **Text normalization** - Procesamiento de strings
- **Performance optimization** - Elegir estructuras por velocidad

---

## 🔍 **Algoritmos Avanzados Sugeridos**

```javascript
// Ejemplos de implementaciones complejas que puedes intentar:

// Algoritmo TF-IDF completo
function calcularTFIDF(termino, documentoId) {
    const documento = documentos.get(documentoId);
    const palabrasDoc = procesarTexto(documento.contenido);
    
    // Term Frequency
    const tf = palabrasDoc.filter(p => p === termino).length / palabrasDoc.length;
    
    // Inverse Document Frequency
    const docConTermino = indiceInvertido.get(termino)?.size || 0;
    const idf = Math.log(documentos.size / (1 + docConTermino));
    
    return tf * idf;
}

// Búsqueda booleana con parser
function busquedaBooleana(expresion) {
    // Parsear expresión: "web AND (javascript OR python) NOT php"
    const tokens = tokenizarExpresion(expresion);
    const arbolExpresion = construirArbolBooleano(tokens);
    return evaluarArbolBooleano(arbolExpresion);
}

// Autocompletado inteligente
function autocompletarInteligente(prefijo) {
    const candidatos = Array.from(indicePrefijos.get(prefijo) || []);
    
    return candidatos
        .map(termino => ({
            termino,
            popularidad: frecuenciaTerminos.get(termino)?.size || 0,
            distancia: calcularDistanciaEdicion(prefijo, termino)
        }))
        .sort((a, b) => b.popularidad - a.popularidad || a.distancia - b.distancia)
        .slice(0, 10)
        .map(c => c.termino);
}

// Sistema de cache inteligente con LRU
class CacheResultados {
    constructor(maxSize = 1000, ttl = 300000) { // 5 minutos TTL
        this.cache = new Map();
        this.maxSize = maxSize;
        this.ttl = ttl;
    }
    
    get(consulta) {
        const item = this.cache.get(consulta);
        if (!item) return null;
        
        if (Date.now() - item.timestamp > this.ttl) {
            this.cache.delete(consulta);
            return null;
        }
        
        // Mover al final (LRU)
        this.cache.delete(consulta);
        this.cache.set(consulta, item);
        return item.resultados;
    }
    
    set(consulta, resultados) {
        if (this.cache.size >= this.maxSize) {
            const firstKey = this.cache.keys().next().value;
            this.cache.delete(firstKey);
        }
        
        this.cache.set(consulta, {
            resultados,
            timestamp: Date.now()
        });
    }
}
```

---

## 📊 **Métricas de Performance Esperadas**

```javascript
// Tu motor debería lograr estas métricas aproximadas:
const metricasObjetivo = {
    indexacion: "< 100ms por documento",
    busquedaExacta: "< 10ms para índices de 10k términos",
    busquedaFuzzy: "< 50ms para distancia <= 2", 
    cache: "< 1ms para consultas cacheadas",
    memoria: "< 50MB para 1000 documentos",
    precision: "> 85% para búsquedas relevantes"
};
```

---

**🚀 ¡Cuando termines, tendrás un motor de búsqueda funcional y habrás aplicado TODAS las estructuras de datos y algoritmos del curso en un proyecto de nivel profesional!**

---

[🔙 **Volver al Libro Principal**](../ESTRUCTURAS-DATOS-LIBRO.md) | [🏠 **Índice General**](../../../README.md) | [📚 **Navegación**](../../../NAVEGACION-DOCUMENTOS.md) | [📝 **Ver Cheatsheet**](../CHEATSHEET-VISUAL.md)
