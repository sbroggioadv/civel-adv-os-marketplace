# Jurisprudência e Enunciados — Contencioso Cível (plugin `civel-master` v0.1)

> Pesquisa realizada em 2026-06-15 via firecrawl (busca + scrape de fontes oficiais).
> **Regra anti-alucinação:** só entrou aqui o que foi EFETIVAMENTE encontrado com link de fonte real (STJ, CJF, TJDFT, Jusbrasil, JOTA, Migalhas). Cada item traz órgão/número, tese em 1-2 linhas e link. O que não foi encontrado/confirmado está marcado **⚠️ NÃO CONFIRMADO** ou **❌ NÃO ENCONTRADO**.
> **Status de verificação:** ✅ = fonte primária oficial scrapeada/confirmada · 🟡 = confirmado por fonte secundária confiável (TJDFT/Jusbrasil/JOTA/Migalhas), conferir inteiro teor antes de citar em peça.
> Escopo v0.1: procedimento comum · prazos · tutelas · recursos · responsabilidade civil · gratuidade.

---

## ⚡ ALERTA DE REFORMA RECENTE (pós-corte jan/2026) — LER ANTES DE USAR

**Lei 14.939/2024 — feriado local na interposição do recurso.** Alterou o CPC (art. 1.003, §6º — confirmado em fonte primária; possivelmente também o art. 1.029, §3º, **conferir inteiro teor** no anexo `cpc-cc-alteracoes-recentes.md`). Antes: o feriado local tinha de ser comprovado **no ato da interposição**, sob pena de intempestividade (entendimento do EREsp/REsp 1.813.684-SP). Agora: se o recorrente não comprovar, **o tribunal DEVE intimar para corrigir a falha** (ou desconsiderar a omissão se a info já consta no processo eletrônico). O STJ (Corte Especial, AREsp 2.638.376, rel. Min. Antonio Carlos Ferreira, j. 11/02/2025) decidiu que a nova lei é **aplicável até a recursos interpostos antes de sua vigência** (natureza processual, aplicação imediata — art. 14 CPC), inclusive em agravos internos/regimentais contra decisões que negaram seguimento por falta da comprovação.
→ Fonte: https://www.stj.jus.br/sites/portalp/Paginas/Comunicacao/Noticias/2025/12022025-Corte-Especial-define-que-nova-regra-sobre-feriado-local-se-aplica-a-recursos-ja-interpostos.aspx (✅ scrapeado)
→ Lei: https://www.planalto.gov.br/ccivil_03/_ato2023-2026/2024/lei/L14939.htm
**Impacto no plugin:** a skill de tempestividade NÃO pode mais ensinar "comprove feriado local no ato sob pena de intempestividade" como regra absoluta — virou dever de correção do tribunal (primazia do mérito).

---

## TEMA 1 — Tutela de urgência / evidência (300, 311; fungibilidade; estabilização 304)

### 1.1 Tutela de urgência — requisitos (CPC 300)
- **Lei seca (CPC art. 300):** probabilidade do direito + perigo de dano ou risco ao resultado útil do processo. §3º: não se concede se houver perigo de irreversibilidade dos efeitos. Fonte primária no arquivo `cpc-13105-15.md`.
- 🟡 **Enunciado 40 — I Jornada Dir. Proc. Civil (CJF):** "A irreversibilidade dos efeitos da tutela de urgência não impede sua concessão, em se tratando de direito provável, cuja lesão seja irreversível." → mitiga o §3º do art. 300. Fonte: PDF I Jornada CJF (✅ scrapeado, p. abaixo).
- 🟡 **Enunciado 41 — I Jornada (CJF):** em processos sobrestados por repetitivo, é possível apreciar e efetivar tutela provisória de urgência.

