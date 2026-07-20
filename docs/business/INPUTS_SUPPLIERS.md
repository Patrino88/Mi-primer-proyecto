# Insumos y proveedores

Especificación genérica aprobada para la futura ruta de negocios. No contiene proveedores, precios, productos ni operaciones reales.

## Modelo

```text
Insumo
  └─ Presentación de compra
       └─ Oferta de proveedor
            └─ Compra
                 └─ Recepción
                      └─ Capa de inventario PEPS
```

## Decisiones aprobadas

- El insumo conserva su identidad aunque cambien el proveedor o el empaque.
- Una presentación puede ser ofrecida por varios proveedores.
- La compra representa el compromiso financiero; la recepción representa la entrada física.
- Sólo la cantidad recibida, aceptada y utilizable aumenta el inventario.
- La unidad base y las conversiones son explícitas, auditables y versionadas.
- Las conversiones entre masa y volumen requieren densidad registrada.
- El costo utilizable considera descuentos, cargos y cantidad aceptada.
- Los costos incompletos permanecen visibles y no se convierten en cero confirmado.
- Cada recepción crea una capa histórica de inventario con su propio costo.
- Caducidad, merma, devoluciones y ajustes conservan causa y trazabilidad.
- Archivar conserva compras, consumos, costos y relaciones históricas.

## Tipos previstos

- Materia prima.
- Empaque o envase.
- Consumible operativo.
- Servicio sin inventario físico.

Los activos y equipos se administrarán en un módulo diferente para evitar confundir consumo con depreciación o mantenimiento.

