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
