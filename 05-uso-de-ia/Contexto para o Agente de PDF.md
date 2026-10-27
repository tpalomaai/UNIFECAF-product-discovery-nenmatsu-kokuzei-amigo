# Contexto do Projeto — para o Agente de PDF

Este arquivo resume tudo o que o agente precisa saber para montar o PDF teórico. O conteúdo do PDF está no arquivo "PDF Teórico - Rascunho.md". Este aqui explica o projeto, os termos e as regras.


## 1. O trabalho

- Disciplina: Metodologias Ágeis e Validação de Produtos (UniFECAF)
- Título do trabalho: Da Hipótese à Evidência: Validando um Produto Digital com IA e Métodos Ágeis
- Aluna: Paloma Ai Tsuchinaga
- Curso: IA e Automação Digital, 2º semestre
- Prazo: 28/10/2026
- Formato desta entrega: PDF (Parte Teórica)
- O que a banca avalia: a qualidade do PROCESSO de descoberta (hipóteses, experimento, evidências, decisão), não se a ideia é boa. Regra central do enunciado: "IA não valida mercado; pessoas reais validam."

Itens obrigatórios da Parte Teórica, segundo o enunciado:
1. Problema identificado, público e oportunidade
2. Hipóteses de problema, solução e valor
3. Solução inicialmente proposta e definição do MVP
4. Como a IA foi utilizada no processo de descoberta
5. Experimento escolhido e critérios de sucesso
6. Critério previamente definido para decidir (perseverar, ajustar, pivotar ou abandonar)


## 2. O projeto em 3 linhas

- Problema: brasileiros que trabalham no Japão adiam ou erram o preenchimento da declaração de dependentes (fuyō kōjo shinkokusho) porque não entendem os campos.
- Solução testada: assistente de IA no NotebookLM, com fontes oficiais da Agência Nacional de Impostos do Japão (Kokuzeichō), que explica o preenchimento em português.
- Experimento: a pessoa testa sozinha com uma família fictícia e responde um Google Forms anônimo em modo teste (cerca de 12 minutos, sem entrevista).


## 3. Linha do tempo

| Data | O que aconteceu |
|---|---|
| 20/10 | Planejamento com Tree-of-Thoughts. Primeira ideia (resumo de comunicados da escola) descartada. Problema definido: declaração de dependentes |
| 20/10 | Pesquisa nas fontes oficiais. Base de conhecimento com 25 cenários, revisada com Self-Refine e avaliação de fidelidade (9 correções) |
| 20/10 | Família fictícia e gabarito do quiz. NotebookLM montado e compartilhado |
| 21/10 | Eval do assistente: rodada 1 = 10/11 + 2/2; rodada 2 = 11/11 + 2/2 |
| 21/10 | Google Forms montado e testado. Critérios congelados. Forms publicado e divulgado |
| 21 a 26/10 | Coleta das respostas |
| 26/10 | Análise e decisão (vai para o README e o vídeo, não para este PDF) |


## 4. Glossário (usar sempre com romaji e significado)

| Termo | Leitura | Significado |
|---|---|---|
| 給与所得者の扶養控除等(異動)申告書 | kyūyo shotokusha no fuyō kōjo-tō (idō) shinkokusho | Declaração de dependentes do assalariado |
| 国税庁 | Kokuzeichō | Agência Nacional de Impostos do Japão |
| 記載例 | kisairei | Exemplo de preenchimento |
| 年末調整 | nenmatsu chōsei | Ajuste de fim de ano |
| 収入 | shūnyū | Salário bruto |
| 所得 | shotoku | Renda líquida |
| 特定親族 | tokutei shinzoku | Categoria nova para familiares de 19 a 22 anos com renda um pouco maior |
| 住民税 | jūminzei | Imposto residencial (prefeitura) |
| 社会保険 | shakai hoken | Seguro social |


## 5. Regras de conteúdo para o PDF

1. Usar o texto do arquivo "PDF Teórico - Rascunho.md" como está. Pode quebrar parágrafos longos, mas não reescrever o sentido, não resumir dados e não acrescentar informações.
2. Nunca inventar números, datas, resultados ou citações. Se algo estiver faltando, deixar um marcador visível: [FALTA: descrição].
3. Todo termo em japonês aparece com a leitura em romaji e o significado em português, como no glossário.
4. Tabelas continuam como tabelas.
5. Cada marcação [Print: ...] do rascunho vira um espaço reservado para imagem, com a legenda do print. Se o arquivo de imagem tiver sido enviado junto, usar a imagem.
6. Este PDF NÃO traz os resultados da coleta. Eles entram depois, no README e no vídeo.
7. Linguagem: português do Brasil, clara, para quem não conhece o assunto.


## 6. Prints disponíveis (nomes dos arquivos)

| Arquivo | Print | Onde entra |
|---|---|---|
| Arquivo na pasta Prints | Print | Onde entra |
|---|---|---|
| 01_fontes-notebooklm.png | Painel de fontes e tela de configuração do chat (um print só) | Seção 3 |
| placar-eval.png | Placar do eval | Seção 4 |
| eval-pergunta-5.png | Pergunta 5, rodada 1 (erro: valor inventado) | Seção 4 |
| eval-pergunta-5-rodada2.png | Pergunta 5, rodada 2 (corrigida) | Seção 4 |
| forms-edicao.png | Forms no modo de edição | Seção 5 |
| post-recrutamento-grupo-da-cidade-facebook-parte-1.jpg | Post no grupo do Facebook | Seção 5 |
| post-recrutamento-stories-instagram.jpg | Stories do Instagram | Seção 5 |
| 2026-10-21_criterios-congelados.png | Critérios congelados com data e hora | Seção 6 |

Os demais prints da pasta (parte 2 do Facebook e mensagens de WhatsApp) são evidência guardada, mas não entram no PDF.


## 7. Links

- NotebookLM: https://notebook.google.com/notebook/fb38933d-f2a2-484e-ad90-f479220349fd
- Google Forms: https://docs.google.com/forms/d/e/1FAIpQLSdWkEzgEcBtztzTXN6StSxFSbEX4bHaYuxx9MwAe4zaqydfBw/viewform?usp=header
- 記載例 2027 (oficial): https://www.nta.go.jp/publication/pamph/gensen/nencho2026/pdf/309.pdf
