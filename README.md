# Dashboard CMV 2026 · V10.1

## Publicación en GitHub Pages

1. En MapTiler, configura la clave **pública** para permitir únicamente el origen `ramford25.github.io`. Comprueba que el plan autorice este uso público/institucional.
2. Abre `config.js` y reemplaza `PEGAR_AQUI_TU_CLAVE_PUBLICA_MAPTILER` por tu clave pública. **No compartas claves privadas ni credenciales administrativas.**
3. En el repositorio `RAMFORD25/Dashboard-CMV-2026`, sustituye `index.html`, y agrega `config.js` y `.nojekyll` en la raíz de la rama `main` (puedes actualizar README.md).
4. Comprueba `https://ramford25.github.io/Dashboard-CMV-2026/` después de que termine la publicación. Recarga con Ctrl+F5 si ves una versión anterior.

### Seguridad

El botón de edición de la API Key fue retirado. Los visitantes no pueden modificar la configuración compartida desde la interfaz; **sí pueden inspeccionar la clave pública** en el código del sitio y alterar localmente su navegador. Restringe dominio, supervisa cuotas y rota la clave si detectas abuso.

### Cartografía

Calles, Satélite y Topográfico usan MapTiler y requieren Internet. El mapa local con trazados GL/GR permanece disponible como respaldo. Se mantienen 199 registros de matriz y 289 geometrías, que no equivalen a 289 intervenciones.
