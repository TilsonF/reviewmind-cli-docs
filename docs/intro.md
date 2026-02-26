---
sidebar_position: 1
slug: /
---

# remi CLI

`remi` es el CLI oficial de ReviewMind para disparar revisiones, consultar estado y descargar reportes sin entrar a la UI.

## Casos de uso

- Re-ejecutar una review del mismo PR/commit (recheck).
- Forzar análisis si el webhook falla.
- Análisis manual/local antes de abrir PR.
- Descargar reportes en Markdown desde CI.

## Requisitos

- Node.js 18+
- Acceso a la API de ReviewMind

## Primeros pasos

```bash
npm install -g remi-cli
remi login --api https://api.reviewmindai.com
```
