# Política de Privacidad — Leira

Página estática con la Política de Privacidad de la app [Leira](https://github.com/), publicada
vía GitHub Pages para tener una URL pública y permanente (sin login) que enlazar desde el menú de
perfil de la app y desde la ficha de Google Play.

Fuente única: `index.html`. Para editar el contenido, edita ese archivo y vuelve a hacer push —
GitHub Pages lo redespliega solo.

## Pendiente antes de publicar en Google Play

- Rellenar los datos legales reales en la sección "Quiénes somos" (`[nombre completo o razón
  social del responsable]`, `[NIF/DNI]`, `[domicilio a efectos de notificaciones]`) — hoy son
  placeholders a propósito.
- Revisión legal recomendada: este texto es un borrador de buena fe, no asesoría jurídica.
- Actualizar `EXPO_PUBLIC_PRIVACY_POLICY_URL` en el proyecto de la app (local y en EAS,
  `eas env:push`) con la URL final de GitHub Pages.
