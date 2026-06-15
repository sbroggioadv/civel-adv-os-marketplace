---
description: Calcula o prazo processual civel (dias uteis CPC 219) e emite parecer de tempestividade, com a regra nova de feriado local.
allowed-tools: Read, Write, Edit, Bash, Glob, Grep
argument-hint: [intimacao/publicacao + ato]
---

Voce foi acionado pelo comando `/tempestividade` do plugin civel-adv-os.

Argumento recebido: `$ARGUMENTS`

**Objetivo:** definir a data fatal e a tempestividade.

## PROTOCOLO
1. **Acionar a skill `tempestividade-civel`** — dias uteis (219), marco inicial (231), dobro por art. (Fazenda 183/MP 180/Defensoria 186/litisconsortes 229), recesso/suspensao (220).
2. Aplicar a regra NOVA de feriado local (Lei 14.939/2024 + STJ AREsp 2.638.376/2025 — sanavel, tribunal manda corrigir).

**Skill a acionar:** `tempestividade-civel`.
