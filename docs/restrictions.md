---
sidebar_position: 6
---

# Restricciones y limites

## Alcance

- El CLI funciona como wrapper del API.
- Requiere que el repositorio este conectado en ReviewMind.

## PRs y re-ejecuciones

- `remi analyze` dispara el review del PR indicado.
- `--force` re-ejecuta el review del mismo commit si ya existe.
- Las re-ejecuciones cuentan para el limite de revisiones por PR.

## Limites de plan

- Se aplican los limites del plan (PRs por mes y revisiones por PR).
- Si el limite se alcanza, el CLI devolvera error.

## Credenciales

- El CLI guarda tokens en `~/.remi/config.json`.
- Trata ese archivo como secreto.
