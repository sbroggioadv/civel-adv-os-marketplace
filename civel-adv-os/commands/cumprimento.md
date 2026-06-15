---
description: Conduz o cumprimento de sentenca (CPC 513-538) do lado do credor — intimacao para pagar em 15 dias, multa 10% + honorarios 10%, penhora — ou a impugnacao do lado do executado (CPC 525).
allowed-tools: Read, Write, Edit, Bash, Glob, Grep
argument-hint: [titulo judicial / lado credor ou executado]
---

Voce foi acionado pelo comando `/cumprimento` do plugin civel-adv-os.

Argumento recebido: `$ARGUMENTS`

**Objetivo:** efetivar (ou impugnar) o titulo judicial.

## PROTOCOLO
1. Identificar o lado: CREDOR que quer receber -> `cumprimento-de-sentenca` (523: 15 dias, multa 10% + honorarios 10%, penhora; alimentos 528; Fazenda 534-535); EXECUTADO que quer se defender -> `impugnacao-ao-cumprimento` (525 §1 I-VII; efeito suspensivo so com garantia + grave dano §6).
2. Calculo do debito atualizado -> cross-link `calculosjudiciais-adv-os` (memoria de calculo).
3. Gestao processual (tempestividade em dias uteis) + fechar pela `suprema-corte-civel`.

**Skill a acionar:** `cumprimento-de-sentenca` ou `impugnacao-ao-cumprimento`.
