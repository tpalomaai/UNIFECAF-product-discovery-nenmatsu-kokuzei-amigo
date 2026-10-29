# Como a IA foi usada em cada etapa

A IA apoiou pesquisa, organização, escrita e testes. Quem validou as hipóteses foram 8 pessoas reais, e a decisão saiu de uma regra registrada antes do teste.

| Etapa | Técnica | Como a IA ajudou | O que eu decidi |
|---|---|---|---|
| Planejamento | Tree-of-Thoughts | Gerou e comparou 10 abordagens | Escolhi o problema |
| Cenários | Self-Consistency | Levantou 25 cenários por 3 caminhos | Defini os tipos de família |
| Revisão da base | Self-Refine | Conferiu as regras na fonte oficial (9 correções) | Aprovei as correções |
| MVP | Instrução com 10 regras | Redigiu a instrução do assistente | Montei o NotebookLM |
| Validação v1 | Evals (13 perguntas) | Achou um valor inventado | Rodei os testes |
| Experimento | Rascunho estruturado | Ajudou no questionário e na família fictícia | Registrei os critérios antes |
| Análise | Chain-of-Verification | Conferiu cada número na resposta de origem | Apliquei a regra: AJUSTAR |
| Versão 2 | Graph-of-Thoughts | Ligou os achados às mudanças | Escolhi o escopo da v2 |
| Validação v2 | Evals + red-teaming | Corrigiu 23 respostas e achou falhas | Rodei as 3 rodadas |
| Entrega | Few-shot + tags XML | Ajudou no PDF, README e slides | Gravei o vídeo e revisei |

**Ferramentas:** Claude (apoio em todas as etapas) · NotebookLM (o assistente) · ChatGPT (ilustrações) · Canva (slides e PDF).

**A IA não** validou o mercado, não respondeu a pesquisa, não escolheu a decisão e não teve acesso a dados pessoais.

## Aprendizados
1. Instrução não garante comportamento: só o teste mostra o que a IA faz de verdade.
2. Toda melhoria precisa de teste de regressão: a v2 explicou melhor, mas passou a calcular o que devia recusar.
3. Registrar a régua antes de ver os dados evita ajustar a interpretação depois.
4. O assistente acertou as regras, mas as pessoas não o consultaram. Isso só apareceu no teste com gente de verdade.
