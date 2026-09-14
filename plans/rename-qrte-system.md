# System — consolidación de marca QRTE (fases 1-2 hechas)

- Track: `System`. Readiness: `ready` para cierre; infra e integraciones por verificar con el admin.
- Objetivo: consolidar todo bajo la marca QRTE en código, repo, VPS e integraciones, sin referencias previas en el árbol.
- Fase 1 — repo/remoto (hecha 2026-09-11): repo GitHub `poordesigner/qrte` + remoto local + redeploy validado.
- Fase 2 — código (hecha): `config/qrte.php`, envs `QRTE_*`, textos y rutas. Árbol sin referencias previas (`git grep` limpio).
- Fase 3 — VPS/dominio: `qrte.poordesigner.com` resuelve al VPS; confirmar en Coolify dominio + `APP_URL` con el admin.
- Fase 4 — marca/integraciones: `AGENTS.md` y `REGISTRO.md` ya en QRTE; verificar con el admin Paddle, Chatwoot y R2 público.
- Nota de datos: la base de datos conserva su nombre histórico; su renombre se trata en plan aparte (operación en VPS).
- Verificación: árbol sin referencias previas, `AGENTS.md` < 200 líneas, punteros `{gestor}` válidos, cero secrets.
