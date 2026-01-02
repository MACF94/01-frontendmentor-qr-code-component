# GitHub Pages Setup Instructions

Este repositorio está configurado para desplegar automáticamente a GitHub Pages desde la carpeta `qr-code-component-main`.

## Configuración Automática

El workflow de GitHub Actions (`.github/workflows/deploy-pages.yml`) se encarga de:
- Desplegar automáticamente cuando se hace push a la rama `main`
- Usar el contenido de la carpeta `qr-code-component-main` como raíz del sitio

## Pasos para Activar GitHub Pages

Para que el sitio esté disponible públicamente, necesitas configurar GitHub Pages en el repositorio:

1. Ve a la configuración del repositorio en GitHub
2. Navega a **Settings** → **Pages**
3. En la sección **Build and deployment**:
   - **Source**: Selecciona "GitHub Actions"
4. El workflow se ejecutará automáticamente en el próximo push a `main`

## URL del Sitio

Una vez configurado, el sitio estará disponible en:
```
https://MACF94.github.io/01-frontendmentor-qr-code-component/
```

## Desplegar Manualmente

También puedes desplegar manualmente:
1. Ve a la pestaña **Actions** en GitHub
2. Selecciona el workflow "Deploy to GitHub Pages"
3. Haz clic en **Run workflow**

## Estructura

El workflow despliega únicamente el contenido de la carpeta `qr-code-component-main`, que contiene:
- `index.html` - Página principal
- `styles.css` - Estilos
- `images/` - Recursos de imágenes
- Otros archivos del proyecto
