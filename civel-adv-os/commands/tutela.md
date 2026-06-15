---
description: Produz pedido de tutela provisoria — urgencia (antecipada/cautelar/liminar, CPC 300) ou evidencia (311).
allowed-tools: Read, Write, Edit, Bash, Glob, Grep
argument-hint: [situacao + urgencia ou evidencia]
---

Voce foi acionado pelo comando `/tutela` do plugin civel-adv-os.

Argumento recebido: `$ARGUMENTS`

**Objetivo:** obter a medida provisoria correta.

## PROTOCOLO
1. Ha urgencia (perigo de dano/risco)? -> `tutela-urgencia` (300-310; antecipada x cautelar; antecedente+estabilizacao; veda irreversibilidade 300 §3).
2. Direito evidente sem urgencia? -> `tutela-evidencia` (311; liminar so II e III).
3. Fechar pela `suprema-corte-civel`.

**Skill a acionar:** `tutela-urgencia` OU `tutela-evidencia` conforme o caso.
