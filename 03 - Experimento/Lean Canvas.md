# Lean Canvas — Ajudante da Declaração de Dependentes

Versão montada antes do teste. O canvas com o resultado de cada hipótese está em [Prints/lean-canvas-resultados.png](../Prints/lean-canvas-resultados.png).

Legenda: ✅ veio da pesquisa · 🧪 em teste agora · ❓ hipótese não testada

## 1. Problema
1. Brasileiros não entendem os campos do fuyō kōjo shinkokusho (declaração de dependentes), todo em japonês 🧪
2. Confundem salário bruto (shūnyū) com renda líquida (shotoku) e erram os limites 🧪
3. Regras mudaram recentemente (limites novos, categoria tokutei shinzoku), o que confunde até quem já preenchia ✅

Alternativas que existem hoje:
- Perguntar ao RH, ao intérprete da empresa ou a colegas
- Tradutor do celular (Google Lens)
- Versão oficial em português da Kokuzeichō, que é de 2026, tem tradução confusa e não traz exemplo preenchido ✅
- Adiar a entrega ou deixar outra pessoa preencher

## 2. Segmento de clientes
Brasileiros assalariados no Japão que recebem o formulário da empresa todo ano.

Early adopters:
- Famílias com cônjuge ou filhos jovens que fazem arubaito
- Quem sustenta familiares no Brasil

## 3. Proposta de valor única
Saber exatamente onde cada pessoa da família entra no formulário e o que marcar, em português simples e com base nos documentos oficiais.

Conceito de alto nível: "um intérprete do RH no bolso, para o papel do fim do ano"

## 4. Solução
1. Assistente de IA que só responde com base nas fontes oficiais da Kokuzeichō (NotebookLM) ✅
2. Explica cada termo japonês com romaji e significado ✅
3. Converte salário bruto em renda líquida usando a tabela oficial ✅

## 5. Canais
- Grupos de brasileiros no Japão (Facebook, LINE) ✅ usado no recrutamento
- Stories e indicação entre conhecidos ✅ usado no recrutamento
- Empreiteiras e agências que empregam brasileiros ❓

## 6. Fluxos de receita ❓ (não testado neste experimento)
- Gratuito para o trabalhador
- Possível: licença para empreiteiras e agências, que hoje gastam tempo do RH e de intérpretes explicando o papel

## 7. Estrutura de custos
- Ferramenta: NotebookLM gratuito no protótipo ✅
- Tempo para montar e revisar a base de conhecimento ✅
- Atualização anual das fontes, porque o formulário muda todo ano ❓

## 8. Métricas-chave
- Acerto nas armadilhas do formulário (quiz) 🧪
- Confiança do usuário no que preencheu 🧪
- Intenção de uso no próximo outubro 🧪
- Erros do assistente no eval (11/11 + 2/2) ✅

## 9. Vantagem injusta
- Base de conhecimento revisada contra o documento oficial, com cenários reais de famílias brasileiras ✅
- Conhecimento de quem vive a realidade de família brasileira no Japão ✅
- Ainda não é uma vantagem difícil de copiar ❓