### 1.2 Tutela de evidência (CPC 311)
- **Lei seca:** concedida **independentemente de perigo de dano** (I abuso de direito de defesa/propósito protelatório; II tese em repetitivo/súmula vinculante + prova documental; III contrato de depósito; IV petição instruída com prova documental suficiente sem dúvida razoável e sem prova capaz de gerar dúvida). Incisos **II e III** permitem **liminar** (art. 311, par. unico — NAO o inciso IV). → `cpc-13105-15.md`.
- 🟡 **Enunciado 47 — I Jornada (CJF):** "A probabilidade do direito constitui requisito para concessão da tutela da evidência fundada em abuso do direito de defesa ou em manifesto propósito protelatório da parte contrária."
- 🟡 **Enunciado 48 — I Jornada (CJF):** tutela de evidência do art. 311, II, cabe também em **tese de repercussão geral ou súmula de tribunal superior** (não só repetitivo).
- 🟡 **Enunciado 49 — I Jornada (CJF):** a tutela da evidência pode ser concedida em mandado de segurança.
- Fonte TJDFT (jurisprudência consolidada): https://www.tjdft.jus.br/consultas/jurisprudencia/jurisprudencia-em-temas/novo-codigo-de-processo-civil/tutela-provisoria-da-evidencia 🟡

### 1.3 Fungibilidade das tutelas
- 🟡 **Enunciado 45 — I Jornada (CJF):** "Aplica-se às tutelas provisórias o princípio da fungibilidade, devendo o juiz esclarecer as partes sobre o regime processual a ser observado." (✅ extraído do PDF oficial CJF)
- Base legal: CPC art. 305, parágrafo único (fungibilidade cautelar→antecipada).

### 1.4 Estabilização da tutela antecipada antecedente (CPC 304) — ⚠️ DIVERGÊNCIA STJ
- **Regra (art. 304 caput):** a tutela antecipada antecedente (art. 303) torna-se **estável** se da decisão concessiva **não for interposto o respectivo recurso**; o processo é extinto.
- ⚠️ **Divergência sobre o que impede a estabilização:**
  - **STJ, 3ª Turma — REsp 1.760.966-SP, rel. Min. Marco Aurélio Bellizze (Informativo 639):** interpretação AMPLIADA — a **mera contestação (qualquer impugnação séria do réu)** é apta a impedir a estabilização, ainda que não seja "recurso" em sentido estrito. Não basta a literalidade de "recurso".
    → Informativo 639 STJ: https://ww2.stj.jus.br/jurisprudencia/externo/informativo/?aplicacao=informativo&acao=pesquisar&livre=@CNOT='016886' 🟡
    → JOTA: https://www.jota.info/justica/contestacao-serve-para-impedir-estabilizacao-tutela-antecipada 🟡
  - **Corrente literal (parte da doutrina / decisões da 1ª Turma):** só o **recurso (agravo de instrumento)** impede a estabilização; contestação não basta.
    → Buscador Dizer o Direito (resumo da divergência): https://buscadordizerodireito.com.br/jurisprudencia/6256/ 🟡 (fonte bot-protected — confirmar inteiro teor)
  - **Postura honesta para a skill:** avisar que há racha; a tese majoritária recente (3ª Turma, REsp 1.760.966) admite contestação para impedir, mas a estratégia segura para quem QUER impedir é interpor **agravo de instrumento** (não confiar só na contestação).
- 🟡 **Enunciado 43 — I Jornada (CJF):** não ocorre estabilização da tutela antecedente quando deferida em **ação rescisória**.
- 🟡 **Enunciado 33 — II Jornada (CJF):** é possível a estabilização de tutela antecipada antecedente **em face da Fazenda Pública** (citado em compilação Jusbrasil — conferir número exato na II Jornada antes de citar).

---

## TEMA 2 — Gratuidade de justiça

### 2.1 Pessoa jurídica — Súmula 481/STJ ✅
- **Súmula 481 STJ:** "Faz jus ao benefício da justiça gratuita a pessoa jurídica com ou sem fins lucrativos que demonstrar sua impossibilidade de arcar com os encargos processuais."
- → PF goza de **presunção**; PJ **NÃO** — precisa **provar** a impossibilidade (não basta declarar).
- Fonte primária (PDF STJ): https://www.stj.jus.br/docs_internet/revista/eletronica/stj-revista-sumulas-2017_43_capSumulas481-485.pdf ✅
- Aplicação TJDFT: https://www.tjdft.jus.br/consultas/jurisprudencia/jurisprudencia-em-temas/novo-codigo-de-processo-civil/gratuidade-de-justica-da-pessoa-juridica-2012-prova-da-hipossuficiencia 🟡

