# Lotes y producción

Especificación genérica aprobada para negocios que transforman o ensamblan productos. Este módulo es opcional y no contiene recetas, costos, operadores ni producciones reales.

## Flujo

```text
Receta versionada
  └─ Lote
       ├─ Reserva opcional
       ├─ Consumos reales
       ├─ Tiempo y eventos
       ├─ Rendimiento y salidas
       ├─ Calidad y bloqueo
       └─ Liberación y cierre
```

## Principios aprobados

- La receta planea y el lote conserva lo que realmente ocurrió.
- Reservar inventario es opcional y nunca equivale a consumirlo.
- Los consumos confirmados se vinculan a capas históricas de inventario.
- Un lote puede producir varias presentaciones, muestras, subproductos, merma o reproceso.
- Las entradas y salidas deben conciliarse sin forzar diferencias físicas a cero.
- Producido no significa vendible: calidad y liberación controlan la disponibilidad.
- El costo distingue esperado, estimado, incompleto y confirmado.
- Las correcciones generan eventos compensatorios y conservan el historial.
- Cada evento tiene identificador, responsable y marca temporal de alta precisión.

## Niveles de control

- **Rápido:** plantilla, cronómetro y captura únicamente de desviaciones.
- **Guiado:** eventos clave, sustituciones, pausas y mediciones.
- **Controlado:** etapas, roles, autorizaciones y evidencia detallada.

## Reserva configurable

- **Sin reserva:** se registran consumos al ocurrir o al cerrar.
- **Automática:** al iniciar, la aplicación propone capas y cantidades según la receta.
- **Manual:** el responsable elige qué cantidades apartar.

No se exige actualizar el lote cada hora. Los recordatorios son opcionales y el cronómetro registra automáticamente inicio, fin y pausas.

## Criterios de experiencia

- Crear un lote habitual desde una plantilla: menos de 60 segundos después de la configuración inicial.
- Cerrar un lote sin desviaciones: confirmación explícita y menos de dos minutos.
- El atajo “plan igual a real” nunca se ejecuta silenciosamente.
- El uso repetido prioriza plantillas, favoritos y captura por excepción.

