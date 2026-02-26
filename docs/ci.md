---
sidebar_position: 5
---

# CI / CD

Ejemplo minimo para fallar el pipeline si hay criticos:

```bash
remi analyze --repo <repoId> --pr PR-142 --wait --fail-on critical
```

Codigos de salida:

- 0: sin hallazgos segun el nivel elegido
- 1: error general o timeout
- 2: hallazgos en el nivel configurado