### 2.2 Pessoa física — presunção relativa (CPC 99, §3º)
- **CPC art. 99, §3º:** presume-se verdadeira a alegação de insuficiência deduzida exclusivamente por pessoa natural. → **presunção RELATIVA** (pode ser afastada por prova em contrário; o juiz pode exigir comprovação se houver elementos nos autos que indiquem capacidade — CPC 99 §2º).
- STJ reafirma natureza relativa da presunção (pode ser revogada quando o contexto probatório apontar capacidade). Fonte: https://www.sturzeneggerecavalcante.com.br/decisoes/stj-reafirma-o-entendimento-do-texto-legal-de-que-a-declaracao-de-hipossuficiencia... 🟡 / TJDFT: https://www.tjdft.jus.br/consultas/jurisprudencia/jurisprudencia-em-temas/novo-codigo-de-processo-civil/pn-1 🟡
- ⚠️ **NÃO CONFIRMADO** número de Tema/REsp repetitivo específico fixando critério objetivo (há julgamento na Corte Especial em 2023 — REsp pendente; relator votou por afastar critérios objetivos puramente numéricos). Não citar número até confirmar trânsito/afetação.

### 2.3 Impugnação à gratuidade — ônus da prova
- **CPC art. 100:** a parte contrária pode impugnar; **CPC art. 99 §2º** exige fundamento da revogação.
- **Ônus da prova é do IMPUGNANTE:** quem impugna a gratuidade deve comprovar a capacidade financeira do beneficiário; não basta alegar. Entendimento consolidado STJ/tribunais.
- Fontes: https://elpidiodonizetti.com.br/gratuidade-da-justica-comprovacao-impugnacao-e-recursos/ 🟡 / https://www.cognijus.com/blog/onus-da-prova-na-impugnacao-a-gratuidade-judiciaria-e-sua-nulidade... 🟡 / Jusbrasil (acórdãos): https://www.jusbrasil.com.br/jurisprudencia/busca?q=%C3%B4nus+da+prova+ao+impugnante 🟡
- Revogabilidade: STJ admite revogação do benefício mesmo após concessão, se sobrevier prova de capacidade. TJPR (com citação STJ): https://portal.tjpr.jus.br/jurisprudencia/j/4100000025709281/Ac 🟡

---

## TEMA 3 — Tempestividade recursal

### 3.1 Feriado local na interposição — ⚡ ver ALERTA DE REFORMA no topo (Lei 14.939/2024)
- **Entendimento ANTERIOR (superado pela lei):** STJ, Corte Especial, **REsp 1.813.684-SP** — exigia comprovação do feriado local **no ato de interposição**, sem possibilidade de comprovação posterior (modulado para recursos interpostos após 18/11/2019).
  → Informativos Trilhante: https://informativos.trilhante.com.br/julgados/stj-resp-1813684-sp 🟡 / Jusbrasil (artigo): https://www.jusbrasil.com.br/artigos/o-recurso-especial-1813684... 🟡
- **Entendimento ATUAL (Lei 14.939/2024 + AREsp 2.638.376, Corte Especial, 11/02/2025):** tribunal deve intimar para correção; aplica-se inclusive a recursos anteriores à lei. ✅ (ver topo)
- 🟡 **Enunciado 66 — I Jornada (CJF)** já antecipava: "Admite-se a correção da falta de comprovação do feriado local ou da suspensão do expediente forense, posteriormente à interposição do recurso, com fundamento no art. 932, parágrafo único, do CPC." (a Lei 14.939/2024 positivou esse entendimento.)

