# 🔧 Guía de Instalación y Configuración

## Prepara tu Entorno de Desarrollo para la Fase 1 - Fundamentos

> **🎯 "Un buen programador es solo tan bueno como sus herramientas. Configuremos el entorno perfecto para dominar los fundamentos."**

### 📚 **Esta guía te preparará para:**
- **🧠 01-logica-programacion** - Pensamiento computacional y algoritmos
- **📊 02-estructuras-datos** - Arrays, objetos y estructuras complejas  
- **🚀 03-javascript-moderno** - ES6+, módulos y características avanzadas
- **🔗 04-git-github** - Control de versiones y colaboración

---

## 🚀 **Instalación Rápida (5 minutos)**

### 1. 💻 **Node.js (Motor JavaScript)**

```bash
# Verificar si ya tienes Node.js
node --version

# Si no lo tienes, descarga desde:
# https://nodejs.org (versión LTS recomendada)
```

### 2. 🎨 **Visual Studio Code (Editor Recomendado)**

**📥 Descarga:** https://code.visualstudio.com/

**🔌 Extensiones Esenciales para Fase 1:**
```
- JavaScript (ES6) code snippets
- Bracket Pair Colorizer
- Live Server
- Prettier - Code formatter
- Error Lens
- Auto Rename Tag
- GitLens — Git supercharged
- Path Intellisense
```

### 3. 🌐 **Navegador con DevTools**
- **Chrome** (recomendado) o **Firefox**
- Asegúrate de saber abrir DevTools: `F12` o `Ctrl+Shift+I`

### 4. 🔗 **Git y GitHub (Esencial para Tema 4)**

#### 📥 **Instalación de Git**

**Windows:**
```bash
# Descarga Git para Windows desde:
# https://git-scm.com/download/win
# O usa chocolatey si lo tienes:
choco install git
```

**macOS:**
```bash
# Con Homebrew (recomendado):
brew install git

# O descarga desde: https://git-scm.com/download/mac
```

**Linux (Ubuntu/Debian):**
```bash
sudo apt update
sudo apt install git
```

**Verificar instalación:**
```bash
git --version
# Debería mostrar algo como: git version 2.x.x
```

#### ⚙️ **Configuración Inicial de Git**

```bash
# Configurar tu identidad (REQUERIDO)
git config --global user.name "Tu Nombre Completo"
git config --global user.email "tu.email@ejemplo.com"

# Configurar editor por defecto (opcional)
git config --global core.editor "code --wait"  # Para VS Code

# Verificar configuración
git config --list
```

#### 🐙 **Cuenta de GitHub**

