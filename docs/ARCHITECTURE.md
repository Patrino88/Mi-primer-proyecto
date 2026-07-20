# Arquitectura Flutter aprobada

F3 utiliza Flutter y Dart. Android es el primer destino verificable, pero la interfaz y el dominio se preparan para móvil, tableta y escritorio sin duplicar reglas financieras.

## Tecnología base

| Componente | Elección |
|---|---|
| Interfaz multiplataforma | Flutter + Dart |
| Estado y dependencias | Riverpod |
| Navegación | go_router |
| Persistencia | Drift sobre SQLite |
| Dominio | Dart puro, independiente de Flutter |
| Estrategia | Local primero, migraciones versionadas y módulos bajo demanda |

## Capas previstas

| Capa | Responsabilidad |
|---|---|
| Presentación | Pantallas, navegación, accesibilidad y modo discreto |
| Aplicación | Casos de uso, validaciones y coordinación de operaciones |
| Dominio | Movimientos, cuentas, compromisos, periodos y reglas financieras |
| Datos | Persistencia local, migraciones, importación y exportación |
| Plataforma | Calendario, conectividad, archivos, reloj y capacidades del dispositivo |

## Estructura prevista

```text
lib/
  app/
  core/
  domain/
  data/
  features/
  platform/
test/
docs/
```

## Módulos personales

- Inicio ejecutivo
- Captura y movimientos
- Cuentas y tarjetas
- Compromisos y presupuestos
- Calendario financiero
- Ahorros e inversiones
- Reportes y exportación
- Configuración, privacidad y respaldo

## Reglas estructurales

- El dominio no depende de componentes visuales.
- Los cálculos monetarios usan representación decimal segura.
- Cada movimiento tiene identificador único y marca temporal de alta precisión.
- Editar o anular conserva trazabilidad.
- Los saldos pueden ser positivos, cero o negativos.
- Los datos personales y empresariales permanecen separados.
- Las integraciones externas se encapsulan y pueden desactivarse.
- Los módulos opcionales existen en el registro de código, pero sus rutas y pantallas sólo aparecen cuando se activan.
