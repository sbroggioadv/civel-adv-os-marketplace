---
description: Suscita o incidente processual correto — suspeicao/impedimento do juiz (CPC 144-148), conflito de competencia (66, 951-959), IRDR/IAC (976-987, 947), exibicao de documento ou coisa e arguicao de falsidade (396-404, 430-433).
allowed-tools: Read, Write, Edit, Bash, Glob, Grep
argument-hint: [incidente / situacao processual]
---

Voce foi acionado pelo comando `/incidente` do plugin civel-adv-os.

Argumento recebido: `$ARGUMENTS`

**Objetivo:** suscitar o incidente certo, na forma e prazo corretos.

## PROTOCOLO
1. Juiz parcial/impedido -> `suspeicao-impedimento` (144 impedimento objetivo / 145 suspeicao / 146 prazo 15 dias).
2. Dois juizes se dizem (in)competentes -> `conflito-de-competencia` (66, suscitacao 951-959).
3. Multiplos processos iguais / tese vinculante regional -> `irdr-iac` (IRDR 976-987, IAC 947, vinculacao 927 III).
4. Parte/terceiro esconde documento ou documento falso -> `incidentes-probatorios-e-exibicao` (exibicao 396-404, falsidade 430-433).
5. Fechar pela `suprema-corte-civel`.

**Skill a acionar:** a skill de incidente correspondente (Camada 8).
