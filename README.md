# Documentación legal — Leira

Sitio estático con la documentación legal de la app [Leira](https://github.com/), publicado vía
GitHub Pages para tener URLs públicas y permanentes (sin login) que enlazar desde el menú de
perfil de la app y desde la ficha de Google Play. Cuatro páginas, todas con el mismo diseño y
enlazadas entre sí (bloque superior + pie de página):

- `index.html` → Política de Privacidad (`/`)
- `aviso-legal/index.html` → Aviso Legal (`/aviso-legal/`)
- `terminos/index.html` → Términos y Condiciones (`/terminos/`)
- `eliminar-cuenta/index.html` → Eliminación de cuenta (`/eliminar-cuenta/`)

Para editar el contenido, edita el `index.html` correspondiente y vuelve a hacer push — GitHub
Pages redespliega solo.

## Pendiente antes de publicar en Google Play

- Revisión legal recomendada: estos textos son un borrador de buena fe (contrastado contra las
  guías de la AEPD y los requisitos de Google Play), no asesoría jurídica.
- Actualizar `EXPO_PUBLIC_TERMS_OF_SERVICE_URL` en el proyecto de la app (local y en EAS, `eas
  env:push`) para que apunte a `.../terminos/` — hoy esa página ya existe pero la app todavía no
  la enlaza (sigue cayendo al placeholder `www.leira.app/terminos`).
- Confirmar que `EXPO_PUBLIC_PRIVACY_POLICY_URL` sigue apuntando aquí también en el entorno de
  EAS, no solo en el `.env` local.

## Hecho

- Datos identificativos del titular (razón social, NIF, domicilio) ya rellenados en Privacidad y
  Aviso Legal — ya no son placeholders.
- Confirmado que la base de datos/almacenamiento de Supabase está alojado en la UE — reflejado en
  la sección "Transferencias internacionales" de la Política de Privacidad.
