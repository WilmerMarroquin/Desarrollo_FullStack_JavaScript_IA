[🏠 **Volver al Índice de Navegación**](../../../NAVEGACION-DOCUMENTOS.md)

---

# 📋 Git Commands - Cheat Sheet

## ⚙️ **Setup & Configuración**

```bash
# Configuración inicial (requerida)
git config --global user.name "Tu Nombre"
git config --global user.email "tu.email@ejemplo.com"

# Ver configuración
git config --list
git config user.name

# Configurar editor
git config --global core.editor "code --wait"
```

---

## 📁 **Básicos - Repositorio**

```bash
# Inicializar repositorio
git init
git init nombre-proyecto

# Clonar repositorio
git clone https://github.com/usuario/repo.git
git clone git@github.com:usuario/repo.git      # SSH

# Ver estado
git status
git status -s                                  # Formato corto
```

---

## 📝 **Básicos - Staging & Commits**

```bash
# Agregar archivos
git add archivo.js
git add .                                      # Todos los archivos
git add src/                                   # Carpeta específica
git add "*.js"                                 # Patrón de archivos

# Quitar del staging area
git reset HEAD archivo.js
git restore --staged archivo.js               # Nuevo comando

# Crear commit
git commit -m "Mensaje descriptivo"
git commit -am "Mensaje"                       # Add + commit archivos modificados
git commit --amend -m "Nuevo mensaje"         # Modificar último commit
```

---

## 📊 **Información & Historial**

```bash
# Ver historial
git log
git log --oneline                              # Formato compacto
git log --oneline -10                          # Últimos 10 commits
git log --graph                                # Ver branches visualmente
git log --grep="palabra"                       # Buscar en mensajes

# Ver diferencias
git diff                                       # Cambios no staged
git diff --staged                              # Cambios staged  
git diff HEAD~1                                # Comparar con commit anterior
git diff branch1..branch2                     # Entre branches

# Ver detalles de commit
git show
git show commit-hash
git show HEAD~2                                # Commit específico
```

---

## 🌿 **Branches (Ramas)**

```bash
# Ver branches
git branch                                     # Locales
git branch -a                                  # Todos (locales + remotos)
git branch -r                                  # Solo remotos

# Crear branch
git branch nueva-funcionalidad
git checkout -b nueva-funcionalidad            # Crear y cambiar
git switch -c nueva-funcionalidad              # Nuevo comando

# Cambiar de branch
git checkout main
git switch main                                # Nuevo comando

# Eliminar branch
git branch -d nombre-branch                    # Solo si está merged
git branch -D nombre-branch                    # Forzar eliminación

# Renombrar branch
git branch -m nuevo-nombre                     # Branch actual
git branch -m viejo-nombre nuevo-nombre       # Branch específico
```

---

## 🔄 **Merge & Rebase**

```bash
# Merge (fusionar)
git checkout main
git merge nueva-funcionalidad
git merge --no-ff nueva-funcionalidad          # Forzar merge commit

# Rebase (reorganizar historial)
git checkout nueva-funcionalidad
git rebase main
git rebase -i HEAD~3                           # Rebase interactivo

# Abortar merge/rebase
git merge --abort
git rebase --abort
```

---

## 🔗 **Remotos (GitHub)**

```bash
# Ver remotos
git remote -v
git remote show origin

# Agregar remote
git remote add origin git@github.com:usuario/repo.git
git remote add upstream git@github.com:original/repo.git

# Cambiar URL
git remote set-url origin nueva-url

# Eliminar remote
git remote remove nombre-remote
```

---

## ⬆️⬇️ **Sincronización**

```bash
# Push (subir)
git push origin main
git push -u origin main                        # Primera vez (set upstream)
git push --all origin                          # Todos los branches
git push origin --delete branch-name          # Eliminar branch remoto

# Pull (descargar + fusionar)
git pull origin main
git pull --rebase origin main                 # Con rebase

# Fetch (solo descargar)
git fetch origin
git fetch --all                                # Todos los remotos
```

---

## 🚨 **Deshacer Cambios**

```bash
# Descartar cambios en archivo
git checkout -- archivo.js
git restore archivo.js                         # Nuevo comando

# Descartar todos los cambios no staged
git checkout .
git restore .

# Deshacer commits (mantener cambios)
git reset --soft HEAD~1                       # Último commit
git reset --soft commit-hash                  # Hasta commit específico

# Deshacer commits (perder cambios)
git reset --hard HEAD~1                       # ⚠️ PELIGROSO
git reset --hard commit-hash

# Revertir commit (crear nuevo commit que deshaga)
git revert commit-hash
git revert HEAD                                # Último commit
```

