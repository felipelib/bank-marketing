# bank-marketing
📌 Descrição do Projeto

Um banco português realizou campanhas de marketing direto (via chamadas telefônicas) para vender depósitos a prazo. Ligar indiscriminadamente para qualquer pessoa representa um alto custo operacional com baixo retorno, um verdadeiro "tiro no escuro".

O objetivo deste projeto é identificar o perfil dos clientes com maior probabilidade de adquirir o produto, permitindo que o banco crie campanhas mais direcionadas, reduza custos e aumente a taxa de conversão.

O projeto está dividido em duas partes:
- Análise Exploratória de Dados (EDA)
- Modelo de Classificação


🗃️ Sobre os Dados

Dataset obtido no repositório da UCI Machine Learning Repository, contendo 45.211 registros e 17 colunas sobre campanhas de telemarketing de um banco português. Variáveis presentes no dataset:

Informações sobre o possível cliente:
- age (idade): A idade do cliente.

- job (trabalho): Tipo de emprego.

- marital (estado Civil): Estado civil.

- education (educação): Nível de escolaridade.

- default (inadimplência): O cliente tem crédito em inadimplência/calote?

- balance (saldo): Saldo médio anual em euros.

- housing (habitação): Tem empréstimo imobiliário/financiamento da casa?

- loan (empréstimo): Tem empréstimo pessoal?


Informações sobre o contato da campanha atual:

- contact (contato): Tipo de comunicação do contato.

- month (mês): Mês do último contato.

- day (dia): Dia do mês do último contato.

- duration (duração): Duração do último contato em segundos.

- campaign (campanha): Número de contatos realizados durante esta campanha para este cliente.


Informações sobre o contato de campanhas anteriores:

- pdays (dias passados): Número de dias que se passaram desde que o cliente foi contatado pela última vez em uma campanha anterior (-1 significa que o cliente não foi contatado anteriormente).

- previous (anteriores): Número de contatos realizados antes desta campanha para este cliente.

- poutcome (resultado anterior): Resultado da campanha de marketing anterior.

Target:

- y: O cliente subscreveu/assinou um depósito a prazo?


📈 Parte 1 — Análise Exploratória de Dados (EDA)

Principais Descobertas

Perfil dos clientes mais contatados pelo banco (baixa conversão):

Idade entre 30 e 50 anos
Empregos estáveis: operário, gerência, técnico e administrativo
Ensino médio completo
Casados, com empréstimo imobiliário e saldo abaixo de €1.000

Perfil dos clientes com maior taxa de conversão:

Abaixo de 25 anos ou acima de 60 anos
Estudantes, aposentados ou desempregados
Ensino superior completo
Solteiros, sem dívidas e com saldo acima de €1.000
Já haviam sido contatados em campanhas anteriores

Sazonalidade:

Os melhores meses de conversão são março, setembro e dezembro
Existe um trade-off claro: meses com maior volume de ligações apresentam menor taxa de conversão

Operação:

O número de tentativas de contato tem pouco impacto na conversão
Existe uma correlação direta entre a duração da ligação e a conversão — ligações mais longas convertem significativamente mais
