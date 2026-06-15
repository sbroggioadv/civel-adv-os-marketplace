---
name: triagem-civel
description: "Classifica a demanda civel e roteia para a skill certa. Identifica a FASE PROCESSUAL (consulta, ajuizamento, conhecimento, recursal, execucao, incidente) e o OBJETIVO juridico, e indica a skill alvo + o foro competente. Use quando o operador descrever uma situacao civel e nao souber o caminho, ou disser triagem civel, qual o caminho, que peca eu uso, em que fase estou, /triagem-civel."
---

# TRIAGEM-CIVEL

> Tier 0. Porta de classificacao. Chamada pelo `civel-master` no inicio de todo caso.

## Anexos obrigatorios (context/)
- `context/metodologia-civel.md` (mapa de skills + fluxo).
- `context/recursos-tutelas-civel.md` (se a fase for recursal/tutela).

## Objetivo
Em poucas perguntas, dizer: fase processual + objetivo + skill alvo + (se aplicavel) foro/tribunal.

## Arvore de decisao
1. **Vai AJUIZAR (autor)?** -> gestao processual (competencia/foro, valor da causa, gratuidade) + `peticao-inicial-civel` (+ `tutela-urgencia`/`tutela-evidencia` se houver urgencia/evidencia). Acao especifica = v0.2 (`acao-indenizatoria`, `possessorias`, etc.).
2. **Foi CITADO (reu)?** -> `contestacao-civel` (+ `preliminares-civel`, `reconvencao` se cabivel; `revelia` se perdeu prazo).
3. **Esta no fluxo de CONHECIMENTO?** -> conforme o ato: `replica-civel`, `saneamento`, `producao-de-provas`, `audiencia-conciliacao-mediacao`, `audiencia-instrucao`, `razoes-finais-memoriais`, `resumo-de-ata`.
4. **Recebeu DECISAO/SENTENCA e quer recorrer?** -> escolher o recurso: interlocutoria do rol 1.015 -> `agravo-de-instrumento`; sentenca -> `apelacao-civel`; vicio (omissao/contradicao) -> `embargos-de-declaracao`; decisao monocratica -> `agravo-interno`; ultima instancia vs lei federal/CF -> `recursos-excepcionais`. Sempre `admissibilidade-e-tempestividade-recursal`.
5. **Cumprimento/execucao?** -> v0.2 (`cumprimento-de-sentenca`, `impugnacao-ao-cumprimento`) — defesa/estrategia; maquina pesada cross-link `execucao-adv-os`.
6. **Incidente?** (suspeicao, conflito de competencia, IDPJ, IRDR/IAC) -> v0.2.

## Entrega obrigatoria final
- Fase + objetivo + skill alvo + foro/tribunal, em 3-5 linhas, e o handoff para o `civel-master`.

## Guard
Na duvida de competencia/foro, consultar `context/cpc-13105-15.md` (arts. 42-66) + `context/cpc-cc-alteracoes-recentes.md` (Lei 14.879/2024). Nao redigir peca aqui — so classificar e rotear.
