# Calidad y pruebas

## Enfoque

DENTOKLIN utiliza pruebas automatizadas y comprobaciones de build para reducir regresiones en módulos clínicos y administrativos.

## Checkpoint funcional V1 — 23/09/2026

### Backend

- 161 pruebas totales.
- 152 aprobadas.
- 9 omitidas.
- 0 fallidas.
- Exit code 0.

Las 9 pruebas omitidas correspondían a integraciones condicionadas con una instancia MySQL real.

### Frontend

- 22 archivos de prueba.
- 172 pruebas.
- 172 aprobadas.
- 0 fallidas.

### Build

El build del frontend se completó correctamente con Vite.

En ese checkpoint se transformaron 1910 módulos y únicamente se registró una advertencia informativa relacionada con el tamaño de un chunk.

### Git

- `git diff --check`: correcto.
- Working tree limpio al cierre del checkpoint.

## Tipos de validación utilizados

El proyecto combina:

- Pruebas de componentes.
- Pruebas de flujos de interfaz.
- Pruebas de lógica backend.
- Validaciones de reglas de negocio.
- Comprobaciones de build.
- Revisión de integridad antes de integrar cambios.

## Filosofía de cambios

Para módulos ya estabilizados se priorizan cambios pequeños y localizados.

Las reglas de trabajo del proyecto buscan:

1. Evitar reescrituras innecesarias.
2. Mantener contratos existentes.
3. Preservar trazabilidad clínica y financiera.
4. No introducir funcionalidades nuevas durante fases de estabilización sin una decisión explícita.
5. Ejecutar regresión después de cambios relevantes.

## Nota

Las cifras anteriores representan un checkpoint histórico verificable del proyecto, no una promesa de cobertura porcentual ni una afirmación sobre la versión más reciente que pueda existir de forma local.
