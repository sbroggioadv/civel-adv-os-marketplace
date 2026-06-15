---
description: Inicia o wizard de configuracao do plugin civel — cria a pasta civel/ com identidade, areas de atuacao, tribunais-alvo, polo e modo de fluxo.
allowed-tools: Read, Write, Edit, Bash, Glob, Grep
argument-hint: [--update para reconfigurar]
---

Voce foi acionado pelo comando `/start-civel` do plugin civel-adv-os (Civil Litigation Master).

Argumento recebido: `$ARGUMENTS`

**Objetivo:** configurar o plugin de contencioso civel ao perfil do escritorio.

## PROTOCOLO
1. **Acionar a skill `civel-onboarding`** (wizard com botoes via AskUserQuestion nas escolhas de lista fechada).
2. Cria `<cwd>/civel/perfil.md` (identidade, areas, tribunais-alvo, polo, modo).
3. Se ja existir, oferecer continuar / atualizar / recriar.

**Skill a acionar:** `civel-onboarding`.
