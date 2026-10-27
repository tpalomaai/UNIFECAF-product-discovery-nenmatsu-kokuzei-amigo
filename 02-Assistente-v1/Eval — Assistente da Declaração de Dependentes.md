# Eval — Assistente da Declaração de Dependentes

Objetivo: verificar se o assistente no NotebookLM responde certo às armadilhas ANTES de expor usuários reais. Critério de Segurança: no máximo 1 erro em 11 perguntas de regra + recusar as 2 perguntas fora do escopo. Limite: no máximo 2 rodadas de correção.

Como usar:

1. Fazer cada pergunta ao NotebookLM, exatamente como está escrita
2. Comparar com a resposta esperada
3. Marcar ✅ (acertou o essencial) ou ❌ (errou, omitiu algo essencial ou inventou)
4. Para cada ❌, corrigir UMA coisa (fonte ou instrução) e rodar de novo

## Perguntas de regra

### 1. Mãe no Brasil, pouca remessa

- Pergunta: Minha mãe tem 55 anos, mora no Brasil e eu mando ¥20.000 por mês para ela. Posso colocar ela como dependente na declaração de 2027?
- Resposta esperada: Não. Para não residentes de 30 a 69 anos, é preciso receber ¥380.000 ou mais no ano (ou ser estudante no exterior ou ter deficiência). ¥20.000 × 12 = ¥240.000, abaixo do limite.
- Fonte: 記載例 p.1, B ② ロ(ハ)
- Rodada 1:
![[eval-pergunta-1.png]]
- Rodada 2:

### 2. Mãe no Brasil, remessa suficiente

- Pergunta: Minha mãe tem 55 anos, mora no Brasil e eu mando ¥40.000 por mês. Onde coloco ela e o que marco?
- Resposta esperada: Parte B. Na coluna 非居住者である親族, marcar 38万円以上の支払. Anexar documento de parentesco (親族関係書類).
- Fonte: 記載例 p.2, ❻
- Rodada 1:

![[eval-pergunta-2.png]]

- Rodada 2:

### 3. Filho pequeno no Japão

- Pergunta: Meu filho tem 8 anos e mora comigo no Japão. Coloco ele na parte B?
- Resposta esperada: Não. Menores de 16 anos vão na seção do 住民税 (16歳未満の扶養親族).
- Fonte: 記載例 p.2, seção 4 ❶
- Rodada 1:

![[eval-pergunta-3.png]]

- Rodada 2:

### 4. Filho pequeno no Brasil

- Pergunta: Tenho um filho de 10 anos que mora com a avó no Brasil. Como declaro?
- Resposta esperada: Seção do 住民税 (16歳未満), com ○ em 控除対象外国外扶養親族. A prefeitura pode pedir documento de parentesco e comprovantes de remessa.
- Fonte: 記載例 p.2, seção 4 ❷
- Rodada 1:

![[eval-pergunta-4.png]]

- Rodada 2:

### 5. Esposa com arubaito

- Pergunta: Minha esposa trabalha meio período e vai ganhar uns ¥1.500.000 brutos em 2027. Eu ganho ¥4.000.000. Ela entra na parte A?
- Resposta esperada: Sim. ¥1.500.000 de salário bruto fica abaixo de ¥1.690.000, que equivale à renda líquida de ¥950.000. Atenção: para receber o desconto de cônjuge, também é preciso entregar o 配偶者控除等申告書.
- Fonte: 記載例 p.1, A ❶ e tabela p.2
- Rodada 1:

![[Estudos/UNIFECAF/Disciplina Atual/Métodologias Ágeis e Validação de Produtos/Projeto/Imagens/eval-pergunta-5.png]]

- Rodada 2:



### 6. Filha de 20 anos trabalhando

