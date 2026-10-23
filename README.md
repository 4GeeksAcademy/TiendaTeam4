# TiendaTeam4

TiendaTeam4 es una tienda en línea desarrollada como proyecto colaborativo de 4Geeks, con el objetivo de practicar HTML5, Tailwind CSS y trabajo en equipo mediante Git y GitHub.

## Stack

- HTML5
- Tailwind CSS mediante CDN

## Páginas

- `index.html`: página principal
- `catalog.html`: portada de las tres categorías
- `catalog-woman.html`: catálogo de Mujer (9 productos)
- `catalog-man.html`: catálogo de Hombre (7 productos)
- `catalog-accessories.html`: catálogo de Accesorios (4 productos)
- `products/`: 20 fichas individuales, una por producto
- `cart.html`: carrito de ejemplo con 3 productos
- `checkout.html`: formulario de compra simulado con validación HTML nativa

## Cómo abrir el proyecto

Abre `index.html` en un navegador. Tailwind CSS se carga mediante CDN y requiere conexión a internet.

Opcionalmente, el servidor auxiliar original se inicia con `python server.py` en el puerto 3000 y requiere Flask (`pip install flask`). Flask solo sirve los archivos; no procesa compras.

## Interacciones del prototipo

- Los enlaces permiten navegar por categorías. Los radios de talla filtran las tarjetas con variantes Tailwind `group-has` basadas en `:has()`, sin JavaScript propio ni CSS personalizado. Se necesita un navegador moderno y conexión al CDN; no hay consulta de stock ni filtros persistentes. El contador indica el total de la categoría.
- Cada ficha conserva sus tallas y dos desplegables HTML nativos (`details`/`summary`). Las tallas e información de materiales son datos del ejercicio, no un inventario comercial certificado.
- El carrito es estático: las cantidades 1–5 y los botones de añadir/eliminar no recalculan ni guardan el pedido. Los tres productos de ejemplo suman 119,97 €, con IVA incluido y envío gratis.
- En checkout, `required`, el tipo email y los patrones de tarjeta/CVV activan validación nativa al enviar. Los campos no tienen `name`, para no transmitir datos personales o bancarios. Un envío válido lleva al aviso de simulación; no procesa pagos. Usar solo datos ficticios.
- Las imágenes externas son demostrativas y requieren internet. Antes de publicar una tienda comercial deben verificarse sus licencias y sustituirse por fotografías propias o autorizadas.

## Flujo de trabajo

1. Crea una rama independiente para cada tarea.
2. Registra los cambios con commits descriptivos.
3. Sube cada rama a GitHub.
4. Abre un Pull Request.
5. Solicita y completa la revisión.
6. Tras la aprobación, integra el cambio en `main`.
