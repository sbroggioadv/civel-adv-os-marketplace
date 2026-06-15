---
description: Escolhe e redige o recurso civel correto (ED, agravo de instrumento, agravo interno, apelacao, REsp/RE) com admissibilidade e tempestividade.
allowed-tools: Read, Write, Edit, Bash, Glob, Grep
argument-hint: [decisao a recorrer]
---

Voce foi acionado pelo comando `/recurso` do plugin civel-adv-os.

Argumento recebido: `$ARGUMENTS`

**Objetivo:** recorrer da decisao correta, no recurso certo.

## PROTOCOLO
1. Identificar a decisao: vicio (omissao/contradicao) -> `embargos-de-declaracao` (5 dias); interlocutoria do rol 1.015 -> `agravo-de-instrumento`; monocratica -> `agravo-interno`; sentenca -> `apelacao-civel`; ultima instancia vs lei federal/CF -> `recursos-excepcionais` (REsp = CF 105 III / RE = CF 102 III); inadmissao de REsp/RE -> `agravo-em-recurso-excepcional`.
2. SEMPRE `admissibilidade-e-tempestividade-recursal` (cabimento, prazo, preparo) + `tempestividade-civel` (feriado local regra nova Lei 14.939/2024).
3. Fechar pela `suprema-corte-civel`.

**Skill a acionar:** o recurso correspondente + `admissibilidade-e-tempestividade-recursal`.
