# BusDiag 4.3 — Módulo J1939

## Instalación en GitHub desde Android

1. Sube `busdiag-j1939-4.3.js` a la raíz del repositorio `Tuappinventor/busdiag-web` (al lado de `index.html` y `busdiag-catalogo-4.2.js`).
2. Edita `index.html` y añade esta línea **antes de `</body>`**, sin borrar la de 4.2:

   `<script src="./busdiag-j1939-4.3.js" defer></script>`

3. Confirma el cambio y espera a que Cloudflare publique la actualización.
4. En BusDiag → Biblioteca, baja hasta «Vehículos industriales · J1939».
5. Comprueba que se cargan aproximadamente 100 averías. Busca `SPN 154 FMI 13` o `ABS`.

## Qué hace

- Descarga la muestra pública de `j1939_faults.csv` de MechanicDB.
- Permite filtrar por SPN, FMI, texto y fabricante, con 15 resultados por página.
- Muestra fabricante, controlador, código OEM, descripción y fuente documental.
- Guarda una copia en `localStorage` para siguientes visitas; la primera carga requiere internet.
- No modifica las 9.533 fichas OBDex, el diagnóstico, las mediciones ni los casos privados.

## Fuente y licencia

MechanicDB, `https://github.com/MechanicDB/MechanicDB-public`, muestra Heavy Duty `samples/heavyduty/j1939_faults.csv`.
Datos sujetos a Open Database License (ODbL) 1.0: `https://github.com/MechanicDB/MechanicDB-public/blob/main/LICENSE`. Debe conservarse la atribución y, si se publica una base adaptada, respetarse la obligación de compartir bajo ODbL. Documentación y procedencia: `SOURCES.md` en ese repositorio.

No es la base completa ni cubre todos los fabricantes. Las descripciones no son umbrales OEM ni sustituyen las instrucciones de seguridad. No se ha verificado todavía la descarga CORS desde el dominio Cloudflare del usuario.
