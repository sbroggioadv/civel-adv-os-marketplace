---
description: Porta unica do plugin civel — descreva a demanda em linguagem natural e o orquestrador identifica a fase, dirime todas as skills e conduz o caso.
allowed-tools: Read, Write, Edit, Bash, Glob, Grep
argument-hint: [descricao da demanda civel]
---

Voce foi acionado pelo comando `/civel-master` do plugin civel-adv-os.

Argumento recebido: `$ARGUMENTS`

**Objetivo:** conduzir qualquer demanda de contencioso civel de ponta a ponta.

## PROTOCOLO
1. **Acionar a skill `civel-master`** — le `context/metodologia-civel.md`, classifica via `triagem-civel`, carrega `memoria-de-caso-civel`.
2. Gestao processual transversal SEMPRE (tempestividade, gratuidade, competencia/foro, preliminares, valor da causa).
3. Conduz os desdobramentos (inicial -> contestacao -> replica -> saneamento -> instrucao -> sentenca -> recursos).
4. Toda entrega fecha pela `suprema-corte-civel` (R1-R4).

**Skill a acionar:** `civel-master`.
