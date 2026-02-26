---
sidebar_position: 3
---

# Comandos

## login

```bash
remi login --api https://api.reviewmindai.com
```

Guarda tokens en `~/.remi/config.json`.

## analyze

```bash
remi analyze --repo <repoId> --pr PR-142 --wait --fail-on critical
```

Opciones:

- `--force` re-ejecuta el review del mismo commit.
- `--precheck` envia JSON de linters/semgrep.
- `--wait` espera hasta que exista review.

## status

```bash
remi status --repo <repoId> --pr PR-142
```

## report

```bash
remi report --review <reviewId> --out reporte.md
```
