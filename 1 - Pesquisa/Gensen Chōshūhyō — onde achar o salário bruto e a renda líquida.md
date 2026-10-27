# Gensen Chōshūhyō — Onde achar o Salário Bruto e a Renda Líquida

Fonte para a versão 2 do assistente. NÃO adicionar ao notebook atual antes do fim da coleta (26/10, 12h).

Fonte oficial: modelo do 給与所得の源泉徴収票 de 2026 (令和8年分), versão do trabalhador (受給者交付用), Kokuzeichō. https://www.nta.go.jp/taxes/tetsuzuki/shinsei/annai/hotei/pdf/r08/0026009-129.pdf

Legenda:

- ✅ Confirmado no modelo oficial
- ⚠️ Verificar antes de usar

## 1. O que é este papel

| | |
|---|---|
|Nome|給与所得の源泉徴収票 (kyūyo shotoku no gensen chōshūhyō)|
|Em português|Comprovante de rendimentos e de imposto retido do assalariado|
|Quem preenche|A empresa, não o trabalhador|
|Quando chega|Depois do ajuste de fim de ano (nenmatsu chōsei), normalmente em dezembro ou janeiro, ou quando a pessoa sai do emprego|
|Para que serve|Mostra quanto a pessoa ganhou no ano, quais descontos foram aplicados e quanto imposto foi retido|
|Onde é pedido|Renovação de visto, declaração anual (kakutei shinkoku), novo emprego no mesmo ano|

## 2. Onde achar o salário bruto e a renda líquida

Os valores principais ficam na primeira linha de valores do papel, da esquerda para a direita:

|Campo no papel|Leitura|O que é|Fonte|
|---|---|---|---|
|支払金額|shiharai kingaku|**Salário bruto do ano** (shūnyū): tudo o que a empresa pagou, antes de qualquer desconto|✅|
|給与所得控除後の金額（調整控除後）|kyūyo shotoku kōjo-go no kingaku (chōsei kōjo-go)|**Renda líquida do salário** (shotoku): o bruto menos o desconto automático de despesas. É o valor que a declaração de dependentes chama de 所得|✅|
|所得控除の額の合計額|shotoku kōjo no gaku no gōkeigaku|Soma de todos os descontos aplicados (dependentes, cônjuge, seguros etc.)|✅|
|源泉徴収税額|gensen chōshū zeigaku|Imposto de renda retido no ano, já depois do ajuste|✅|

Atenção: a posição exata das colunas pode variar um pouco entre empresas que usam sistemas próprios. Sempre procurar pelo nome do campo. ⚠️

## 3. Como isso ajuda a preencher a declaração de dependentes

A declaração de dependentes pede a renda líquida ESTIMADA de cada familiar para o ano a que o formulário se refere (所得の見積額, shotoku no mitsumorigaku). O gensen chōshūhyō traz os valores de um ano que JÁ TERMINOU.

Regra para usar o papel:

1. Use o 支払金額 (salário bruto) do gensen chōshūhyō como referência de quanto a pessoa costuma ganhar.
2. Ajuste se o salário vai mudar (mais horas, novo emprego, saída do emprego).
3. Converta esse bruto estimado em renda líquida usando a tabela de conversão do ANO do formulário (arquivo "Cenários e Armadilhas").

NÃO copie direto o 給与所得控除後の金額 de um gensen chōshūhyō antigo. As regras de cálculo mudaram nos últimos anos, então o mesmo salário bruto pode dar uma renda líquida diferente em outro ano. ⚠️

Outros cuidados:

- O gensen chōshūhyō que a pessoa tem em mãos no fim do ano normalmente é o do ano ANTERIOR. O do ano atual só chega depois do ajuste de fim de ano.
- Cada pessoa que trabalha recebe o próprio gensen chōshūhyō. Para saber quanto a esposa ou um filho que faz arubaito ganha, é preciso olhar o papel DELES, não o seu.
- Na declaração de dependentes, o trabalhador NÃO escreve a própria renda. Só escreve a renda estimada de cada familiar. A renda do próprio trabalhador vai em outro formulário (o 基礎控除申告書, kiso kōjo shinkokusho).

Exemplo: o gensen chōshūhyō do arubaito da esposa mostra 支払金額 de ¥1.500.000. Se ela vai trabalhar o mesmo tanto, a estimativa de salário bruto dela é ¥1.500.000. Pela tabela de 2027, isso fica abaixo de ¥1.690.000, ou seja, abaixo do limite da parte A.

## 4. Como conferir se os dependentes foram aplicados

Depois do ajuste de fim de ano, o gensen chōshūhyō mostra quais dependentes a empresa considerou. Campos para conferir:

|Campo no papel|Leitura|O que mostra|Fonte|
|---|---|---|---|
|控除対象配偶者|kōjo taishō haigūsha|Se o desconto do cônjuge foi aplicado|✅|
|配偶者の合計所得|haigūsha no gōkei shotoku|A renda total do cônjuge considerada|✅|
|控除対象扶養親族等の数|kōjo taishō fuyō shinzoku-tō no kazu|Quantos dependentes de 16 anos ou mais foram considerados|✅|
|16歳未満扶養親族の数|jūroku-sai miman fuyō shinzoku no kazu|Quantos dependentes menores de 16 anos foram informados|✅|
|特定親族特別控除の額|tokutei shinzoku tokubetsu kōjo no gaku|O valor do desconto especial do tokutei shinzoku (19 a 22 anos)|✅|
|非居住者である親族の数|hikyojūsha de aru shinzoku no kazu|Quantos dependentes que moram fora do Japão foram considerados|✅|
|障害者の数|shōgaisha no kazu|Quantos dependentes com deficiência foram considerados|✅|

Se um dependente declarado não aparece aqui, a pessoa deve perguntar ao RH. ⚠️ (orientação geral, não está no modelo)

## 5. Fora do escopo

- Calcular se o imposto retido está certo.
- Explicar os campos de seguros e financiamento imobiliário (住宅借入金, jūtaku kariirekin) deste papel.
- Usar o gensen chōshūhyō para a renovação de visto (perguntar ao escritório de imigração ou ao gyōseishoshi).

## 6. Perguntas de eval para a versão 2

### V2-1. Achar o bruto

- Pergunta: Recebi o gensen chōshūhyō. Onde vejo quanto eu ganhei no ano, antes dos descontos?
- Resposta esperada: No campo 支払金額 (shiharai kingaku), que é o salário bruto do ano.

### V2-2. Achar o líquido

- Pergunta: A declaração de dependentes pede a renda líquida da minha esposa. Onde acho isso?
- Resposta esperada: Olhar o gensen chōshūhyō DELA, no campo 支払金額 (salário bruto), como referência do quanto ela ganha. Ajustar se o salário dela vai mudar e converter para renda líquida pela tabela de 2027. Não copiar direto o 給与所得控除後の金額 de um ano anterior, porque as regras de cálculo mudaram.

### V2-3. Conferir dependentes

- Pergunta: Como sei se a empresa considerou meus filhos no desconto?
- Resposta esperada: No gensen chōshūhyō, nos campos 控除対象扶養親族等の数 (16 anos ou mais) e 16歳未満扶養親族の数 (menores de 16).

### V2-4. Fora do escopo

- Pergunta: O imposto que descontaram no meu gensen chōshūhyō está certo?
- Resposta esperada: Recusar o cálculo e orientar a perguntar ao RH ou ao zeimusho.