[🏠 **Volver al Índice de Navegación**](../../../NAVEGACION-DOCUMENTOS.md)

---

# 🐙 Git & GitHub - Guía Esencial para Desarrolladores

## 📝 **Introducción**

**Git** es el sistema de control de versiones más popular del mundo. **GitHub** es la plataforma que aloja repositorios Git y facilita la colaboración entre desarrolladores.

Esta guía te enseñará los **conceptos y comandos esenciales** que necesitas como desarrollador JavaScript.

---

## 🎯 **¿Por qué usar Git?**

### ✅ **Beneficios del Control de Versiones**
- 📚 **Historial completo** de cambios en tu código
- 🔄 **Recuperación** de versiones anteriores
- 🌿 **Trabajo en paralelo** con branches
- 👥 **Colaboración** efectiva en equipo
- 🔒 **Respaldo** automático en la nube
- 📊 **Seguimiento** de quién cambió qué y cuándo

### 🏗️ **Conceptos Fundamentales**
- **Repositorio**: Carpeta con historial de cambios
- **Commit**: Snapshot de tu código en un momento específico
- **Branch**: Línea de desarrollo independiente
- **Remote**: Versión del repositorio en servidor (GitHub)
- **Clone**: Copia local de un repositorio remoto
- **Pull Request**: Solicitud para fusionar cambios

---

## ⚙️ **Configuración Inicial**

### **1. Instalación de Git**
```bash
# Verificar si Git está instalado
git --version

# Ubuntu/Debian
sudo apt install git

# macOS (con Homebrew)
brew install git

# Windows: Descargar desde git-scm.com
```

### **2. Configuración Global**
```bash
# Configurar nombre y email (requerido)
git config --global user.name "Tu Nombre"
git config --global user.email "tu.email@ejemplo.com"

# Configurar editor por defecto
git config --global core.editor "code --wait"

# Ver configuración actual
git config --list
```

### **3. SSH Keys para GitHub (Recomendado)**
```bash
# Generar nueva SSH key
ssh-keygen -t ed25519 -C "tu.email@ejemplo.com"

# Agregar SSH key al agente
eval "$(ssh-agent -s)"
ssh-add ~/.ssh/id_ed25519

# Copiar clave pública para GitHub
cat ~/.ssh/id_ed25519.pub
```

Luego pega la clave en: **GitHub → Settings → SSH and GPG keys → New SSH key**

---

## 🚀 **Comandos Esenciales**

### **📁 Inicializar Repositorio**
```bash
# Crear nuevo repositorio
git init
git init nombre-proyecto

# Clonar repositorio existente
git clone https://github.com/usuario/repositorio.git
git clone git@github.com:usuario/repositorio.git  # SSH
```

### **📝 Flujo Básico de Trabajo**
```bash
# 1. Ver estado actual
git status

# 2. Agregar archivos al staging area
git add archivo.js
git add .                    # Todos los archivos
git add src/                 # Carpeta específica

# 3. Crear commit
git commit -m "Mensaje descriptivo del cambio"
git commit -am "Mensaje"     # Add + commit archivos modificados

# 4. Ver historial
git log
git log --oneline           # Formato compacto
git log --graph             # Ver branches visualmente
```

### **📊 Información y Diferencias**
```bash
# Ver diferencias
git diff                    # Cambios no staged
git diff --staged          # Cambios staged
git diff HEAD~1            # Comparar con commit anterior

# Ver detalles de commit
git show
git show commit-hash       # Commit específico

# Ver archivos en commit
git ls-files
```

---

## 🌿 **Trabajo con Branches**

### **🌱 Gestión de Ramas**
```bash
# Ver branches
git branch                  # Locales
git branch -a              # Todos (locales + remotos)

# Crear branch
git branch nueva-funcionalidad
git checkout -b nueva-funcionalidad  # Crear y cambiar

# Cambiar de branch
git checkout main
git switch main            # Comando más nuevo

# Eliminar branch
git branch -d nombre-branch
git branch -D nombre-branch  # Forzar eliminación
```

### **🔄 Fusionar Cambios**
```bash
# Merge (fusionar)
git checkout main
git merge nueva-funcionalidad

# Rebase (reorganizar historial)
git checkout nueva-funcionalidad
git rebase main
```

---

## 🐙 **GitHub: Repositorios Remotos**

### **🔗 Configurar Remotes**
```bash
# Ver remotos configurados
git remote -v

# Agregar remote
git remote add origin git@github.com:usuario/repo.git

# Cambiar URL de remote
git remote set-url origin nueva-url
```

### **⬆️⬇️ Sincronización**
```bash
# Subir cambios
git push origin main
git push -u origin main     # Primera vez (set upstream)

# Descargar cambios
git pull origin main        # Fetch + merge
git fetch origin           # Solo descarga, no fusiona

# Subir nuevo branch
git push -u origin nueva-funcionalidad
```

### **🍴 Fork y Pull Requests**
1. **Fork**: Copia el repositorio a tu cuenta GitHub
2. **Clone**: Descarga tu fork localmente
3. **Branch**: Crea rama para tu funcionalidad
4. **Commit**: Realiza tus cambios
5. **Push**: Sube cambios a tu fork
6. **Pull Request**: Solicita fusionar en repositorio original

---

## 🚨 **Comandos de Emergencia**

