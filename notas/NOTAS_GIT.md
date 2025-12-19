#!/bin/bash

# ==========================================

# MANUAL DE SUPERVIVENCIA GIT - UTL

# Uso: bash manual_git.sh

# ==========================================

cat << 'EOF'

---

## 🚀 BIBLIA DE GIT & GITHUB (Edición Ingeniería)

1. 🛠️ CONFIGURACIÓN INICIAL (Solo 1 vez por PC nueva)
   git config --global user.name "Tu Nombre"
   git config --global user.email "tu_correo@ejemplo.com"

---

2. 🔄 RUTINA DIARIA (Subir cambios a la nube)
   Pasos sagrados para guardar tu código:

   1. Empaquetar: git add .
   2. Etiquetar: git commit -m "Descripción de lo que hice"
   3. Enviar: git push

---

3. ✨ EMPEZAR PROYECTO NUEVO (Desde Cero)

   1. Crea el repo VACÍO en GitHub.
   2. En tu carpeta local ejecuta:
      git init
      git branch -M main
      git remote add origin https://github.com/TU_USUARIO/REPO.git
      git add .
      git commit -m "Inicio"
      git push -u origin main

---

4. 📥 CLONAR (Descargar código en otra PC)

   git clone https://github.com/TU_USUARIO/REPO.git

---

5. 🧹 LIMPIEZA (.gitignore)
   Crea un archivo llamado .gitignore con esto adentro para
   evitar subir basura (.exe, .o):

   _.exe
   _.o
   \*.class
   .vscode/

   _Si ya subiste basura por error, bórrala con:_
   git rm -r --cached .
   git add .
   git commit -m "Limpieza"
   git push

---

6. 🆘 EMERGENCIAS

   - Error "refusing to merge" o historiales diferentes:
     git push -u origin main --force

   - Si todo falla y las carpetas están locas:
     Borra la carpeta oculta .git y empieza de nuevo con git init

---

EOF
