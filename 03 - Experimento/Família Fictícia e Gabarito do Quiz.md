# Família Fictícia e Gabarito do Quiz

Armadilhas testadas: cenários 1, 2, 4 e 5 do arquivo "Cenários e Armadilhas". Todas as regras usadas estão marcadas com ✅ (confirmadas no exemplo oficial de 2027).

## Parte 1 — Ficha da família (o que o testador vê)

Copiar este trecho para a descrição do Google Forms.

> Você é o Carlos, brasileiro, 40 anos, mora no Japão e trabalha numa fábrica. A empresa entregou a declaração de dependentes de 2027 (fuyō kōjo shinkokusho). Use o assistente para descobrir como preencher.
> 
> Sua família mora toda com você no Japão. Os valores abaixo são a estimativa de salário bruto (antes dos descontos) de cada um para o ano de 2027.
> 
> - Carlos (você): 40 anos. Salário bruto de ¥4.200.000
> - Ana (esposa): 38 anos. Trabalha meio período (arubaito). Salário bruto de ¥1.690.000
> - Júlia (filha): nascida em março de 2007, tem 20 anos. Faz arubaito. Salário bruto de ¥1.600.000
> - Pedro (filho): nascido em maio de 2010, tem 17 anos. Faz arubaito. Salário bruto de ¥1.500.000
> - Lucas (filho): nascido em 2021, tem 6 anos. Não trabalha
> 
> Ninguém da família tem deficiência, outra renda além do salário ou outro emprego.

## Parte 2 — Perguntas do quiz (modo teste do Google Forms)

### Pergunta 1 — Lucas (cenário 1)

Onde o Lucas, de 6 anos, deve aparecer no formulário?

- a) Na parte B, junto com os outros filhos
- b) Na seção do imposto residencial (jūminzei), na linha de dependentes menores de 16 anos ✅
- c) Ele não precisa aparecer no formulário
- d) Na parte A

### Pergunta 2 — Ana (cenário 2)

No campo de renda estimada para 2027 (所得の見積額, shotoku no mitsumorigaku) da Ana, qual valor o Carlos deve escrever?

- a) ¥1.690.000
- b) ¥950.000 ✅
- c) ¥0
- d) A Ana não entra no formulário, porque trabalha

### Pergunta 3 — Pedro (cenário 4)

O Pedro, de 17 anos, ganha ¥1.500.000 brutos. Como ele entra no formulário?

- a) Na parte B, como dependente comum
- b) Na parte B, marcando 特定扶養親族 (tokutei fuyō shinzoku)
- c) Ele não entra como dependente, porque passou do limite de renda ✅
- d) Na seção do imposto residencial, com os menores de 16 anos

### Pergunta 4 — Júlia (cenário 5)

A Júlia, de 20 anos, ganha ¥1.600.000 brutos, MAIS do que o Pedro. Como ela entra no formulário?

- a) Ela não entra, porque passou do limite de renda
- b) Na parte B, marcando 特定扶養親族 (tokutei fuyō shinzoku)
- c) Na parte B, marcando 特定親族 (tokutei shinzoku) ✅
- d) Na parte A

## Parte 3 — Gabarito explicado (só para você, não mostrar ao testador)

### Pergunta 1 → b

- Lucas nasceu depois de 2/1/2012, então é menor de 16 anos.
- Menores de 16 anos não entram na parte B (que é só para quem tem 16 anos ou mais). Eles vão na seção do imposto residencial, na linha 16歳未満の扶養親族 (jūroku-sai miman no fuyō shinzoku).
- Erro comum: marcar "a" (colocar junto com os irmãos) ou "c" (achar que criança não precisa constar).
- Fonte: ✅ exemplo oficial, p.1 (parte B: "16 anos ou mais") e p.2 (seção 4 ❶)

### Pergunta 2 → b

- O formulário pede a renda líquida (shotoku), não o salário bruto (shūnyū).
- Pela tabela oficial, um salário bruto de ¥1.690.000 equivale a uma renda líquida de ¥950.000.
- Como ¥950.000 está dentro do limite da parte A (até ¥950.000), Ana entra como cônjuge na parte A.
- Erro comum: marcar "a" (escrever o salário bruto) ou "d" (achar que quem trabalha não pode entrar).
- Fonte: ✅ exemplo oficial, p.1 (A ❶) e tabela de referência, p.2

### Pergunta 3 → c

- Pedro tem 17 anos, então só pode entrar como dependente comum (扶養親族, fuyō shinzoku), que tem limite de salário bruto de ¥1.360.000.
- Ele ganha ¥1.500.000, acima do limite. Não entra como dependente.
- A categoria especial 特定親族 (tokutei shinzoku), que aceita renda maior, só vale de 19 a 22 anos. Pedro é novo demais.
- Erro comum: marcar "a" (não conferir o limite) ou "b" (confundir com a categoria de 19 a 22 anos).
- Fonte: ✅ exemplo oficial, p.1 (B, definição de 扶養親族) e tabela, p.2

### Pergunta 4 → c

- Júlia nasceu entre 2/1/2005 e 1/1/2009, então está na faixa de 19 a 22 anos.
- O salário bruto dela (¥1.600.000) fica entre ¥1.360.001 e ¥1.740.000, ou seja, a renda líquida fica entre ¥620.001 e ¥1.000.000.
- Nessa faixa, ela entra na parte B marcando 特定親族 (tokutei shinzoku).
- Erro comum: marcar "a" (achar que, ganhando mais que o Pedro, ela também ficou de fora) ou "b" (essa opção é para quem tem renda líquida de até ¥620.000).
- Fonte: ✅ exemplo oficial, p.1 (B ②) e p.2 (❺)

### Por que esta família funciona

- As perguntas 3 e 4 formam uma "pegadinha" em par: a filha que ganha MAIS entra, e o filho que ganha MENOS fica de fora. Só acerta quem entende a regra da idade.
- Cada pergunta testa uma armadilha diferente e tem uma única resposta correta.
- Nenhuma pergunta depende de regra marcada com ⚠️.
- Os valores de Ana estão exatamente na tabela oficial, então ninguém precisa fazer contas.

## Parte 4 — Para conferir antes de publicar

- [ ] Ler a ficha e confirmar que está clara para quem não conhece o assunto
- [ ] Fazer as 4 perguntas ao NotebookLM e ver se ele acerta
- [ ] Confirmar no Forms que a ordem das alternativas é embaralhada (opção do modo teste)