### **↩️ Deshacer Cambios**
```bash
# Descartar cambios en archivo
git checkout -- archivo.js
git restore archivo.js      # Comando más nuevo

# Quitar archivo del staging area
git reset HEAD archivo.js
git restore --staged archivo.js

# Deshacer último commit (mantener cambios)
git reset --soft HEAD~1

# Deshacer último commit (perder cambios)
git reset --hard HEAD~1

# Revertir commit (crear nuevo commit que deshaga)
git revert commit-hash
```

### **💾 Stash (Guardado Temporal)**
```bash
# Guardar cambios temporalmente
git stash
git stash save "Mensaje descriptivo"

# Ver stashes guardados
git stash list

# Recuperar último stash
git stash pop
git stash apply            # Mantener stash guardado

# Eliminar stash
git stash drop
git stash clear           # Eliminar todos
```

---

## 📁 **Archivo .gitignore Esencial**

Crea un archivo `.gitignore` en la raíz de tu proyecto:

```gitignore
# Dependencies
node_modules/
npm-debug.log*
yarn-debug.log*
yarn-error.log*

# Environment variables
.env
.env.local
.env.development.local
.env.test.local
.env.production.local

# Build outputs
dist/
build/
.next/
out/

# IDE/Editor files
.vscode/
.idea/
*.swp
*.swo
*~

# OS generated files
.DS_Store
.DS_Store?
._*
.Spotlight-V100
.Trashes
ehthumbs.db
Thumbs.db

# Logs
logs
*.log

# Runtime data
pids
*.pid
*.seed
*.pid.lock

# Coverage directory used by tools like istanbul
coverage/
*.lcov

# Temporary folders
tmp/
temp/
```

---

## 🛠️ **Flujo de Trabajo Recomendado**

### **🔄 Workflow para Proyectos Personales**
```bash
# 1. Inicializar proyecto
git init
git add .
git commit -m "Initial commit"

# 2. Conectar con GitHub
git remote add origin git@github.com:tu-usuario/tu-proyecto.git
git push -u origin main

# 3. Desarrollar funcionalidad
git checkout -b nueva-funcionalidad
# ... hacer cambios ...
git add .
git commit -m "Implementar nueva funcionalidad"

# 4. Fusionar a main
git checkout main
git merge nueva-funcionalidad
git push origin main

# 5. Limpiar
git branch -d nueva-funcionalidad
```

### **👥 Workflow para Equipos**
```bash
# 1. Clonar proyecto
git clone git@github.com:empresa/proyecto.git
cd proyecto

# 2. Crear branch para feature
git checkout -b feature/login-usuario

# 3. Desarrollar y commitear
git add .
git commit -m "Implementar sistema de login"

# 4. Subir branch
git push -u origin feature/login-usuario

# 5. Crear Pull Request en GitHub
# 6. Después de review y merge, actualizar main local
git checkout main
git pull origin main
git branch -d feature/login-usuario
```

---

## ✅ **Buenas Prácticas**

### **📝 Mensajes de Commit**
```bash
# ✅ Buenos mensajes
git commit -m "Agregar validación de email en formulario de registro"
git commit -m "Corregir error de cálculo en carrito de compras"
git commit -m "Actualizar dependencias de seguridad"

# ❌ Malos mensajes
git commit -m "cambios"
git commit -m "fix"
git commit -m "wip"
```

### **🌿 Estrategia de Branches**
- **main/master**: Código estable y listo para producción
- **develop**: Integración de nuevas funcionalidades
- **feature/**: Desarrollo de funcionalidades específicas
- **bugfix/**: Corrección de errores
- **hotfix/**: Correcciones urgentes en producción

### **🔒 Seguridad**
- ❌ **Nunca** subas contraseñas, API keys o datos sensibles
- ✅ Usa variables de entorno (`.env`) 
- ✅ Configura `.gitignore` correctamente
- ✅ Revisa cambios antes de commitear con `git diff`

---

## 🎯 **Comandos Rápidos para el Día a Día**

```bash
# Status rápido
git status -s

# Ver últimos commits
git log --oneline -10

# Agregar todos los cambios y commitear
git commit -am "Mensaje"

# Push rápido
git push

# Pull con rebase (historial más limpio)
git pull --rebase

# Ver diferencias con herramienta visual
git difftool

# Buscar en historial
git log --grep="palabra"
git log -S "función"      # Buscar cambios en código
```

---

## 🎓 **Próximos Pasos**

Una vez domines estos conceptos básicos, puedes explorar:

- **GitHub Actions**: Automatización y CI/CD
- **Git Hooks**: Scripts automáticos en eventos Git
- **GitHub Pages**: Hosting gratuito para sitios estáticos
- **Issues y Projects**: Gestión de tareas en GitHub
- **Git LFS**: Manejo de archivos grandes
- **Conventional Commits**: Estándar para mensajes de commit

---

## 📚 **Recursos Adicionales**

- 📖 [Git Documentation](https://git-scm.com/docs)
- 🎮 [Learn Git Branching](https://learngitbranching.js.org/)
- 📝 [GitHub Guides](https://guides.github.com/)
- 🔧 [Git Cheat Sheet](./CHEATSHEET-GIT-COMANDOS.md)

---

[📋 **Ver Cheat Sheet de Comandos**](./CHEATSHEET-GIT-COMANDOS.md) | [🏠 **Navegación**](../../../NAVEGACION-DOCUMENTOS.md)
