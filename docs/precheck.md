---
sidebar_position: 4
---

# Precheck (Semgrep + Linters)

El CLI puede enviar un JSON con resultados de linters/semgrep para mezclar con el precheck interno.

## Ejemplo

```bash
remi analyze --repo <repoId> --pr PR-142 --precheck ./semgrep.json
```

La plantilla esta en `examples/semgrep.json` dentro del repo.

## Mapeo de severidades

- `ERROR` / `CRITICAL` / `BLOCKER` -> `critical`
- `WARNING` / `HIGH` / `MAJOR` -> `warning`
- `INFO` / `LOW` / `MINOR` -> `suggestion`