---

## 💾 **Stash (Guardado Temporal)**

```bash
# Guardar cambios temporalmente
git stash
git stash save "Mensaje descriptivo"
git stash push -m "Mensaje" archivo.js         # Archivo específico

# Ver stashes
git stash list
git stash show                                 # Último stash
git stash show stash@{0}                       # Stash específico

# Recuperar stash
git stash pop                                  # Último stash (y eliminarlo)
git stash apply                                # Último stash (mantenerlo)
git stash apply stash@{0}                      # Stash específico

# Eliminar stash
git stash drop                                 # Último stash
git stash drop stash@{0}                       # Stash específico
git stash clear                                # Todos los stashes
```

---

## 🔍 **Búsqueda & Navegación**

```bash
# Buscar texto en archivos
git grep "función"
git grep -n "TODO"                            # Con números de línea

# Buscar cambios en código
git log -S "función"
git log -G "regex"

# Ver quién modificó líneas
git blame archivo.js
git blame -L 10,20 archivo.js                 # Líneas específicas

# Navegar por historial
git checkout commit-hash                       # Ir a commit específico
git checkout HEAD~2                            # 2 commits atrás
git checkout main                              # Volver a branch actual
```

---

## 🏷️ **Tags**

```bash
# Crear tag
git tag v1.0.0
git tag -a v1.0.0 -m "Versión 1.0.0"          # Tag con mensaje

# Ver tags
git tag
git tag -l "v1.*"                              # Con patrón

# Push tags
git push origin v1.0.0                        # Tag específico
git push origin --tags                        # Todos los tags

# Eliminar tag
git tag -d v1.0.0                              # Local
git push origin --delete v1.0.0               # Remoto
```

---

## 🔧 **Herramientas & Utilidades**

```bash
# Ver archivos ignorados
git ls-files --ignored --exclude-standard

# Limpiar archivos no tracked
git clean -n                                   # Mostrar qué se eliminará
git clean -f                                   # Eliminar archivos
git clean -fd                                  # Eliminar archivos y carpetas

# Configurar alias útiles
git config --global alias.st status
git config --global alias.co checkout
git config --global alias.br branch
git config --global alias.cm commit
git config --global alias.lg "log --oneline --graph"

# Usar alias
git st                                         # = git status
git lg                                         # = git log --oneline --graph
```

---

## 🎯 **Comandos de Un Solo Uso**

```bash
# Combo rápido para el día a día
git add . && git commit -m "Mensaje" && git push

# Ver estado, agregar todo y commitear
git status && git add . && git commit -m "Mensaje"

# Crear branch, cambiar y push en una línea
git checkout -b nueva-feature && git push -u origin nueva-feature

# Actualizar main y merge feature
git checkout main && git pull && git merge nueva-feature

# Ver últimos 5 commits en formato bonito
git log --oneline --graph -5

# Ver diferencias y agregar archivo interactivamente
git diff archivo.js && git add -p archivo.js
```

---

## 📚 **Patterns de Workflow**

### **🔄 Feature Branch Workflow**
```bash
# 1. Actualizar main
git checkout main && git pull origin main

# 2. Crear feature branch
git checkout -b feature/nueva-funcionalidad

# 3. Desarrollar
git add . && git commit -m "Implementar funcionalidad"

# 4. Push feature
git push -u origin feature/nueva-funcionalidad

# 5. Crear PR en GitHub, después del merge:
git checkout main && git pull origin main
git branch -d feature/nueva-funcionalidad
```

### **🚨 Hotfix Workflow**
```bash
# 1. Crear hotfix desde main
git checkout main && git pull origin main
git checkout -b hotfix/corregir-error-critico

# 2. Corregir y commitear
git add . && git commit -m "Corregir error crítico en producción"

# 3. Push y merge rápido
git push -u origin hotfix/corregir-error-critico
# Crear PR urgente en GitHub
```

---

## ⚠️ **Comandos Peligrosos** 

```bash
# ⚠️ USAR CON PRECAUCIÓN - Pierden historial/cambios
git reset --hard HEAD~1                       # Elimina último commit
git push --force                               # Sobrescribe historial remoto
git branch -D nombre-branch                    # Elimina branch sin verificar merge
git clean -fd                                  # Elimina archivos no rastreados
git reflog expire --expire=now --all          # Elimina reflog
```

---

[📖 **Ver Guía Completa**](./GIT-GITHUB-GUIA.md) | [🏠 **Navegación**](../../../NAVEGACION-DOCUMENTOS.md)
