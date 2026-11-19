# BusDiag Online 4.0 — primera versión pública de pruebas

Web estática adaptable a móvil. La pantalla inicial pregunta primero por los síntomas; marca, modelo y código de avería son opcionales. Incluye diagnóstico orientativo por reglas, biblioteca de ejemplo, cálculos de mediciones y casos guardados en el navegador.

## Publicación gratuita desde GitHub

1. Sube `index.html` y `README.md` a la raíz de tu repositorio privado `busdiag-web`.
2. En Cloudflare: **Workers & Pages → Create → Pages → Connect to Git**. Autoriza el repositorio privado.
3. Selecciona `busdiag-web`. Configura **Framework preset: None**, **Build command: vacío**, **Build output directory: /** (raíz). Si la interfaz no admite `/`, usa el modo de despliegue estático correspondiente.
4. Publica y abre la dirección `.pages.dev` que Cloudflare te asigne.

## Límites y privacidad

- Esta versión NO conecta todavía OBDex, MechanicDB, J1939 ni Supabase.
- La biblioteca contiene nueve fichas orientativas; no son datos OEM certificados.
- Los casos se guardan en `localStorage` de ese navegador, no en el repositorio ni en un servidor. Exporta copias de seguridad.
- La web publicada será accesible a cualquiera que tenga la dirección, aunque GitHub sea privado. No subas datos personales ni información confidencial.
- Los resultados de diagnóstico son hipótesis y listas de comprobación, nunca instrucciones de sustitución ni garantías de seguridad.

## Próximas fases

Autenticación, Supabase con permisos por usuario/taller, importadores licenciados, J1939/SPN-FMI y diagnósticos guiados por procedimientos verificados.
