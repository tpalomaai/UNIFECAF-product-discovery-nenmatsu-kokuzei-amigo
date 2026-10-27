# Verificação do Rascunho do PDF Teórico

Chain-of-Verification: cada número, data e afirmação factual do rascunho foi conferido contra a fonte de onde veio.
Este arquivo NÃO vai para o agente de PDF. Serve só para mim, como registro.

Legenda:
- ✅ Confere com a fonte
- 🔧 Estava impreciso e foi corrigido no rascunho
- ⏳ Falta completar


## Seção 1 — Problema, público e oportunidade

| Dado ou afirmação | Fonte | Status |
|---|---|---|
| O formulário chega entre outubro e dezembro | Pesquisa no site da Kokuzeichō e prática das empresas | ✅ |
| A versão em português é de 2026 | Página de versões estrangeiras da Kokuzeichō (令和8年分) | ✅ |
| A versão em português tem trechos confusos e não traz exemplo preenchido | Leitura do arquivo r08_01_po.pdf | ✅ |
| O exemplo de preenchimento existe só em japonês | Busca feita em 20/10 | ✅ |
| Consequências de erro no formulário | Cenários e Armadilhas, seção 6 (selos 🔹 e ⚠️) | 🔧 Antes estavam escritas como certezas; agora usam "pode" |
| Limites subiram a partir de 2026 e existe a categoria 特定親族 | Aviso no topo do 記載例 2027 e seção ❺ | 🔧 Antes dizia que a categoria "foi criada em 2026", e o 記載例 não confirma o ano de criação |
| Comunicados importantes da escola chegam no início do mês | Observação minha (20/10) | ✅ |


## Seção 3 — MVP

| Dado ou afirmação | Fonte | Status |
|---|---|---|
| 2 fontes no NotebookLM | Print do painel de fontes | ✅ |
| 25 cenários | Cenários e Armadilhas: 1 a 23, 9b e 24 | ✅ |
| 10 regras na instrução | Instrução salva no Configurar chat | ✅ |
| Limite de 1.500 caracteres | Contagem do texto cortado em 20/10 | ✅ |
| Acesso por link público com conta Google | Configuração de compartilhamento e Ajuda do NotebookLM | ✅ |


## Seção 4 — Uso da IA

| Dado ou afirmação | Fonte | Status |
|---|---|---|
| Tree-of-Thoughts com 10 abordagens e agentes defendendo cada finalista | Conversa de 20/10 (segunda árvore) | ✅ |
| Self-Consistency com três caminhos independentes | Conversa de 20/10 | 🔧 Antes dizia "manter só o que os três concordavam"; na verdade, as divergências foram mantidas e marcadas como incertas |
| 9 correções na avaliação de fidelidade, cobertura e clareza | Lista F1–F4, C1–C3, L1–L2 | ✅ |
| Eval com 13 perguntas | Arquivo Eval: 11 de regra + 2 fora do escopo | 🔧 Antes dizia "com resposta esperada e fonte"; as 2 fora do escopo não têm fonte |
| Rodada 1: 10 de 11 e 2 de 2 | Placar do eval | ✅ |
| Rodada 2: 11 de 11 e 2 de 2 | Placar do eval | 🔧 Agora explica que só a pergunta 5 foi refeita |
| O que mudou na rodada 2 | Instrução nova (regras 6 e 10) | 🔧 Faltava a regra do aviso de protótipo |
| Precisou apagar o histórico para testar de novo | Conversa de 21/10 | ✅ |


## Seção 5 — Experimento

| Dado ou afirmação | Fonte | Status |
|---|---|---|
| Cerca de 12 minutos | Teste do Forms feito por mim | ✅ (confirmar o tempo que eu medi) |
| Família: filho de 6 anos, esposa com arubaito, filho de 17 e filha de 20 | Família Fictícia e Gabarito | ✅ |
| Ficha informa só o salário bruto | Questionário, Seção 2 | ✅ |
| Recrutamento entre 21 e 26/10 em grupos, stories e conhecidos | Prints dos posts | ✅ |
| Tabela de critérios | Nota "Critérios congelados" | ✅ Idêntica |


## Seção 6 — Decisão

| Dado ou afirmação | Fonte | Status |
|---|---|---|
| Regra de decisão | Nota "Critérios congelados" | ✅ Idêntica |
| Pivotar se a pergunta aberta apontar outra dor em 2 ou mais pessoas | Nota "Critérios congelados" | ✅ |
| Inconclusivo se houver menos de 5 respostas até 26/10, 12h | Nota "Critérios congelados" | ✅ |
| Registrado em 21/10/2026, [HORA] | Print dos critérios congelados | ⏳ Completar a hora |


## Resumo
- 5 correções feitas no rascunho (🔧)
- 1 item para completar: a hora do congelamento (⏳)
- Nenhum número sem fonte