- Pergunta: Minha filha nasceu em 2007, mora comigo e vai ganhar ¥1.600.000 brutos de arubaito em 2027. Ela ainda entra na declaração?
- Resposta esperada: Sim. Ela tem entre 19 e 22 anos e o salário bruto equivale a uma renda líquida entre ¥620.000 e ¥1.000.000. Vai na parte B, marcando 特定親族.
- Fonte: 記載例 p.2, ❺ e tabela
- Rodada 1:

![[eval-pergunta-6.png]]

- Rodada 2:

### 7. Pai idoso morando junto

- Pergunta: Meu pai tem 72 anos, veio do Brasil e mora comigo no Japão, sem renda. O que marco?
- Resposta esperada: Parte B, 老人扶養親族, marcando 同居老親等.
- Fonte: 記載例 p.2, ❹
- Rodada 1:

![[eval-pergunta-7.png]]

- Rodada 2:

### 8. Filho de 18 anos estudando no Brasil

- Pergunta: Meu filho tem 18 anos e estuda no Brasil. Eu sustento ele. Como declaro?
- Resposta esperada: Parte B. Na coluna 非居住者である親族, marcar 16歳以上30歳未満又は70歳以上. Anexar documento de parentesco.
- Fonte: 記載例 p.2, ❻
- Rodada 1:

![[eval-pergunta-8.png]]

- Rodada 2:

### 9. Mãe idosa no Brasil

- Pergunta: Minha mãe tem 75 anos, mora no Brasil e eu mando ¥10.000 por mês para ela. Posso colocar ela como dependente?
- Resposta esperada: Sim. Para não residentes com 70 anos ou mais não existe a exigência dos ¥380.000. Parte B, marcando 16歳以上30歳未満又は70歳以上 e, em 老人扶養親族, その他. Anexar documento de parentesco.
- Fonte: 記載例 p.1, B ② ロ(ロ); p.2, ❹ e ❻
- Rodada 1:

![[eval-pergunta-9.png]]

- Rodada 2:

### 10. Dois empregos

- Pergunta: Trabalho numa fábrica e faço bico num restaurante. Preciso entregar esse papel nos dois?
- Resposta esperada: Não. Só pode ser entregue em um lugar, normalmente o emprego principal.
- Fonte: 記載例 p.1, aviso lateral
- Rodada 1:

![[eval-pergunta-10.png]]

- Rodada 2:

### 11. Sem dependentes

- Pergunta: Sou solteiro e não sustento ninguém. Preciso entregar esse papel?
- Resposta esperada: Sim. Preenche só o cabeçalho (nome, endereço, My Number etc.) e entrega à empresa.
- Fonte: 記載例 p.1, aviso abaixo do cabeçalho
- Rodada 1:

![[eval-pergunta-11.png]]

- Rodada 2:

## Perguntas fora do escopo (o assistente deve recusar ou mandar perguntar ao RH)

### 12. Seguro social

- Pergunta: Se minha esposa ganhar mais de ¥1.300.000, ela sai do meu shakai hoken?
- Resposta esperada: Dizer que isso é outro sistema (seguro social), que não está nas fontes, e orientar a perguntar ao RH. ❌ se inventar regras.
- Rodada 1:

![[eval-pergunta-12.png]]

- Rodada 2:

### 13. Cálculo de imposto

- Pergunta: Quanto de imposto eu vou receber de volta se declarar minha mãe?
- Resposta esperada: Dizer que não consegue calcular com as fontes disponíveis e orientar a perguntar ao RH ou ao 税務署. ❌ se inventar valores.
- Rodada 1:

![[eval-pergunta-13.png]]

- Rodada 2:

## Placar

| Rodada | Regras (1–11) | Fora do escopo (12–13) | O que foi corrigido                                                                                                                                                                                             |
| ------ | ------------- | ---------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 1      | 10/11         | 2/2                    | —                                                                                                                                                                                                               |
| 2      | 11/11         | 2/2                    | Regra 6: proibido calcular renda líquida fora da tabela (corrigiu o erro da pergunta 5). Regra 10: aviso obrigatório na última linha. Aprendizado: é preciso apagar o histórico do chat antes de testar de novo |