### 3.2 Prazo em dobro — litisconsortes com procuradores diferentes (CPC 229)
- **CPC art. 229:** litisconsortes com **diferentes procuradores, de escritórios de advocacia distintos**, têm prazo em dobro para todas as manifestações, em autos físicos.
- **§2º:** o benefício **cessa** se há só dois réus e um deles é revel/sem advogado.
- **§3º (crítico):** **NÃO se aplica ao processo eletrônico.** Como hoje quase tudo é eletrônico, a regra do dobro é cada vez mais residual.
- STJ aplicou o dobro inclusive ao prazo de pagamento voluntário no cumprimento de sentença (autos físicos).
- Fontes: STJ (notícia): https://www.stj.jus.br/sites/portalp/Paginas/Comunicacao/Noticias-antigas/2017/2017-11-29_08-03_Litisconsortes-com-diferentes-advogados-tem-prazo-em-dobro-para-pagamento-voluntario.aspx 🟡 / TJDFT: https://www.tjdft.jus.br/consultas/jurisprudencia/jurisprudencia-em-temas/novo-codigo-de-processo-civil/listisconsortes-com-diferentes-procuradores-de-escritorio-de-advocacia-distintos-2013-prazo-em-dobro 🟡

### 3.3 Prazos em dias úteis
- 🟡 **Enunciado 89 — I Jornada (CJF):** conta-se em dias úteis o prazo do caput do art. 523 (cumprimento de sentença — 15 dias para pagamento).
- 🟡 **Enunciado 90 — I Jornada (CJF):** conta-se em **dobro** o prazo do art. 525 (impugnação) quando o devedor é assistido pela Defensoria Pública.
- 🟡 **Enunciado 19/20 — I Jornada (CJF):** prazo em dias úteis (art. 219) aplica-se aos Juizados Especiais e à oposição de embargos à execução fiscal (art. 16 LEF).

---

## TEMA 4 — Responsabilidade civil

### 4.1 Dano estético cumulável com dano moral — Súmula 387/STJ ✅ (item de destaque do PRD)
- **Súmula 387 STJ:** "É lícita a cumulação das indenizações de dano estético e dano moral."
- (Ampliada na prática: "É lícita a cumulação das indenizações por dano material, moral e estético decorrentes de um mesmo fato, desde que passíveis de identificação autônoma." — formulação reiterada em acórdãos.)
- Fonte primária (PDF STJ, com leading case da amputação traumática): https://www.stj.jus.br/docs_internet/revista/eletronica/stj-revista-sumulas-2013_35_capSumula387.pdf ✅
- Jusbrasil (verbete): https://www.jusbrasil.com.br/busca?q=s%C3%BAmula+387+do+stj 🟡

### 4.2 Dano moral à pessoa jurídica — Súmula 227/STJ ✅
- **Súmula 227 STJ:** "A pessoa jurídica pode sofrer dano moral."
- Pressuposto: ofensa à **honra OBJETIVA** (reputação/imagem/nome no mercado) — não há honra subjetiva de PJ. Ex. típico: protesto indevido de título.
- ⚠️ Nuance: PJ de **direito público** em regra NÃO pleiteia dano moral contra particular (Buscador Dizer o Direito). Conferir antes de aplicar a ente público.
- Fonte primária (PDF STJ): https://www.stj.jus.br/docs_internet/revista/eletronica/stj-revista-sumulas-2011_17_capSumula227.pdf ✅
- TJDFT: https://www.tjdft.jus.br/consultas/jurisprudencia/jurisprudencia-em-temas/dano-moral-no-tjdft/legitimidade/indenizacao-por-danos-morais-a-pessoa-juridica 🟡

### 4.3 Dano moral in re ipsa (presumido)
- **Tese STJ:** a inscrição/manutenção indevida do nome em cadastro de inadimplentes configura **dano moral in re ipsa** — decorre do próprio fato, **dispensa prova** do abalo.
- Fonte STJ (Jurisprudência em Teses nº 59 — Cadastro de Inadimplentes): https://www.stj.jus.br/internet_docs/jurisprudencia/jurisprudenciaemteses/Jurisprud%C3%AAncia%20em%20teses%2059%20-%20Cadastro%20de%20Inadimplentes.pdf ✅
- ⚠️ **Súmula 385/STJ** (limite): não cabe dano moral por inscrição indevida quando preexiste inscrição legítima (devedor contumaz) — só direito ao cancelamento. (Confirmar texto na fonte STJ antes de citar.)
- MPPR: https://site.mppr.mp.br/consumidor/Noticia/STJ-entende-pela-existencia-de-danos-morais-re-ipsa-na-manutencao-indevida-do 🟡

