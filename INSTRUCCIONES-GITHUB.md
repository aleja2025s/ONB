# 🚀 Instrucciones para Subir a GitHub

## Paso 1: Crear Repositorio en GitHub

1. Ve a [github.com](https://github.com) e inicia sesión
2. Haz clic en el botón **"+"** (arriba derecha) → **"New repository"**
3. Configura tu repositorio:
   - **Repository name:** `Entrenamiento-ACQ-GitHub` (o el nombre que prefieras)
   - **Description:** "Presentación interactiva de entrenamiento ACQ para Nu Colombia"
   - **Visibility:** Elige **Public** o **Private** según necesites
   - ⚠️ **NO marques** "Initialize with README" (ya tienes uno)
4. Haz clic en **"Create repository"**

## Paso 2: Conectar tu Proyecto Local con GitHub

Abre la **Terminal** y ejecuta estos comandos:

```bash
# Navegar a la carpeta del proyecto
cd /Users/alejandra.pinzon/Desktop/Entrenamiento-ACQ-GitHub

# Verificar que todo está guardado
git status

# Conectar con tu repositorio de GitHub (reemplaza [TU-USUARIO] y [NOMBRE-REPO])
git remote add origin https://github.com/[TU-USUARIO]/[NOMBRE-REPO].git

# Cambiar rama a main (si está en master)
git branch -M main

# Subir todo a GitHub
git push -u origin main
```

### Ejemplo con datos reales:
```bash
git remote add origin https://github.com/alejandrapinzon/Entrenamiento-ACQ-GitHub.git
git branch -M main
git push -u origin main
```

## Paso 3: Activar GitHub Pages (Publicar en línea)

1. En tu repositorio de GitHub, ve a **Settings** (⚙️)
2. En el menú lateral, busca **Pages**
3. En **Source**, selecciona:
   - **Branch:** `main`
   - **Folder:** `/ (root)`
4. Haz clic en **Save**
5. Espera 1-2 minutos
6. Tu sitio estará disponible en:
   ```
   https://[TU-USUARIO].github.io/[NOMBRE-REPO]
   ```

## 📋 Estado Actual del Proyecto

✅ **Git inicializado**  
✅ **Commit realizado** (Versión 2.0)  
✅ **README actualizado**  
✅ **Archivos listos para subir**

### Archivos incluidos:
- ✅ `index.html` - Presentación completa (18 slides)
- ✅ `README.md` - Documentación detallada
- ✅ `.gitignore` - Archivos a ignorar
- ✅ `dashboard-wedukas.html` - Dashboard adicional
- ✅ `seguimiento-wedukas.html` - Seguimiento
- ✅ `tags-fon.html` - Tags FON

## 🔐 Autenticación en GitHub

Si Git te pide autenticación, tienes dos opciones:

### Opción 1: Personal Access Token (Recomendado)
1. Ve a GitHub → Settings → Developer settings
2. Personal access tokens → Tokens (classic)
3. Generate new token
4. Selecciona scopes: `repo`
5. Copia el token y úsalo como contraseña

### Opción 2: GitHub CLI
```bash
# Instalar GitHub CLI (si no lo tienes)
brew install gh

# Autenticarte
gh auth login
```

## 🆘 Solución de Problemas

### Error: "remote origin already exists"
```bash
git remote remove origin
git remote add origin https://github.com/[TU-USUARIO]/[NOMBRE-REPO].git
```

### Error: "failed to push"
```bash
git pull origin main --rebase
git push -u origin main
```

### Verificar conexión
```bash
git remote -v
```

## 📊 Comandos Útiles

```bash
# Ver estado actual
git status

# Ver historial de commits
git log --oneline

# Ver archivos que se subirán
git ls-files

# Ver qué remoto está configurado
git remote -v
```

## ✨ Actualizaciones Futuras

Cuando hagas cambios en el futuro:

```bash
# 1. Guardar cambios
git add .

# 2. Crear commit
git commit -m "Descripción de los cambios"

# 3. Subir a GitHub
git push
```

## 🎯 Resultado Final

Una vez subido, podrás:
- ✅ Ver tu código en GitHub
- ✅ Compartir el enlace de GitHub Pages
- ✅ Colaborar con otros
- ✅ Mantener historial de versiones
- ✅ Acceder desde cualquier lugar

---

**💜 ¡Listo para subir a GitHub!**

Si tienes dudas, consulta la [documentación oficial de GitHub](https://docs.github.com/es).
