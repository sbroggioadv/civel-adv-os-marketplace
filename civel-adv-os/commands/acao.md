---
description: Escolhe e redige a acao civel correta da gama (indenizatoria, fazer/nao fazer, resolucao/revisional contratual, cobranca/monitoria, consignacao, declaratoria, anulatoria, possessorias, usucapiao, reivindicatoria, exigir contas, embargos de terceiro, rescisoria, producao antecipada).
allowed-tools: Read, Write, Edit, Bash, Glob, Grep
argument-hint: [o que o autor quer / descricao do caso]
---

Voce foi acionado pelo comando `/acao` do plugin civel-adv-os.

Argumento recebido: `$ARGUMENTS`

**Objetivo:** identificar a acao civel adequada e redigir a peca certa.

## PROTOCOLO
1. Classificar o objetivo material -> selecionar a skill da Camada 5: reparar dano -> `acao-indenizatoria`; compelir conduta -> `obrigacao-fazer-nao-fazer`; desfazer/revisar contrato -> `resolucao-rescisao-contratual` / `revisional-contratual`; cobrar sem titulo -> `cobranca-e-monitoria`; credor recusa receber -> `consignacao-em-pagamento`; (in)existencia de relacao -> `acao-declaratoria`; vicio do negocio -> `anulatoria-negocio-juridico`; posse -> `possessorias`; propriedade por posse -> `usucapiao-judicial`; reaver coisa -> `reivindicatoria-petitoria`; prestar contas -> `exigir-contas`; bem de terceiro constrito -> `embargos-de-terceiro`; desconstituir coisa julgada -> `acao-rescisoria`; perpetuar prova -> `producao-antecipada-de-provas`.
2. SEMPRE a gestao processual transversal (Camada 2) antes de redigir: `competencia-e-foro`, `valor-da-causa`, `gratuidade-e-impugnacao`, `tempestividade-civel`.
3. Fechar pela `suprema-corte-civel`.

**Skill a acionar:** a acao correspondente (Camada 5) + gestao processual (Camada 2). Em duvida, deixe `civel-master` dirimir.
