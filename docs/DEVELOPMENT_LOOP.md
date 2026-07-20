# Loop de construcción con Codex

Desde F3, cada unidad pequeña seguirá un ciclo controlado:

1. Seleccionar una función y sus criterios de aceptación.
2. Leer únicamente las especificaciones relacionadas.
3. Implementar el cambio mínimo completo.
4. Ejecutar pruebas automáticas y comprobaciones estáticas.
5. Revisar el flujo visual cuando corresponda.
6. Comparar el resultado con los criterios aprobados.
7. Corregir fallos y repetir con un límite definido.
8. Detenerse al cumplir los criterios y registrar un punto estable en Git.

## Límites del loop

- No es infinito.
- No sustituye decisiones de producto.
- No modifica módulos fuera del alcance de la tarea.
- Se detiene ante requisitos contradictorios, pérdida de datos o cambios destructivos.
- Cada cierre debe dejar pruebas reproducibles.

## Niveles

- **Microloop:** función individual.
- **Loop de flujo:** interacción completa entre pantallas y datos.
- **Loop de fase:** regresión general antes de aprobar una etapa.

