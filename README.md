# BusDiag 4.1 — Catálogo técnico inicial

Actualización de BusDiag 4.0. Conserva diagnóstico, mediciones y casos locales.

## Novedades
- Biblioteca con búsqueda por código, sistema o descripción.
- Botón para descargar en el navegador los códigos OBD-II públicos de OBDex (no se almacena permanentemente).
- Muestra la fuente y distingue fichas orientativas de códigos importados.
- Si falla la conexión o cambia el formato externo, la biblioteca local sigue funcionando.
- Limita resultados visibles a 80 para mantener fluidez en Android.

## Publicación manual
En GitHub, abre `index.html`, elige Edit (lápiz), sustituye el contenido por el del nuevo archivo y pulsa Commit changes; o usa Add file > Upload files para reemplazarlo. Reemplaza también README.md si quieres. La actualización de Cloudflare depende de cómo hayas configurado el despliegue; comprueba que aparece «4.1 · CATÁLOGO».

## Alcance y limitaciones
OBDex: https://github.com/foerbsnavi/OBDex (el proyecto indica CC0). No se han importado ni copiado manuales OEM. No se ha integrado MechanicDB ni J1939 todavía. La compatibilidad del formato remoto y CORS se comprueban al pulsar Cargar; pueden variar. La importación es temporal y los casos permanecen en el almacenamiento local del navegador. No introducir datos personales de clientes. Nunca interpretar un código como diagnóstico definitivo.
