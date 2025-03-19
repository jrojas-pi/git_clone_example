# GIT Comandos Básicos

## 📚 Configuración Inicial
```bash
git config --global user.name "Tu Nombre"
git config --global user.email "tuemail@example.com"
git config --list  # Ver configuración actual
```

---

## 📂 Inicializar y Clonar Repositorios
```bash
git init  # Inicializa un nuevo repositorio Git en la carpeta actual
git clone URL_DEL_REPO  # Clona un repositorio remoto
```

---

## 📌 Estado y Seguimiento de Cambios
```bash
git status  # Muestra el estado del repositorio
git add archivo.txt  # Agrega un archivo al área de staging
git add .  # Agrega todos los archivos modificados
git commit -m "Mensaje del commit"  # Guarda los cambios en el historial
git log  # Muestra el historial de commits
git log --oneline --graph --decorate --all  # Historial en una línea con ramas
```

---

## 🔄 Trabajo con Ramas
```bash
git branch  # Lista todas las ramas
git branch nueva_rama  # Crea una nueva rama
git checkout nueva_rama  # Cambia a otra rama (Git <2.23)
git switch nueva_rama  # Cambia de rama (Git 2.23+)
git checkout -b nueva_rama  # Crea y cambia a la nueva rama
git switch -c nueva_rama  # Alternativa moderna a checkout -b
git merge otra_rama  # Fusiona 'otra_rama' en la actual
git branch -d nombre_rama  # Borra una rama local
```

---

## 🚀 Sincronización con Remoto
```bash
git remote add origin URL_DEL_REPO  # Vincula el repo local con el remoto
git remote -v  # Muestra los repositorios remotos configurados
git push origin main  # Envía cambios a la rama 'main'
git push -u origin main  # Sube la rama actual y la vincula con remoto
git pull origin main  # Descarga y fusiona cambios del remoto
git fetch origin  # Descarga cambios sin fusionarlos
```

---

## 🚑 Deshacer Cambios
```bash
git checkout -- archivo.txt  # Revierte cambios en un archivo
git reset HEAD archivo.txt  # Quita el archivo del área de staging
git reset --soft HEAD~1  # Revierte el último commit pero mantiene los cambios
git reset --hard HEAD~1  # Revierte el último commit y borra los cambios
git revert HEAD  # Crea un commit que revierte el último commit
```

---

## 🔍 Ver y Comparar Cambios
```bash
git diff  # Muestra los cambios en los archivos
git diff --staged  # Muestra los cambios en el área de staging
git show HEAD  # Muestra detalles del último commit
```

---

## 🔒 Manejo de Stash (Guardar Cambios Temporales)
```bash
git stash  # Guarda los cambios sin hacer commit
git stash list  # Muestra la lista de stashes guardados
git stash pop  # Recupera los cambios guardados en el stash
git stash drop  # Elimina un stash específico
```

---

## 📀 Tags (Etiquetas para versiones)
```bash
git tag -a v1.0 -m "Versión 1.0"  # Crea un tag anotado
git tag  # Lista todas las etiquetas
git push origin v1.0  # Envía un tag al remoto
git push --tags  # Envía todos los tags al remoto
```

