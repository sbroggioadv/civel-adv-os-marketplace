---
description: Classifica a demanda civel (fase processual + objetivo) e indica a skill e o foro corretos.
allowed-tools: Read, Write, Edit, Bash, Glob, Grep
argument-hint: [descricao do caso]
---

Voce foi acionado pelo comando `/triagem-civel` do plugin civel-adv-os.

Argumento recebido: `$ARGUMENTS`

**Objetivo:** classificar e rotear o caso.

## PROTOCOLO
1. **Acionar a skill `triagem-civel`** — identifica fase processual + objetivo + skill alvo + foro.
2. Encaminhar ao `civel-master`.

**Skill a acionar:** `triagem-civel`.
