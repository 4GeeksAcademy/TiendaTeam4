# Contexto para IA y coding agents

## Stack

- Usa exclusivamente HTML5 semántico y clases de Tailwind CSS cargadas mediante CDN.
- No uses React, Vue, Next.js, otros frameworks ni JavaScript; las interacciones pueden ser visuales si el ejercicio no exige funcionalidad.
- Mantén la misma configuración de Tailwind CDN en todos los archivos HTML, incluidos los colores personalizados acordados.
- No añadas dependencias nuevas.

## Diseño

- Mantén una estética elegante, moderna y comercial, coherente con una marca de ropa francesa.
- Usa la paleta acordada: `slate-900` para elementos principales, `amber-600` para acentos y ofertas, `stone-50` como fondo y `stone-200` para bordes.
- Usa `font-sans`, títulos en negrita y texto base en `text-slate-700`.
- En las tarjetas de producto, reutiliza el patrón aprobado: `rounded-lg`, `shadow-sm`, `hover:shadow-md`, `transition` y `p-4`.
- Mantén los botones primarios en `bg-slate-900 text-white` y los secundarios con borde `border-slate-900` y texto `text-slate-900`, respetando los estados hover acordados.
- Diseña para distintos tamaños de pantalla y mantén la consistencia visual entre todas las páginas.
- Conserva los componentes globales aprobados y evita estilos que rompan la identidad visual del proyecto.

## Componentes globales

- Mantén la navbar y el footer consistentes en todas las vistas.
- Si ya están aprobados, no los regeneres ni rediseñes sin necesidad.
- Reutiliza los patrones visuales existentes antes de crear otros.

## Requisitos de catálogo y detalle

- En `catalog.html`, incluye la navbar y el footer compartidos, filtros por categoría y talla, y una cuadrícula de 20 productos (4 columnas por 5 filas en escritorio, adaptable a pantallas pequeñas).
- Cada producto del catálogo debe reutilizar la tarjeta aprobada y enlazar a su página de detalle en `product.html`.
- En `product.html`, presenta una imagen principal y, en una segunda columna, el nombre, la referencia, el precio, las tallas disponibles y el botón de compra.
- Añade debajo una sección con información sobre los materiales y usos del producto.
- Mantén la navegación entre páginas y reutiliza la identidad visual y los componentes globales aprobados.

## Reglas de edición

- Revisa el código existente antes de modificarlo.
- Limita los cambios a los archivos necesarios para la tarea actual.
- No elimines código existente sin una razón clara.
- Usa HTML semántico.
- Evita duplicaciones innecesarias.
- Respeta los cambios realizados por otros colaboradores.

