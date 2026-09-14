# Project decisions — QRTE

Decisiones que no se repiten. Una línea por decisión con fecha.
Política: solo repetible, máximo ~30 líneas, obsoleto se marca no se borra. Nada de secrets.

## Formato

- `YYYY-MM-DD` — decisión — motivo corto.

## Decisiones

- `2026-09-10` — pago por tokens por obra, suscripciones legado deprecado — modelo de negocio actual.
- `2026-09-10` — QR firmado HMAC versionado con `public_id` UUID — ficha pública verificable.
- `2026-09-10` — tickets con `TKT-####`, sin auto-envío IA ni auto-cierre — admin decide.
- `2026-09-10` — esquema `solo-prod` en `VPS-01` con hook `migrate` a potestad del admin — deploy simple.
- `2026-09-14` — base de datos renombrada a `qrte` (dump/restore + env Coolify) y vestigios previos purgados — identidad única QRTE.
- `2026-09-14` — dominios enrutados al mismo servicio: `qrte.poordesigner.com` (app) y `arte.poordesigner.com` (fichas/QR); `APP_URL`=qrte, `QRTE_PUBLIC_URL`=`https://arte.poordesigner.com`.
- `2026-09-14` — storage R2 en bucket `qrtebucket` (público `pub-2adb…r2.dev`), migrado desde el bucket previo — nombre alineado a la marca.
