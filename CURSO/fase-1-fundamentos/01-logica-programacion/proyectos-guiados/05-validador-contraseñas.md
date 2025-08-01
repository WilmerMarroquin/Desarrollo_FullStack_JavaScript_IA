[🏠 **Volver al Índice de Navegación**](../../../NAVEGACION-DOCUMENTOS.md)

---

# 🔐 Validador de Contraseñas - Proyecto de Lógica

## 📝 **Descripción del Proyecto**
Crear un sistema que valide contraseñas según diferentes criterios de seguridad, usando funciones, expresiones regulares básicas y lógica condicional compleja.

---

## 🎯 **Objetivos de Aprendizaje**
- Aplicar **funciones de validación** múltiples
- Usar **métodos de string** para análisis de texto
- Implementar **lógica condicional compleja**
- Trabajar con **caracteres especiales** y **códigos ASCII**
- Crear **feedback detallado** para el usuario

---

## 🔧 **Funcionalidades Requeridas**

### ✅ **Criterios de Validación**
- **Longitud mínima**: 8 caracteres
- **Al menos una mayúscula** (A-Z)
- **Al menos una minúscula** (a-z)
- **Al menos un número** (0-9)
- **Al menos un carácter especial** (!@#$%^&*)

### ✅ **Análisis de Fortaleza**
- **Débil**: Cumple 1-2 criterios
- **Regular**: Cumple 3-4 criterios
- **Fuerte**: Cumple todos los criterios
- **Muy Fuerte**: Fuerte + longitud > 12 caracteres

### ✅ **Funcionalidades Extra**
- **Generar sugerencias** de mejora
- **Calcular tiempo estimado** para descifrar
- **Detectar patrones comunes** débiles
- **Mostrar progreso visual** de fortaleza

---

## 📋 **Estructura Esperada**

```javascript
// Funciones de validación individual
function tieneLongitudMinima(password) { /* tu código */ }
function tieneMayuscula(password) { /* tu código */ }
function tieneMinuscula(password) { /* tu código */ }
function tieneNumero(password) { /* tu código */ }
function tieneCaracterEspecial(password) { /* tu código */ }

// Función que evalúa fortaleza general
function evaluarFortaleza(password) { /* tu código */ }

// Función que genera sugerencias
function generarSugerencias(password) { /* tu código */ }

// Función principal
function validadorContraseñas() {
    // Pedir contraseña al usuario
    // Ejecutar todas las validaciones
    // Mostrar resultados y sugerencias
}

// Iniciar el validador
validadorContraseñas();
```

---

## 🧪 **Ejemplo de Funcionamiento**

```
🔐 VALIDADOR DE CONTRASEÑAS

Ingresa la contraseña a validar: abc123

📊 RESULTADOS DE VALIDACIÓN:
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

✅ Criterios cumplidos:
├─ ❌ Longitud mínima (6/8 caracteres)
├─ ❌ Contiene mayúscula
├─ ✅ Contiene minúscula
├─ ✅ Contiene número
└─ ❌ Contiene carácter especial

🎯 FORTALEZA: 🔴 DÉBIL (2/5 criterios)
⏱️ Tiempo estimado para descifrar: < 1 segundo

💡 SUGERENCIAS DE MEJORA:
├─ Añade al menos 2 caracteres más
├─ Incluye una letra mayúscula (A-Z)
├─ Añade un carácter especial (!@#$%^&*)
└─ Evita secuencias obvias como "123"

¿Quieres validar otra contraseña? (s/n)
```

---

## 🧠 **Conceptos Clave a Aplicar**

### 🔍 **Análisis de Caracteres**
```javascript
function tieneMayuscula(password) {
    for (let i = 0; i < password.length; i++) {
        const char = password[i];
        if (char >= 'A' && char <= 'Z') {
            return true;
        }
    }
    return false;
}
```

### 🎯 **Métodos de String Útiles**
```javascript
password.length                    // Longitud
password.includes('caracter')      // Contiene carácter específico
password.charAt(i)                 // Carácter en posición i
```

### 🧮 **Lógica de Puntuación**
```javascript
function calcularPuntuacion(password) {
    let puntos = 0;
    if (tieneLongitudMinima(password)) puntos++;
    if (tieneMayuscula(password)) puntos++;
    if (tieneMinuscula(password)) puntos++;
    if (tieneNumero(password)) puntos++;
    if (tieneCaracterEspecial(password)) puntos++;
    return puntos;
}
```

---

## 🎨 **Feedback Visual**

```javascript
function mostrarBarraFortaleza(nivel) {
    const barras = {
        1: "🔴 ▓░░░░ DÉBIL",
        2: "🟠 ▓▓░░░ DÉBIL", 
        3: "🟡 ▓▓▓░░ REGULAR",
        4: "🟢 ▓▓▓▓░ FUERTE",
        5: "🟢 ▓▓▓▓▓ MUY FUERTE"
    };
    return barras[nivel] || barras[1];
}
```

---

## ⏱️ **Tiempo Estimado**
**2-4 horas** (incluyendo funcionalidades extra)

## 🎓 **Nivel de Dificultad**
🔴 **INTERMEDIO-AVANZADO** - Lógica compleja y múltiples validaciones

---

## 💡 **Pistas para Empezar**

1. **Una validación a la vez**: Empieza con longitud mínima
2. **Usa códigos ASCII**: Para verificar rangos de caracteres
3. **Prueba con casos extremos**: Contraseñas muy cortas, muy largas, etc.
4. **Haz feedback útil**: No solo "válida/inválida", sino cómo mejorar
5. **Organiza bien las funciones**: Cada validación debe ser independiente

---

## 🎯 **Algoritmo de Caracteres Especiales**

```javascript
function tieneCaracterEspecial(password) {
    const especiales = "!@#$%^&*()_+-=[]{}|;:,.<>?";
    for (let i = 0; i < password.length; i++) {
        if (especiales.includes(password[i])) {
            return true;
        }
    }
    return false;
}
```

---

## 🎯 **Desafío Extra (Opcional)**

- **Detectar patrones débiles**: "password123", "qwerty", etc.
- **Sugerir contraseñas seguras** automáticamente
- **Calcular entropía** de la contraseña
- **Verificar contra lista** de contraseñas más comunes

---

**🚀 ¡Este proyecto te dará experiencia sólida con validación de datos y lógica de seguridad!**

---

[🔙 **Volver al Libro Principal**](../LOGICA-PROGRAMACION-LIBRO.md) | [🏠 **Índice General**](../../../README.md) | [📚 **Navegación**](../../../NAVEGACION-DOCUMENTOS.md) | [📝 **Ver Cheatsheet**](../CHEATSHEET-VISUAL.md)
