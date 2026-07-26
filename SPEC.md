# Vitrina — asistente de ventas y costeo por WhatsApp

## Qué es

Un asistente con IA, operado 100% por WhatsApp, para vendedores informales (reposteros caseros, reventa de ropa, etc.) que hoy atienden pedidos a mano por chat. No es "un catálogo con link de pago" — es un asistente contable y de ventas.

## Flujo 1 — Onboarding / carga de inventario (conversacional)

- El vendedor le manda al asistente fotos y datos de sus productos por WhatsApp.
- El asistente arma el inventario a medida que se lo van pasando.
- Por cada producto pregunta: **costo** y **precio de reventa**.
- Si el producto es una **composición/receta** (ej. una torta), el asistente ayuda a calcular el costo preguntando: componentes, cantidad de cada uno, y precio de costo de cada componente. Con eso arma el costo total del producto.
- Recién con costo + precio de reventa definidos, el producto queda "publicado" en la vitrina del negocio.

## Flujo 2 — Atención al cliente final (conversacional)

- El mismo asistente atiende a los clientes del negocio por WhatsApp.
- Toma el pedido conversando (no un formulario).
- Arma el link de pago de Mercado Pago por el total.
- **Delivery**: el vendedor puede configurar si ofrece delivery o no, y si el delivery tiene costo adicional o es gratis. Si lo ofrece, el asistente pregunta si el cliente lo quiere y suma el costo correspondiente al total antes de generar el link de pago.

## Flujo 3 — Cumplimiento del pedido

- Una vez que Mercado Pago confirma el pago, el asistente le avisa al negocio (dueño) que hay un pedido nuevo confirmado, con el detalle, para que lo despache/entregue.

## Flujo 4 — Registro y métricas

- Cada venta confirmada queda registrada.
- El asistente calcula y acumula el margen real de cada venta (precio de reventa − costo), para que el vendedor sepa cuánto está ganando de verdad, no solo cuánto factura.

## Flujo 5 — Facturación AFIP (fase posterior, no MVP)

- Si el cliente pide factura, integrar con AFIP para generar la facturación electrónica automáticamente.
- Requiere CUIT y certificado digital del vendedor — se deja para cuando haya usuarios pagando que lo pidan, no es parte del MVP inicial.

## Modelo de negocio (contexto, ya definido)

- SaaS por suscripción (USD 3-8/mes), no comisión por venta.
- Mercado Pago le paga directo al vendedor — Vitrina nunca toca la plata (evita riesgo regulatorio de pasarela de pagos).
- Landing de validación ya publicada: https://damiantofay.github.io/vitrina/ (todavía sin tráfico real).

## Alcance sugerido para este MVP (Tramo 1)

Priorizar Flujos 1-4 (inventario conversacional + costeo de recetas + atención de ventas + delivery opcional + registro de márgenes). AFIP (Flujo 5) queda para después.
