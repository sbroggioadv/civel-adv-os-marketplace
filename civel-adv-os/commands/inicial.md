---
description: Produz a peticao inicial civel pelo rito comum (CPC 319-321), com gestao processual (competencia/foro, valor da causa, gratuidade) e tutela se cabivel.
allowed-tools: Read, Write, Edit, Bash, Glob, Grep
argument-hint: [fatos + pedido]
---

Voce foi acionado pelo comando `/inicial` do plugin civel-adv-os.

Argumento recebido: `$ARGUMENTS`

**Objetivo:** redigir a peticao inicial.

## PROTOCOLO
1. Gestao processual ANTES: `competencia-e-foro`, `valor-da-causa`, `gratuidade-e-impugnacao`.
2. **Acionar a skill `peticao-inicial-civel`** — pedido certo/determinado, cumulacao, tutela (cross-link `tutela-urgencia`/`tutela-evidencia`) se houver urgencia/evidencia.
3. Fechar pela `suprema-corte-civel`.

**Skill a acionar:** `peticao-inicial-civel` (orquestrada pelo `civel-master`).