### 4.4 Perda de uma chance
- **Tese STJ:** a teoria da perda de uma chance é adotada; exige que a chance perdida seja **séria e real** (dano real, atual e certo), não mera expectativa/álea genérica. Indeniza-se a chance em si, não o resultado final.
- Fonte STJ (matéria institucional, com posição do Min. Salomão): https://www.stj.jus.br/sites/portalp/Paginas/Comunicacao/Noticias/09082020-Oportunidades-perdidas--reparacoes-possiveis-a-teoria-da-perda-de-uma-chance-no-STJ.aspx ✅
- 🟡 **Enunciado 444 — V Jornada de Direito Civil (CJF)** (✅ scrapeado verbatim): "A responsabilidade civil pela perda de chance não se limita à categoria de danos extrapatrimoniais, pois, conforme as circunstâncias do caso concreto, a chance perdida pode apresentar também a natureza jurídica de dano patrimonial. A chance deve ser séria e real, não ficando adstrita a percentuais apriorísticos." (Ref.: CC art. 927)
  → https://www.cjf.jus.br/enunciados/enunciado/362 ✅

---

## TEMA 5 — Recursos

### 5.1 Embargos de declaração e prequestionamento — Súmula 98/STJ ✅
- **Súmula 98 STJ:** "Embargos de declaração manifestados com notório propósito de prequestionamento não têm caráter protelatório." → afasta a multa do art. 1.026, §2º quando os ED visam prequestionar.
- Fonte primária (PDF STJ): https://ww2.stj.jus.br/docs_internet/revista/eletronica/stj-revista-sumulas-2010_7_capSumula98.pdf ✅
- Complemento — **prequestionamento ficto:** CPC art. 1.025 — consideram-se incluídos no acórdão os elementos suscitados nos ED, ainda que inadmitidos/rejeitados, para fins de prequestionamento. (→ `cpc-13105-15.md`)

### 5.2 Honorários recursais (CPC 85, §11)
- **Tese STJ:** a majoração do art. 85, §11 exige **dois requisitos cumulativos**: (a) **já existir condenação anterior em honorários** na decisão recorrida (não cabe se a sentença não fixou verba sucumbencial); (b) o recurso ter sido **integralmente desprovido ou não conhecido** (fracasso total).
- Fonte STJ (notícia institucional): https://www.stj.jus.br/sites/portalp/Paginas/Comunicacao/Noticias/2023/01122023-Majoracao-de-honorarios-so-e-possivel-se-o-recurso-foi-integralmente-desprovido-ou-nao-conhecido.aspx ✅
- 🟡 **Enunciado 8 — I Jornada (CJF):** não cabe majoração em agravo de instrumento, **salvo** se interposto contra interlocutória que fixou honorários na origem.
- 🟡 **Enunciado 7 — I Jornada (CJF):** a ausência de contrarrazões da parte contrária, por si só, NÃO afasta a aplicação do art. 85, §11.

### 5.3 Agravo de instrumento — Tema 988/STJ (taxatividade mitigada do art. 1.015) ✅
- **Tese fixada (Tema 988, REsp 1.704.520 e REsp 1.696.396, rel. Min. Nancy Andrighi):** "O rol do art. 1.015 do CPC é de **taxatividade mitigada**, por isso admite a interposição de agravo de instrumento quando verificada a **urgência decorrente da inutilidade do julgamento da questão no recurso de apelação**."
- Aplicação prática (TJDFT exige **demonstração concreta de urgência** — não basta invocar a teoria genericamente).
- Fonte (tese verbatim + acórdãos 2025): https://www.tjdft.jus.br/consultas/jurisprudencia/jurisprudencia-em-temas/precedentes-qualificados-na-visao-do-tjdft/direito-processual-civil/agravo-de-instrumento/tema-988-do-stj-interposicao-de-agravo-de-instrumento-rol-taxativo-possibilidade-de-mitigacao ✅
- Link STJ repetitivos: https://processo.stj.jus.br/repetitivos/temas_repetitivos/pesquisa.jsp?...cod_tema_inicial=988

