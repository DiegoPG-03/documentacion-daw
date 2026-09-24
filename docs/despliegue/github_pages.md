---
sidebar_position: 1
---

# Despliegue del Proyecto y Documentación

Tanto el código fuente del proyecto como esta propia documentación en Docusaurus se pueden alojar en un repositorio Git y desplegar de forma pública.

## Despliegue de la Documentación en GitHub Pages

Para compilar y publicar este sitio estático de documentación directamente en GitHub, debes seguir estos pasos desde tu terminal (Bash o Linux):

1. Modifica el archivo `docusaurus.config.js` de la raíz, asegurando que los parámetros `url`, `baseUrl`, `organizationName` y `projectName` corresponden a tu cuenta y repositorio.
2. Ejecuta el comando de compilación y subida automática:

```bash
GIT_USER=<tu_usuario_github> USE_SSH=true npm run deploy
