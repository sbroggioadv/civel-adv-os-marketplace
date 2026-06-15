---
description: Prepara audiencia civel — conciliacao/mediacao (CPC 334) ou instrucao e julgamento (358-368, roteiro + inquiricao).
allowed-tools: Read, Write, Edit, Bash, Glob, Grep
argument-hint: [tipo de audiencia + caso]
---

Voce foi acionado pelo comando `/audiencia` do plugin civel-adv-os.

Argumento recebido: `$ARGUMENTS`

**Objetivo:** preparar a audiencia.

## PROTOCOLO
1. Conciliacao/mediacao (334)? -> `audiencia-conciliacao-mediacao`.
2. Instrucao e julgamento? -> `audiencia-instrucao` (ordem das provas, inquiricao de testemunhas, depoimento pessoal, alegacoes finais orais).
3. Apos a audiencia, `resumo-de-ata` extrai deliberacoes/prazos/providencias.

**Skill a acionar:** `audiencia-conciliacao-mediacao` OU `audiencia-instrucao`.