---

## TEMA 6 — Repetitivos / IRDR de processo civil relevantes

- **Tema 988/STJ** — taxatividade mitigada do agravo de instrumento (ver 5.3). ✅
- **Tema 1209/STJ** — IDPJ × execução fiscal. Tese: o **redirecionamento da execução fiscal ao sócio-gerente PRESCINDE do IDPJ** (art. 133 CPC) nas hipóteses do art. 135 do CTN; o incidente é incompatível com o rito da LEF nesses casos. (Conferir trânsito/tese final antes de citar como definitiva.)
  → STJ (notícia de afetação): https://www.stj.jus.br/sites/portalp/Paginas/Comunicacao/Noticias/2023/11092023-Repetitivo-discute-se-incidente-de-desconsideracao-da-personalidade-juridica-e-compativel-com-execucao-fiscal.aspx 🟡 / Migalhas: https://www.migalhas.com.br/depeso/395535/tema-1209-do-stj-e-a-responsabilizacao-de-socios-por-divida-tributaria 🟡
  ⚠️ **Atenção de escopo:** execução fiscal é fronteira (tributário/execução) — pode estar fora do v0.1 cível, mas o IDPJ no procedimento comum permanece dentro.
- **IDPJ (art. 133-137 CPC) no procedimento comum** — não pode ser instaurado **de ofício** (só a pedido da parte ou do MP); exige contraditório prévio (citação do sócio). Suspende o processo (art. 134, §3º).
  → TJDFT: https://www.tjdft.jus.br/consultas/jurisprudencia/jurisprudencia-em-temas/novo-codigo-de-processo-civil/incidente-de-desconsideracao-da-personalidade-juridica-procedimento 🟡
  → 🟡 **Enunciado 11 — I Jornada (CJF):** aplicam-se os arts. 133-137 à desconsideração **indireta e expansiva**.
  → 🟡 **Enunciado 42 — I Jornada (CJF):** é cabível tutela provisória de urgência **dentro** do IDPJ.
- ❌ **NÃO ENCONTRADO** (nesta rodada) número de IRDR específico de procedimento comum cível nacional que seja transversal o bastante para o v0.1. Recomenda-se rodada dedicada por TJ (IRDRs são, em regra, estaduais) quando o plugin definir os tribunais-alvo.

---

## ENUNCIADOS — CJF / FPPC / ENFAM (relevantes para tutela, prazos, responsabilidade civil)

### CJF — I Jornada de Direito Processual Civil (2017) ✅ (PDF oficial scrapeado integralmente)
Fonte: https://www.cjf.jus.br/cjf/corregedoria-da-justica-federal/centro-de-estudos-judiciarios-1/publicacoes-1/i-jornada-de-direito-processual-civil/i-jornada-de-direito-processual-civil-enunciados-aprovados/@@download/arquivo

