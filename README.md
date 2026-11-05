# Library Scrapping · competencia de productos Sip

Anuncios de la competencia en **Meta Ad Library** y **Google Ads Transparency Center** (Perú), en dos grupos:

- **Anuncios Growth:** una pestaña por producto de Sip: Crédito Efectivo, Maxicash, Tarjeta de Crédito,
  PLD (Préstamo de Libre Disponibilidad) y Sip con Garantía.
- **Anuncios Branding:** anuncios de las mismas marcas que no están asociados a esos productos (marca e institucional,
  sorteos y concursos, educación y seguridad, becas, empleo y comunidad).

Archivos:

- `index.html`: dashboard con filtros por grupo, producto, subtipo de branding, fuente (Meta / Google) y anunciante.
- `data.js`: anuncios clasificados (grupo/producto, fuente, anunciante, fecha de inicio, formato, texto, link al original).
- `img/`: miniaturas propias (los links de imagen de Meta caducan).
- `data_raw*.json`: capturas antes de clasificar.

## Cómo se armó (captura del 5 nov 2026)

- **Meta, Growth:** anuncios activos que aparecen en búsquedas por palabras clave de cada producto ("efectivo express",
  "súper efectivo", "préstamo efectivo", "libre disponibilidad", "solicita tu tarjeta", "tarjeta CMR", etc.), filtrados a
  bancos y financieras, más todos los anuncios activos de las páginas oficiales de Interbank y cajas municipales
  (Arequipa, Piura, Cusco, Trujillo, Ica, Metropolitana), clasificados por texto.
- **PLD tiene prioridad:** todo anuncio que dice "préstamo personal" o "libre disponibilidad" se clasifica como PLD y se
  muestra primero, con la etiqueta "PLD explícito". La ficha de PLD de Sip sale de https://sip.pe/productos/prestamo-personal.
- **Google, Growth:** todos los anuncios mostrados por primera vez desde el 1 oct 2026 en bancoripley.com.pe,
  bancofalabella.pe, bbva.pe, viabcp.com, scotiabank.com.pe y santanderconsumer.com.pe, clasificados por texto o leyendo la pieza.
- **Meta, Branding:** anuncios activos de las páginas oficiales (Ripley, Falabella, BBVA, BCP, Scotiabank, Santander
  Consumer, BanBif, Interbank y cajas) que no mencionan ningún producto financiero ni servicio transaccional.
- Se excluyen páginas que suplantan a Interbank.

## Limitaciones

- Google de Interbank y cajas queda pendiente (Google bloqueó temporalmente la IP).
- En Google no se revisaron los videos de BBVA, BCP y Scotiabank que no traen texto (YouTube está bloqueado en la red).
- En las páginas con muchos anuncios (BBVA, BCP, Ripley) Meta carga hasta ~250 por corrida; Branding no es exhaustivo.
- Meta y Google no publican inversión ni impresiones de anuncios comerciales en Perú.
