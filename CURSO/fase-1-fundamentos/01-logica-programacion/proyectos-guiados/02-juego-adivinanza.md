[🏠 **Volver al Índice de Navegación**](../../../../NAVEGACION-DOCUMENTOS.md)

---

# 🎯 Juego de Adivinanza - Proyecto de Lógica

## 📝 **Descripción del Proyecto**
Crear un juego donde el programa genere un número aleatorio y el usuario deba adivinarlo usando bucles, condicionales y lógica de control.

---

## 🎯 **Objetivos de Aprendizaje**
- Dominar **bucles while** y control de iteraciones
- Usar **Math.random()** para generar números aleatorios
- Aplicar **condicionales anidadas** para diferentes casos
- Implementar **contadores y acumuladores**
- Practicar **entrada y salida de datos**

---

## 🔧 **Funcionalidades Requeridas**

### ✅ **Mecánica Básica**
- Generar **número aleatorio** entre 1 y 100
- **Pedir al usuario** que ingrese su adivinanza
- **Dar pistas**: "Muy alto", "Muy bajo", "¡Correcto!"
- **Contar intentos** realizados

### ✅ **Lógica de Juego**
- **Validar entrada**: Solo números del 1 al 100
- **Bucle principal**: Continuar hasta adivinanza correcta
- **Mostrar estadísticas**: Número de intentos al final
- **Opción de jugar de nuevo**

### ✅ **Mejoras Opcionales**
- **Sistema de puntuación** basado en intentos
- **Diferentes niveles** de dificultad (rangos de números)
- **Historial de intentos** del jugador

---

## 📋 **Estructura Esperada**

```javascript
// Función para generar número aleatorio
function generarNumeroAleatorio(min, max) { /* tu código */ }

// Función para validar entrada del usuario
function validarEntrada(numero) { /* tu código */ }

// Función principal del juego
function juegoAdivinanza() {
    // Generar número secreto
    // Inicializar contador de intentos
    // Bucle principal del juego
    // Mostrar resultado final
}

// Función para jugar de nuevo
function preguntarJugarDeNuevo() { /* tu código */ }

// Iniciar el juego
juegoAdivinanza();
```

---

## 🧪 **Flujo de Juego Esperado**

```
🎯 ¡Bienvenido al Juego de Adivinanza!
He pensado un número entre 1 y 100.

Intento 1: ¿Cuál es tu adivinanza? 50
🔽 El número es más bajo

Intento 2: ¿Cuál es tu adivinanza? 25  
🔼 El número es más alto

Intento 3: ¿Cuál es tu adivinanza? 37
🎉 ¡Correcto! El número era 37
✨ Lo lograste en 3 intentos

¿Quieres jugar de nuevo? (s/n)
```

---

## 🧠 **Conceptos Clave a Aplicar**

### 🔄 **Bucles**
```javascript
while (numeroSecreto !== adivinanza) {
    // Lógica del juego
}
```

### 🎲 **Números Aleatorios**
```javascript
const numeroSecreto = Math.floor(Math.random() * 100) + 1;
```

### 🔍 **Condicionales Múltiples**
```javascript
if (adivinanza < numeroSecreto) {
    console.log("🔼 El número es más alto");
} else if (adivinanza > numeroSecreto) {
    console.log("🔽 El número es más bajo");
} else {
    console.log("🎉 ¡Correcto!");
}
```

---

## ⏱️ **Tiempo Estimado**
**1.5-2.5 horas** (incluyendo mejoras opcionales)

## 🎓 **Nivel de Dificultad**
🟢 **BÁSICO-INTERMEDIO** - Perfecto para practicar bucles

---

## 💡 **Pistas para Empezar**

1. **Empieza con lo básico**: Genera el número y pide una adivinanza
2. **Añade el bucle**: Usa `while` para repetir hasta acertar  
3. **Implementa las pistas**: Compara y da feedback
4. **Cuenta los intentos**: Usa un contador que se incremente
5. **Valida entradas**: Asegúrate de que sean números válidos

---

**🚀 ¡Este proyecto te ayudará a dominar bucles y lógica condicional de forma divertida!**

---

[🔙 **Volver al Libro Principal**](../LOGICA-PROGRAMACION-LIBRO.md) | [🏠 **Índice General**](../../../../README.md) | [📚 **Navegación**](../../../../NAVEGACION-DOCUMENTOS.md) | [📝 **Ver Cheatsheet**](../CHEATSHEET-VISUAL.md)
