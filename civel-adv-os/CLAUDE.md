# CLAUDE.md — civel-adv-os (Civil Litigation Master)

> Estende o CLAUDE.md global/workspace. Regras locais do plugin de contencioso cível.

## Regras invioláveis do plugin
1. **Sempre consultar `context/` antes de redigir.** CPC/2015, CC/2002, reformas, jurisprudência e recursos/tutelas vivem nos anexos — os arquivos são grandes (CPC ~845KB, CC ~750KB): **localizar o artigo por busca (grep) e ler a faixa**, não despejar o anexo inteiro. Cada skill lista seus anexos.
2. **`civel-master` dirime TODAS as skills** pertinentes à tarefa, sem esquecer nenhuma. Nunca produzir peça sem antes passar pela gestão processual transversal (tempestividade, gratuidade, competência/foro, preliminares, valor da causa).
3. **Gate Suprema Corte.** Antes de QUALQUER entrega, `suprema-corte-civel` (R1 fatos/competência/foro · R2 fundamentação vigente · R3 jurisprudência real · R4 forma/pedidos/tempestividade/valor/gratuidade).
4. **Anti-alucinação.** Nenhum dispositivo/súmula/tese/acórdão entra em peça sem `validador-civel` (cruza `context/` + guard global `anti-alucinacao-juridica`). Na dúvida, bloquear e checar ao vivo.
5. **Lei vigente (jun/2026) — não errar:**
   - CC/2002 **vigente**; a Reforma do CC é o **PL 4/2025 EM TRAMITAÇÃO** — NÃO citar como lei.
   - **Lei 14.879/2024** mudou o foro de eleição (CPC art. 63 §1º/§5º — exige pertinência; juízo aleatório = abuso).
   - **Lei 14.939/2024** mudou o feriado local na admissibilidade (CPC art. 1.003 §6º) + STJ Corte Especial AREsp 2.638.376 (2025): não é mais intempestividade automática — tribunal manda corrigir.
   - **EC 136/2025 = precatórios** (CF 100/165), **NÃO altera o CPC**.
   - Prazos em **dias úteis** (CPC 219); regra geral 15 dias; ED 5 dias; dobro Fazenda(183)/MP(180)/Defensoria(186)/litisconsortes(229, não em autos eletrônicos).
6. **Foco: contencioso.** Fronteiras: consumidor/família/sucessões fora; execução pesada/bancário/cálculos = cross-link (não duplicar).

## Porta única
`civel-master` é o orquestrador: classifica via `triagem-civel` (fase processual + objetivo), carrega `memoria-de-caso-civel`, seleciona e conduz todas as skills, e fecha pela `suprema-corte-civel`.
