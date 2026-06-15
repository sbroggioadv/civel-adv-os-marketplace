# Metodologia Cível — Mapa de Uso do Plugin

> Anexo central. O `civel-master` lê este arquivo primeiro. Define como as skills se articulam, qual anexo cada uma usa, o fluxo processual e as regras de ouro.

## Arquitetura (9 camadas + QA) — 64 skills (completo)
- **Camada 0 — Orquestração/QA:** `civel-master`, `civel-onboarding`, `triagem-civel`, `memoria-de-caso-civel`, `estilo-civel`, `suprema-corte-civel`.
- **Camada 1 — Fundação:** `base-legal-cpc`, `base-legal-cc`, `jurisprudencia-civel`, `validador-civel`.
- **Camada 2 — Gestão processual transversal:** `tempestividade-civel`, `gratuidade-e-impugnacao`, `competencia-e-foro`, `preliminares-civel`, `valor-da-causa`, `estrategia-processual`, `cronologia-e-providencias`.
- **Camada 3 — Tutelas:** `tutela-urgencia`, `tutela-evidencia`.
- **Camada 4 — Conhecimento/1º grau:** `peticao-inicial-civel`, `emenda-inicial`, `contestacao-civel`, `reconvencao`, `replica-civel`, `revelia`, `saneamento`, `producao-de-provas`, `audiencia-conciliacao-mediacao`, `audiencia-instrucao`, `razoes-finais-memoriais`, `resumo-de-ata`.
- **Camada 5 — Ações cíveis:** `acao-indenizatoria`, `obrigacao-fazer-nao-fazer`, `resolucao-rescisao-contratual`, `revisional-contratual`, `cobranca-e-monitoria`, `consignacao-em-pagamento`, `acao-declaratoria`, `anulatoria-negocio-juridico`, `possessorias`, `usucapiao-judicial`, `reivindicatoria-petitoria`, `exigir-contas`, `embargos-de-terceiro`, `acao-rescisoria`, `producao-antecipada-de-provas`.
- **Camada 6 — Recursos:** `embargos-de-declaracao`, `agravo-de-instrumento`, `agravo-interno`, `apelacao-civel`, `recursos-excepcionais`, `agravo-em-recurso-excepcional`, `admissibilidade-e-tempestividade-recursal`, `contrarrazoes`.
- **Camada 7 — Cumprimento & Execução:** `cumprimento-de-sentenca`, `impugnacao-ao-cumprimento`, `penhora-e-expropriacao`, `defesa-do-executado`, `idpj-e-fraude-a-execucao`, `medidas-executivas-atipicas`.
- **Camada 8 — Incidentes:** `suspeicao-impedimento`, `conflito-de-competencia`, `irdr-iac`, `incidentes-probatorios-e-exibicao`.

## Anexos de `context/`
| Anexo | Conteúdo | Como usar |
|---|---|---|
| `cpc-13105-15.md` | CPC/2015 consolidado (~845KB) | **grep o artigo** + ler a faixa (não ler inteiro) |
| `cc-10406-02.md` | CC/2002 consolidado (~750KB) | idem |
| `cpc-cc-alteracoes-recentes.md` | Reformas 2024-2026 + status PL 4/2025 | ler sempre antes de citar artigo alterado |
| `jurisprudencia-civel.md` | Súmulas/temas/enunciados verificados (✅/🟡/❌) | só citar ✅; 🟡 conferir; nunca ❌ |
| `recursos-tutelas-civel.md` | Recursos (cabimento/prazo/preparo/efeito) + tutelas | base das Camadas 3 e 6 |

## Fluxo processual (conduzido pelo `civel-master`)
```
triagem-civel (fase + objetivo) → memoria-de-caso-civel (estado) →
[SEMPRE] gestão processual: tempestividade · gratuidade · competência/foro · preliminares · valor da causa →
skill da fase: inicial → (emenda) → contestação+preliminares → réplica → saneamento → provas → audiências → razões finais → sentença →
recursos (ED/agravo/apelação/excepcionais) conforme a decisão →
cumprimento/execução (Camada 7) · incidentes quando surgirem (Camada 8) → suprema-corte-civel (R1-R4) em TODA entrega
```

## Regras de ouro
1. **Gestão processual transversal é obrigatória** em toda peça (o "não esquecer nada"): tempestividade, gratuidade+impugnação, competência/foro, preliminares (CPC 337), valor da causa.
2. **Prazos em dias úteis** (CPC 219); regra 15 dias; ED 5 dias; dobro por art. (Fazenda 183 / MP 180 / Defensoria 186 / litisconsortes 229).
3. **Lei vigente:** CC/2002 (PL 4/2025 só monitorar) · CPC + Lei 14.879/2024 (foro) + Lei 14.939/2024 (feriado local) · EC 136 = precatórios (não CPC).
4. **Competência/foro correto** em R1. **Anti-alucinação** via `validador-civel`. **Gate final** `suprema-corte-civel`.
5. **Cross-link, não duplicar:** execução pesada → `execucao-adv-os`; revisional bancária → `bancario-adv-os`; cálculos → `calculosjudiciais-adv-os`; família → `direito-familia-adv-os`.
