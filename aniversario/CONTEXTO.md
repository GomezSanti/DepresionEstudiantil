# Contexto: invitación web aniversario 15 años — Santi & Floppy

Este archivo resume todo lo decidido en el chat donde se armó la invitación, para retomarla en otra conversación sin perder nada. Pegalo (o pedile a Claude que lo lea) al empezar.

## Qué es

Una página web de invitación para el fin de semana de aniversario (15 años juntos) de **Santi & Floppy**, para compartir por WhatsApp con amigos.

- **Link publicado:** https://claude.ai/artifact/JMbtWyBFZJXGvyivcELQEM (compartido como "Cualquiera con el link")
- **Código:** repo `gomezsanti/depresionestudiantil`, rama `claude/anniversary-invitation-website-gpda09`, carpeta `aniversario/`
  - `aniversario/index.html` — la página completa (HTML + CSS + JS en un solo archivo)
  - `aniversario/fotos/` — fotos optimizadas (≈1200–1400 px, JPG calidad ~78–80)
- **Cómo actualizar:** editar `index.html`, volver a publicar el mismo artifact pasando su URL (así el link no cambia) e incluir en `files` las fotos nuevas como `fotos/<nombre>.jpg`. Commit + push a la rama.

## Datos del evento

| Dato | Valor |
|---|---|
| Nombres | Santi & Floppy |
| Motivo | 15 años juntos ("la mitad de nuestra vida 😅") |
| Lugar | Balneario Bella Vista, Maldonado, Uruguay |
| Ubicación exacta | -34.80573272705078, -55.354427337646484 → https://www.google.com/maps/search/?api=1&query=-34.80573272705078%2C-55.354427337646484 |
| Reserva desde | Viernes 23 de octubre de 2026, desde las 12:00 |
| Reserva hasta | Lunes 26 de octubre de 2026, a las 10:00 |
| WhatsApp para confirmar | 092 786 001 (en código: `59892786001`) — solo este número |
| Alojamiento | Ya pago por Santi & Floppy; los invitados no ponen plata para la casa |

## La casa (predio)

- 3 casas en un mismo predio: **casa principal** (2 dormitorios, baño, living con estufa a leña), **cabaña chica** (1 dormitorio, baño), **cabaña grande** (2 dormitorios, baño). Los nombres "chica/grande" los puso Claude.
- Total: 5 dormitorios, 3 baños, **capacidad 14 personas** ("Somos menos, así que hay lugar de sobra").
- Para compartir: parrillero, deck techado, gran patio, living con estufa a leña.
- Link Airbnb original (no se pudo leer por bloqueo de red): https://es-l.airbnb.com/rooms/47951753

## Estructura actual de la página (en orden)

1. **Portada:** "15" grande, "Santi & Floppy", subtítulo cercano, **collage de 5 fotos de la pareja sin títulos** (estrellas grande + perros, blanco y negro, viaje, cantando). Debajo, franja tipo ticket: Reserva desde / Reserva hasta / Dónde / Faltan X días (cuenta regresiva dinámica: se recalcula al abrir; "¡Es hoy!" durante el finde; "Gracias por venir" después).
2. **La invitación:** texto cálido ("Hace quince años empezamos esta historia…"), firma "Los esperamos con muchas ganas, Santi & Floppy". Tarjetas: Quedarte a dormir (recomienda traer sábanas y toallas) · Venir por el día ("Caés cuando quieras…") · La casa ya está paga.
3. **La casa — "Dónde vamos a estar":** galería de 16 fotos del predio con visor ampliado (tocar para agrandar, flechas, Esc). Tarjetas de las tres casas y "Para compartir".
4. **El plan — "Ideas de itinerario"** (tablero de 4 casillas con dados):
   - Viernes: Mediodía — llegamos y ya estamos para recibir a quien quiera venir · Noche — picamos algo
   - Sábado: Mediodía — pastas · Noche — pizzas y juegos de caja
   - Domingo: Sin planes — trekking, mate en el pasto, playa, juegos, libros o charlas de catarsis. Todo vale.
   - Lunes: Temprano — desayuno · 10:00 — entregamos la casa
5. **Cómo llegar — "Bella Vista, Maldonado":** esquema de costa + botón a Google Maps con el pin exacto. En ómnibus: desde Tres Cruces, ómnibus a Piriápolis que pasan por Bella Vista; avisar y los van a buscar a la parada. Nota: "Nosotros salimos el viernes de mañana y tenemos 2 lugares en el auto."
6. **Qué traer:** recuadro "Si te quedás a dormir, te recomendamos traer sábanas y toallas. Nosotros vamos a llevar algunas, pero mejor que no falten." · Si querés, traé: algo para tomar, algo para compartir, tu juego de caja favorito, un abrigo · No hace falta: plata para la casa.
7. **Confirmación — "¿Venís?":** formulario (nombre; Me quedo a dormir / Voy por el día / Esta vez no puedo, pero los tkm; días Vie–Lun; cuántos son; mensaje opcional) → arma el texto y abre WhatsApp al 092 786 001, con botón "Copiar texto" de respaldo.
8. **Pie:** "Los esperamos en Bella Vista · Santi & Floppy · 23 al 26 de octubre de 2026".

## Decisiones tomadas (no volver a proponer)

- **Sin asado** en ningún lado (sí se menciona el parrillero como comodidad).
- **Sin dress code**, sin traje de baño/protector solar, sin restricciones alimentarias, sin pregunta de transporte.
- **No organizan autos**: solo se ofrecen sus 2 lugares del viernes de mañana; quien va en ómnibus avisa y lo buscan.
- **Sin actividades "de tarde"** en el plan.
- **Sin "vuelta"**: cada uno gestiona su regreso; solo se indica que la reserva termina el lunes 10:00.
- Lo de traer cosas va como sugerencia ("Si querés, traé"), nunca como obligación.
- Se sacó la sección "book" de fotos y el "Gracias por mirar"; las fotos de la pareja quedaron en el collage de portada.
- No se agregó "cocina" a comodidades (pidieron no hacerlo). La info del ómnibus quedó confirmada como está.
- Confirmación por WhatsApp (no base de datos) porque los invitados abren el link sin cuenta.

## Diseño

- Tema único claro, paleta mar/arena: tinta `#17303F`, mar `#2F6F73`, verde agua `#DCEBE7`, sol `#F0B63F`, coral `#E0674F`, fondo `#F2F6F4`.
- Tipografías: **Young Serif** (títulos) + **Figtree** (texto), de Google Fonts.
- Responsive (probado en 400 px y 1200 px), sin scroll horizontal.

## Fotos (`aniversario/fotos/`)

- Pareja: `nosotros-estrellas.jpg` (principal), `nosotros-perros.jpg`, `nosotros-bn.jpg` (recortado sin el sticker de Instagram), `nosotros-pisa.jpg`, `nosotros-cantando.jpg`.
- Predio: `casa-principal`, `living`, `cocina`, `deck-techado`, `cabanas`, `cabanas-hortensias`, `parrillero-noche` (leyenda "Parrillero"), `parrillero`, `dormitorio-matrimonial`, `dormitorio-cuchetas`, `dormitorio-camas`, `bano-1`, `bano-2`, `patio`, `jardin`, `camino-al-mar`.

## Cómo trabajar con los cambios

- Los cambios llegaron como comentarios sobre el artifact ("Send to Claude"): se aplicaban, se republicaba, se respondía en el hilo y se marcaba resuelto.
- Estilo de textos: rioplatense/uruguayo, cercano, voseo ("venís", "traé", "avisanos"), sin sonar a obligación.
