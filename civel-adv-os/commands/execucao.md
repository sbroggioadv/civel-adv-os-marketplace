---
description: Defende o executado e conduz a execucao no que e do contencioso civel — escolha da via de defesa, penhora/expropriacao (SISBAJUD/RENAJUD/INFOJUD), IDPJ e fraude a execucao, medidas executivas atipicas (CPC 139 IV).
allowed-tools: Read, Write, Edit, Bash, Glob, Grep
argument-hint: [situacao da execucao / lado executado]
---

Voce foi acionado pelo comando `/execucao` do plugin civel-adv-os.

Argumento recebido: `$ARGUMENTS`

**Objetivo:** atuar na execucao com a via correta.

## PROTOCOLO
1. EXECUTADO que se defende -> `defesa-do-executado` (escolhe entre embargos a execucao 914-920 para titulo extrajudicial, impugnacao 525 para titulo judicial, ou pre-executividade para materia de ordem publica).
2. Constricao patrimonial -> `penhora-e-expropriacao` (833 impenhoraveis, 835 ordem, 854 SISBAJUD, leilao).
3. Atingir socio / patrimonio blindado -> `idpj-e-fraude-a-execucao` (IDPJ 133-137, CC 50, fraude a execucao 792, pauliana 158-165).
4. Devedor contumaz -> `medidas-executivas-atipicas` (CPC 139 IV, com proporcionalidade e contraditorio).
5. Cross-link: execucao pesada/leilao completo -> `execucao-adv-os`; calculos -> `calculosjudiciais-adv-os`. Fechar pela `suprema-corte-civel`.

**Skill a acionar:** a skill da Camada 7 conforme o passo. Em duvida, `civel-master` dirime.
