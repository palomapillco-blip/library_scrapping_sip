# Library Scrapping · competencia de productos Sip

Anuncios de la competencia en **Meta Ad Library** y **Google Ads Transparency Center** (Perú), agrupados por producto de Sip:
Crédito Efectivo, Maxicash, Tarjeta de Crédito, Sip con Garantía y DLP (préstamo de libre disposición).

- `index.html`: dashboard con una pestaña por producto y filtros por fuente (Meta / Google) y por anunciante.
- `data.js`: anuncios clasificados (fuente, anunciante, fecha de inicio, formato, texto, link al anuncio original).
- `img/`: miniaturas propias (los links de imagen de Meta caducan).
- `data_raw.json` / `data_raw_google.json`: capturas antes de clasificar.

## Cómo se armó (captura del 5 nov 2026)

- **Meta:** anuncios activos que aparecen en búsquedas por palabras clave de cada producto ("efectivo express", "súper efectivo",
  "préstamo efectivo", "libre disponibilidad", "solicita tu tarjeta", "tarjeta CMR", etc.), filtrados a bancos, financieras y cajas.
- **Google:** todos los anuncios mostrados por primera vez desde el 1 oct 2026 en los dominios bancoripley.com.pe,
  bancofalabella.pe, bbva.pe, viabcp.com, scotiabank.com.pe y santanderconsumer.com.pe. Se clasificaron por su texto y,
  cuando el anuncio no trae texto, leyendo la pieza.
- **Interbank y cajas municipales** (Arequipa, Piura, Cusco, Trujillo, Ica, Metropolitana): todos los anuncios activos de su página oficial en Meta, clasificados por texto. Se excluyen páginas que suplantan a Interbank. Google de Interbank y cajas queda pendiente (Google bloqueó temporalmente la IP).

## Limitaciones

- En Google no se revisaron los videos de BBVA, BCP y Scotiabank que no traen texto (YouTube está bloqueado en la red).
- Meta y Google no publican inversión ni impresiones de anuncios comerciales en Perú.
