# Arquitectura conceptual

La arquitectura definitiva y el framework móvil se aprobarán al abrir F3. Esta estructura evita acoplar reglas financieras a una interfaz específica.

## Capas previstas

| Capa | Responsabilidad |
|---|---|
| Presentación | Pantallas, navegación, accesibilidad y modo discreto |
| Aplicación | Casos de uso, validaciones y coordinación de operaciones |
| Dominio | Movimientos, cuentas, compromisos, periodos y reglas financieras |
| Datos | Persistencia local, migraciones, importación y exportación |
| Plataforma | Calendario, conectividad, archivos, reloj y capacidades del dispositivo |

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

