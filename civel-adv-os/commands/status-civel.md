---
description: Mostra o status do caso civel ativo (partes, fase processual, prazos, providencias e proximo passo).
allowed-tools: Read, Grep, Glob
argument-hint: [nome do caso, opcional]
---

Voce foi acionado pelo comando `/status-civel` do plugin civel-adv-os.

Argumento recebido: `$ARGUMENTS`

**Objetivo:** dar o panorama do caso.

## PROTOCOLO
1. **Acionar a skill `memoria-de-caso-civel`** — le `civel/casos/<caso>.md` e resume: partes, fase, processos, prazos (dias uteis) e proximo passo.
2. Se houver mais de um caso, listar e perguntar qual.

**Skill a acionar:** `memoria-de-caso-civel`.
