# Dashboard CMV 2026 · V10

Dashboard territorial con **199 registros** de la Matriz PIA-2026(3) y **289 geometrías** viales GL/GR. Las geometrías no equivalen a intervenciones adicionales.

## Publicación en GitHub Pages

1. Subir `index.html`, `.nojekyll` y `README.md` a la raíz del repositorio `RAMFORD25/Dashboard-CMV-2026`.
2. En GitHub: **Settings → Pages → Build and deployment → Deploy from a branch → main → /(root) → Save**.
3. Visitar `https://ramford25.github.io/Dashboard-CMV-2026/` cuando se complete la publicación.
4. Crear en MapTiler una **clave pública** de mapas web y autorizar `ramford25.github.io` en **Allowed HTTP Origins**.
5. En el dashboard, abrir **Ámbito Territorial**, pulsar **⚙ API Key**, introducir la clave y guardar. La clave se guarda en `localStorage` de ese navegador, **no** en GitHub.
6. Seleccionar **Calles**, **Satélite** o **Topográfico**. Si falla la conexión o la autorización, el visor local mantiene los trazados.

## Notas técnicas

- No introducir tokens privados ni credenciales administrativas.
- El almacenamiento local de la clave es específico del navegador y dispositivo. Otros usuarios necesitarán configurar su propia clave, salvo que se implemente una clave pública de producción restringida al dominio en una versión posterior.
- MapTiler requiere Internet y un plan adecuado a uso institucional. Verificar atribución, límites y licencia antes de difusión pública.
- Los estilos Claro, Oscuro y Alto contraste muestran trazados sin solicitar teselas MapTiler.
- Chart.js y Leaflet se obtienen mediante CDN; para funcionamiento completamente desconectado habría que alojar estas bibliotecas localmente.
- La red vial proviene de los GeoJSON entregados y los indicadores de la matriz; las geometrías simplificadas no reemplazan a los archivos GIS originales.
- Los nombres de las rutas sin coincidencia no deben incorporarse automáticamente a los totales de intervenciones.
