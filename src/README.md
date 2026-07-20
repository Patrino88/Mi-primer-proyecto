# Código fuente Flutter

El framework quedó aprobado: Flutter + Dart. Al inicializar F3, el código ejecutable seguirá la convención de Flutter dentro de `lib/`; esta carpeta descriptiva no debe convertirse en una segunda raíz de código.

Organización prevista:

```text
lib/
  app/
  core/
  domain/
  data/
  features/
  platform/
test/
```

El dominio permanece en Dart puro y no depende de widgets. Flutter compone la presentación; Riverpod coordina estado y dependencias; Drift administra SQLite y sus migraciones.
