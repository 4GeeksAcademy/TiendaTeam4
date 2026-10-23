# Contexto para IA y coding agents

## Stack

- Usa exclusivamente HTML5 semántico y clases de Tailwind CSS cargadas mediante CDN.
- No uses React, Vue, Next.js, otros frameworks ni JavaScript; las interacciones pueden ser visuales si el ejercicio no exige funcionalidad.
- Usa el mismo CDN de Tailwind en todos los HTML. No añadas configuración JavaScript propia: se usan las utilidades estándar.
- No añadas dependencias nuevas.

## Diseño

- Mantén la estética minimalista, limpia y comercial de LUXE.
- Usa `stone-50` como fondo, `stone-200` para bordes y blanco, negro y tonos stone en los componentes.
- Usa `font-sans`, títulos en negrita y texto base en `text-stone-600` o `text-stone-900`.
- En las tarjetas del catálogo, conserva `bg-white group`, imagen `aspect-[3/4]`, precio y enlace individual. El carrito usa tarjetas con borde y `rounded-lg`.
- Mantén los botones primarios negros o `bg-stone-900 text-white` y los secundarios con borde stone, respetando los estados de foco y hover.
- Diseña para distintos tamaños de pantalla y mantén la consistencia visual entre todas las páginas.
- Conserva los componentes globales aprobados y evita estilos que rompan la identidad visual del proyecto.

## Componentes globales

- Mantén la navbar y el footer consistentes en todas las vistas.
- Si ya están aprobados, no los regeneres ni rediseñes sin necesidad.
- Reutiliza los patrones visuales existentes antes de crear otros.

## Requisitos de catálogo y detalle

- `catalog.html` es la portada con tres bloques de categoría. Los 20 productos se reparten, sin duplicados, entre `catalog-woman.html` (9), `catalog-man.html` (7) y `catalog-accessories.html` (4).
- Los catálogos tienen enlaces de categoría, filtro por talla mediante radios HTML y variantes Tailwind `group-has`/`:has()`, y grid responsive de 2/3/4 columnas. Los filtros necesitan un navegador moderno; no consultan stock ni guardan la selección. El contador refleja el total de la categoría.
- Cada tarjeta enlaza a su ficha en `products/` y debe mantener el mismo nombre, precio, color e imagen. Las referencias son únicas. No existe `product.html`.
- Las fichas muestran la imagen a la izquierda y la información a la derecha desde `md`; en móvil se apilan. Conserva nombre, referencia, precio con IVA incluido, tallas y botón de compra.
- Debajo del botón, en la misma columna, coloca dos `details` con `summary`: Materiales y cuidados y Usos y combinaciones. Después va Volver al catálogo. No dupliques esos contenidos debajo del grid.
- Mantén la navegación entre páginas y reutiliza la identidad visual y los componentes globales aprobados.

## Reglas de edición

- Revisa el código existente antes de modificarlo.
- Limita los cambios a los archivos necesarios para la tarea actual.
- No elimines código existente sin una razón clara.
- Usa HTML semántico.
- Evita duplicaciones innecesarias.
- Respeta los cambios realizados por otros colaboradores.

## Decisiones

- Debido a la restricción de no usar JavaScript, hemos optado por crear la carpeta `products/` en la raíz, con un archivo HTML independiente por producto, en lugar de cargar distintos productos dinámicamente en `product.html`.
- Las tarjetas del catálogo y los productos destacados de inicio enlazan a su ficha correspondiente dentro de `products/`.
- El botón «Añadir al carrito» es únicamente visual: no añade productos ni actualiza cantidades o totales. Esta interacción queda fuera del alcance del prototipo estático, por la restricción de JavaScript y la ausencia de lógica de servidor para gestionar el carrito.
- El enlace al carrito permite navegar a `cart.html`, pero no transfiere el producto ni la talla seleccionada.
- Los tres ejemplos del carrito suman 119,97 €, envío gratis e IVA incluido; no se vuelve a sumar un 21 %. Las cantidades 1–5 y eliminar son controles de un prototipo estático y no actualizan los totales.
- Checkout usa `type="submit"` y validación HTML nativa, sin `novalidate`. Sus campos no tienen `name` para no transmitir datos personales ni bancarios. Un envío válido abre el aviso de simulación; nunca se procesa un pago.
- El servidor Flask original es opcional y solo sirve archivos. No es una dependencia del frontend ni implementa lógica de compra.
- Las imágenes de terceros son demostrativas; verificar permisos antes de cualquier publicación comercial.

