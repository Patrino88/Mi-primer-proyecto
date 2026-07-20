# Activación progresiva de negocios y módulos

La aplicación inicia únicamente con el espacio personal. Negocios es una capacidad opcional que se vuelve visible cuando el usuario crea su primer negocio.

## Regla principal

Los módulos existen en la arquitectura, pero la interfaz sólo los muestra cuando se crean o activan. Los límites de productos y variantes representan capacidad soportada; no son registros, botones ni espacios precargados.

## Progresión visual

1. Inicio personal con una acción opcional para agregar un negocio.
2. Al crear el primer negocio aparece su tablero mínimo y el selector de espacios.
3. Al crear el primer producto aparece el catálogo correspondiente.
4. Inventario, producción, fiscalidad y otras áreas se activan por separado.
5. Un negocio de servicios o reventa no necesita mostrar producción.
6. Desactivar un módulo lo oculta sin borrar su historial.

## Arquitectura prevista

- Registro central de módulos, rutas, dependencias y permisos.
- Manifiesto de módulos activos por espacio de negocio.
- Navegación construida dinámicamente desde ese manifiesto.
- Esquema de datos disponible mediante migraciones, sin filas ficticias.
- Verificación de espacio y módulo en cada ruta.
- Carga diferida del código y los datos de áreas no utilizadas.
- Búsqueda, paginación y virtualización para catálogos amplios.

## Reglas de experiencia

- Un estado vacío presenta contexto y una acción principal.
- No se muestran tableros llenos de ceros ni cientos de espacios vacíos.
- La capacidad máxima sólo se muestra en administración avanzada o cerca del límite.
- Personal permanece limpio aunque existan uno o varios negocios.
- Activar y desactivar es reversible; archivar conserva la trazabilidad.

