Mode: production

# civel-adv-os — Civil Litigation Master

Plugin Claude Code de **contencioso cível brasileiro** — o sistema operacional do litígio cível, do ajuizamento ao trânsito em julgado. Orquestrador **`civel-master`** que dirige (dirime) **todas** as skills necessárias por tarefa, sem esquecer nenhuma.

> Onboarding: **`/start-civel`**. Porta única: **`civel-master`**.

## Cobertura (v0.1 — núcleo)
- **Conhecimento / 1º grau:** petição inicial, emenda, contestação + preliminares, reconvenção, réplica, revelia, saneamento, provas, audiências (conciliação/instrução), razões finais, sentença, resumo de ata.
- **Tutelas:** urgência (antecipada/cautelar/antecedente/estabilização) e evidência.
- **Recursos:** ED, agravo de instrumento, agravo interno, apelação, REsp/RE + repercussão geral/repetitivos, agravo em recurso excepcional, admissibilidade/tempestividade, contrarrazões.
- **Gestão processual transversal (o "não esquecer nada"):** tempestividade, gratuidade + impugnação, competência/foro, preliminares (CPC 337), valor da causa, estratégia, cronologia/providências.
- **Material:** responsabilidade civil, contratos/obrigações, direitos reais (fundamento das peças).

> **v0.2 (próxima):** a gama de ações específicas (indenizatória, obrigação de fazer/não fazer, possessórias, usucapião, anulatória, etc.), cumprimento/execução e incidentes.

## Fundação jurídica enraizada (`context/`)
CPC/2015 + CC/2002 consolidados · reformas recentes (Lei 14.879/2024 foro de eleição; Lei 14.939/2024 feriado local; EC 136/2025 = precatórios, não altera o CPC; PL 4/2025 da Reforma do CC **em tramitação** — só monitorar) · jurisprudência STJ/STF + enunciados CJF/FPPC · recursos e tutelas.

## Fronteiras
Consumidor (CDC), Família, Sucessões = **fora** (cross-link onde existe). Execução pesada/cobrança/monitória → `execucao-adv-os`. Revisional bancária → `bancario-adv-os`. Cálculos → `calculosjudiciais-adv-os`. **Foco: o que não está nos outros plugins.**

## Comandos principais
`/start-civel` · `/civel-master` · `/triagem-civel` · `/inicial` · `/contestacao` · `/tutela` · `/recurso` · `/tempestividade` · `/gratuidade` · `/audiencia` · `/revisao-final` · `/status-civel`