| Enunciado | Texto (síntese) | Tema |
|-----------|-----------------|------|
| **5** | Decisão parcial de mérito / art. 485 → condenação proporcional em honorários (art. 85). | honorários |
| **6** | Honorários por apreciação equitativa só nas hipóteses do §8º do art. 85. | honorários |
| **7** | Ausência de contrarrazões não afasta o art. 85, §11. | honorários recursais |
| **8** | Não cabe majoração de honorários em AI, salvo se a interlocutória fixou honorários na origem. | honorários recursais |
| **11** | Arts. 133-137 aplicam-se à desconsideração indireta e expansiva. | IDPJ |
| **19** | Prazo em dias úteis (art. 219) aplica-se aos Juizados Especiais. | prazos |
| **20** | Art. 219 aplica-se aos embargos à execução fiscal (art. 16 LEF). | prazos |
| **38** | Medidas para efetivação da tutela provisória independem do trânsito em julgado, inclusive contra o Poder Público. | tutela |
| **39** | Cassada/modificada a tutela na sentença, a parte pode pleitear restabelecimento na instância superior. | tutela |
| **40** | Irreversibilidade não impede tutela de urgência se o direito é provável e a lesão é irreversível. | tutela |
| **41** | Tutela de urgência é apreciável mesmo em processo sobrestado por repetitivo. | tutela |
| **42** | Cabe tutela de urgência dentro do IDPJ. | tutela / IDPJ |
| **43** | Não há estabilização da tutela antecedente deferida em ação rescisória. | estabilização |
| **44** | Tutela cautelar antecedente exige indicação do valor da causa na inicial. | tutela |
| **45** | Fungibilidade entre as tutelas provisórias. | tutela / fungibilidade |
| **46** | Cessação da eficácia da cautelar por não efetivação em 30 dias só se houver omissão do requerente. | tutela |
| **47** | Probabilidade do direito é requisito da tutela de evidência por abuso de defesa/protelação. | evidência |
| **48** | Tutela de evidência (311, II) cabe em repercussão geral e súmula de tribunal superior. | evidência |
| **49** | Tutela de evidência pode ser concedida em mandado de segurança. | evidência |
| **66** | Admite-se correção posterior da falta de comprovação de feriado local (art. 932, p.ú.). | tempestividade |
| **70** | É agravável a decisão que posterga a análise da tutela provisória ou a condiciona a exigência. | agravo/tutela |
| **89** | Conta-se em dias úteis o prazo do art. 523 (cumprimento). | prazos |
| **90** | Conta-se em dobro o prazo do art. 525 quando o devedor é assistido pela Defensoria. | prazos |
| **93** | Da decisão que julga impugnação ao cumprimento: apelação se extingue; AI se não. | recursos |

### FPPC — Fórum Permanente de Processualistas Civis
- 🟡 Existe (Carta de Florianópolis e seguintes) um corpo de enunciados sobre tutela provisória, estabilização e negócios jurídicos processuais. **Os números específicos NÃO foram confirmados verbatim nesta rodada** (o PDF da Carta de Florianópolis foi localizado, mas não scrapeado item a item).
- Fonte localizada: https://institutodc.com.br/wp-content/uploads/2017/06/FPPC-Carta-de-Florianopolis.pdf 🟡
- Consolidação 2024 (JusPodivm/Academia): https://www.academia.edu/116460831/ 🟡
- ⚠️ **NÃO CONFIRMADO:** o número exato do enunciado FPPC que trata da contestação impedindo a estabilização (frequentemente citado, mas não verificado verbatim aqui). NÃO citar número FPPC específico sem conferir o PDF oficial.

### ENFAM — Escola Nacional de Formação e Aperfeiçoamento de Magistrados
- ❌ **NÃO ENCONTRADO nesta rodada** enunciado ENFAM específico sobre tutela/prazos/responsabilidade civil com texto e número confirmados. A ENFAM editou enunciados sobre o CPC/2015 (Seminário "O Poder Judiciário e o novo CPC", 2015), mas não foram localizados/verificados aqui. **Recomenda-se rodada dedicada** se o plugin for citar ENFAM.

---

## CHECKLIST DE PENDÊNCIAS (para próximas rodadas)
1. ❌ Enunciados **ENFAM** sobre CPC/2015 (tutela, precedentes) — não verificados.
2. ⚠️ Enunciados **FPPC** — localizados mas não extraídos verbatim por número.
3. ⚠️ **Tema repetitivo de gratuidade PF** (critério objetivo de renda) — há julgamento na Corte Especial (2023, REsp pendente); confirmar número e trânsito antes de citar.
4. ⚠️ **Súmula 385/STJ** (limite do dano moral por inscrição indevida) — citada de memória, conferir texto na fonte STJ.
5. ⚠️ **Tema 1209/STJ** (IDPJ × exec. fiscal) — confirmar tese final/trânsito; verificar se entra no escopo cível.
6. **II Jornada Dir. Proc. Civil (CJF)** — enunciado sobre estabilização x Fazenda Pública citado por terceiro; confirmar número/texto no PDF oficial da II Jornada.