1. **📝 Crear cuenta**: Ve a [github.com](https://github.com) y regístrate
2. **🔐 Configurar SSH** (recomendado para tema 4):
   ```bash
   # Generar clave SSH
   ssh-keygen -t ed25519 -C "tu.email@ejemplo.com"
   
   # Agregar a SSH agent
   eval "$(ssh-agent -s)"
   ssh-add ~/.ssh/id_ed25519
   
   # Copiar clave pública (para agregar en GitHub)
   cat ~/.ssh/id_ed25519.pub
   ```
3. **➕ Agregar clave SSH**: GitHub → Settings → SSH and GPG keys → New SSH key

#### ✅ **Verificar conexión con GitHub**
```bash
ssh -T git@github.com
# Debería responder: "Hi usuario! You've successfully authenticated..."
```

---

## ⚙️ **Configuración Detallada**

### 🎯 **VS Code Settings (Configuración Recomendada)**

Crea archivo: `.vscode/settings.json`

```json
{
  "editor.fontSize": 14,
  "editor.tabSize": 2,
  "editor.wordWrap": "on",
  "editor.minimap.enabled": true,
  "editor.suggestSelection": "first",
  "editor.bracketPairColorization.enabled": true,
  "editor.guides.bracketPairs": true,
  "javascript.suggest.autoImports": true,
  "javascript.updateImportsOnFileMove.enabled": "always",
  "files.autoSave": "afterDelay",
  "files.autoSaveDelay": 1000,
  "terminal.integrated.fontSize": 12,
  "workbench.colorTheme": "Dark+ (default dark)",
  "prettier.singleQuote": true,
  "prettier.semi": true
}
```

### 🎪 **Snippets Personalizados**

Archivo: `.vscode/javascript.json`

```json
{
  "Log to console": {
    "prefix": "cl",
    "body": [
      "console.log('$1:', $1);"
    ],
    "description": "Log output to console"
  },
  "Function": {
    "prefix": "fn",
    "body": [
      "function $1($2) {",
      "  $3",
      "}"
    ],
    "description": "Create function"
  },
  "Arrow Function": {
    "prefix": "af",
    "body": [
      "const $1 = ($2) => {",
      "  $3",
      "};"
    ],
    "description": "Create arrow function"
  }
}
```

---

## 🧪 **Verificación de Instalación**

### ✅ **Test Rápido**

Crea archivo: `test-setup.js`

```javascript
// 🧪 Test de configuración del entorno
console.log("🎉 ¡Node.js funcionando!");
console.log("📅 Fecha actual:", new Date().toLocaleDateString());
console.log("🖥️ Versión Node.js:", process.version);

// Test de características ES6+
const mensaje = `¡ES6+ funciona perfectamente!`;
const numeros = [1, 2, 3, 4, 5];
const pares = numeros.filter(n => n % 2 === 0);

console.log("✨", mensaje);
console.log("🔢 Números pares:", pares);

// Test de objetos y métodos
const desarrollador = {
  nombre: "Mi Nombre",
  habilidades: ["JavaScript", "Lógica", "Resolución de problemas"],
  presentarse() {
    return `¡Hola! Soy ${this.nombre} y domino: ${this.habilidades.join(", ")}`;
  }
};

console.log("👋", desarrollador.presentarse());
console.log("🚀 ¡Tu entorno está listo para programar!");
```

**🏃‍♂️ Ejecutar test:**
```bash
node test-setup.js
```

### ✅ **Test de Git y GitHub**

```bash
# Verificar instalaciones
echo "🔍 Verificando herramientas..."
node --version
git --version

# Test de Git
echo "📝 Configuración de Git:"
git config user.name
git config user.email

# Test de GitHub (si configuraste SSH)
echo "🐙 Conexión con GitHub:"
ssh -T git@github.com

# Test de repositorio local
echo "📂 Creando repo de prueba..."
mkdir test-git && cd test-git
git init
echo "# Test" > README.md
git add README.md
git commit -m "Primer commit"
echo "✅ Git funcionando correctamente!"
cd .. && rm -rf test-git
```

---

## 🔧 **Herramientas Adicionales Recomendadas**

### 🌐 **Navegador - DevTools**

**🔍 Consola JavaScript:**
- `F12` → Pestaña "Console"
- Prueba código JavaScript en tiempo real
- Depura errores fácilmente

**💡 Shortcuts útiles:**
- `Ctrl + Shift + I` - Abrir DevTools
- `Ctrl + Shift + C` - Inspeccionar elemento
- `Ctrl + Shift + J` - Ir directo a Console

### 📦 **Gestores de Paquetes (Opcional)**

```bash
# NPM (incluido con Node.js)
npm --version

# Yarn (alternativa)
npm install -g yarn
```

### 🎨 **Extensiones VS Code Avanzadas**

```
🔧 Herramientas:
- GitLens — Git supercharged
- REST Client (para APIs)
- Thunder Client (alternativa a Postman)

🎨 Visualización:
- Indent Rainbow
- Highlight Matching Tag
- Color Highlight

🚀 Productividad:
- Auto Close Tag
- Path Intellisense
- IntelliSense for CSS class names
```

---

## 🎯 **Configuración del Proyecto**

### 📁 **Estructura Recomendada para Fase 1**

```
fase-1-fundamentos/
├── 🧠 01-logica-programacion/
│   ├── ejercicios/
│   ├── proyectos/
│   └── notas-personales.md
├── 📊 02-estructuras-datos/
│   ├── ejercicios/
│   ├── proyectos/
│   └── notas-personales.md
├── 🚀 03-javascript-moderno/
│   ├── ejemplos/
│   ├── proyectos/
│   └── notas-personales.md
├── � 04-git-github/
│   ├── repositorios-practica/
│   └── comandos-frecuentes.md
└── � recursos-compartidos/
    └── utilidades-comunes.js
```

### 🎪 **Package.json para Fase 1**

```json
{
  "name": "fase-1-fundamentos-javascript",
  "version": "1.0.0",
  "description": "Mi práctica de fundamentos JavaScript - Fase 1",
  "main": "index.js",
  "scripts": {
    "start": "node index.js",
    "test": "node test-setup.js",
    "serve": "live-server"
  },
  "keywords": ["javascript", "fundamentos", "logica", "estructuras-datos", "es6", "git"],
  "author": "Tu Nombre",
  "license": "MIT"
}
```

---

## 🎉 **¡Listo para Empezar!**

### ✅ **Checklist Final:**

- [ ] ✅ Node.js instalado y funcionando
- [ ] 🎨 VS Code configurado con extensiones
- [ ] 🌐 Navegador con DevTools listo
- [ ] � Git instalado y configurado
- [ ] 🐙 GitHub account creado y SSH configurado
- [ ] �📁 Estructura de proyecto creada
- [ ] 🧪 Test de configuración ejecutado exitosamente
- [ ] 📚 Acceso a materiales de aprendizaje

### 🚀 **Próximos Pasos:**

1. **🎯 Ejecuta ambos tests** para verificar todo (Node.js y Git)
2. **📖 Empieza con Tema 1** - Lógica de Programación
3. **🧪 Ten el cheatsheet a mano** para consultas rápidas
4. **💻 Practica cada concepto** en VS Code inmediatamente
5. **🔗 Cuando llegues al Tema 4**, ya tendrás Git y GitHub listos

**🎊 ¡Tu entorno de desarrollo está perfecto para conquistar los 4 temas de la Fase 1!**

---

[🏠 **Volver a Fase 1**](./README.md) | [🧠 **Tema 1: Lógica**](./01-logica-programacion/LOGICA-PROGRAMACION-LIBRO.md) | [� **Tema 2: Estructuras**](./02-estructuras-datos/) | [🚀 **Tema 3: JS Moderno**](./03-javascript-moderno/) | [🔗 **Tema 4: Git**](./04-git-github/)
