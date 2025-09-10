# Despliegue en GitHub Pages

## Instrucciones para desplegar esta aplicación en GitHub Pages

### Paso 1: Preparar el repositorio
1. Sube todos los archivos de la carpeta `dist` a la rama `gh-pages` de tu repositorio
2. O configura GitHub Pages para usar la rama `main` con la carpeta `/docs` si prefieres

### Paso 2: Configurar GitHub Pages
1. Ve a la configuración de tu repositorio en GitHub
2. Navega a la sección **Pages**
3. Selecciona la fuente: **Deploy from a branch**
4. Elige la rama `gh-pages` (o `main` con `/docs`)
5. Guarda la configuración

### Paso 3: Actualizar el manifiesto (opcional)
Si necesitas actualizar el manifiesto de archivos después del despliegue:
```bash
npm run update-manifest
```

### Estructura de archivos
- `index.html` - Página principal
- `assets/` - Archivos CSS, JS y otros recursos
- `docs/` - Documentación en formato Markdown
- `constants.ts` - Configuración de la aplicación
- `update-manifest.js` - Script para actualizar el manifiesto
- `.github/workflows/` - Workflows de GitHub Actions

### Notas importantes
- Esta es una aplicación estática compatible con GitHub Pages
- No requiere servidor backend
- Todos los archivos necesarios están incluidos en esta carpeta
- Los workflows de GitHub Actions están incluidos para automatizar el despliegue
