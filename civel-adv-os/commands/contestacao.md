---
description: Produz a contestacao civel com toda a defesa em peca unica (CPC 335-342) — preliminares (337), impugnacao especifica, merito, reconvencao se cabivel.
allowed-tools: Read, Write, Edit, Bash, Glob, Grep
argument-hint: [contexto da defesa]
---

Voce foi acionado pelo comando `/contestacao` do plugin civel-adv-os.

Argumento recebido: `$ARGUMENTS`

**Objetivo:** redigir a defesa do reu.

## PROTOCOLO
1. **Tempestividade** primeiro (`tempestividade-civel` — 15 dias uteis, art. 335).
2. **Acionar a skill `contestacao-civel`** — `preliminares-civel` (337) + impugnacao especifica (341, fato nao impugnado presume-se verdadeiro) + merito + `reconvencao` se cabivel.
3. Fechar pela `suprema-corte-civel` (confere se nenhuma preliminar foi esquecida).

**Skill a acionar:** `contestacao-civel`.
