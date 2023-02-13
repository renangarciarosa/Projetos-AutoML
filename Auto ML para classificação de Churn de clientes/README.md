# Auto-Sklearn para previsão de Churn

Nesse projeto eu irei aplicar a biblioteca de Auto Machine Learning Auto-Sklearn para gerar um modelo que preveja o Churn de clientes de uma empresa de Telecomunicações. A vantagem do processo de Auto Machine Learning é que todo processo de escolha, treinamento e tunning do modelo é algo automático, permitindo que tempo e esforço sejam aplicados para outras áreas do projeto. Além dessa biblioteca usarei algoritmos de reamostragem de dados para realizar o rebalanceamento das classes da variável alvo.

# O que é churn ?

A rotatividade de clientes é a percentagem de clientes que pararam de usar o produto ou serviço de sua empresa durante um determinado período de tempo. Uma das maneiras de calcular uma taxa de churn é dividir o número de clientes perdidos durante um determinado intervalo de tempo pelo número de clientes ativos no início do período. Por exemplo, se você conseguiu 1.000 clientes e perdeu 50 no mês passado, sua taxa de rotatividade mensal é de 5%.

Prever a rotatividade de clientes é um problema de negócio desafiador, mas extremamente importante, especialmente em setores onde o custo de aquisição de clientes (CAC) é alto, como tecnologia, telecomunicações, finanças, etc. A capacidade de prever que um determinado cliente corre um alto risco de rotatividade, embora ainda haja tempo para fazer algo a respeito, representa uma enorme fonte potencial de receita adicional para as empresas.

O objetivo principal do modelo preditivo de rotatividade de clientes é reter clientes com maior risco de rotatividade, envolvendo-se de forma proativa com eles. Por exemplo: Ofereça um voucher de oferta ou qualquer preço promocional e retenha-o por mais um ou dois anos para estender seu valor vitalício para a empresa.
Existem dois conceitos gerais para entender aqui:

* Queremos um modelo preditivo de rotatividade de clientes para prever a rotatividade com antecedência (digamos com um mês de antecedência, três meses de antecedência ou até seis meses de antecedência - tudo depende do caso de uso). Isso significa que você deve ser extremamente cuidadoso com a data limite, ou seja, você não deve usar nenhuma informação após a data limite como uma feature no modelo de machine learning, caso contrário, haverá vazamento. O período anterior à data limite é conhecido como Event.
* Normalmente, para previsão de rotatividade de clientes, você terá que trabalhar um pouco para criar uma coluna de destino (target), geralmente não está disponível na forma que você gostaria. Por exemplo, você deseja prever se o cliente se desligará no próximo trimestre, e assim irá iterar por todos os clientes ativos a partir da data limite do evento e verificar se eles deixaram a empresa no próximo trimestre ou não (1 para sim, 0 para não). O trimestre, neste caso, é denominado Janela de desempenho (Performance Window).

## Workflow do modelo de Churn do Cliente

Agora que você entende como os dados são originados e a coluna churn target esta criada (o que é uma das partes mais desafiadoras do problema), vamos discutir como esse modelo de machine learning será usado nos negócios. Leia o diagrama abaixo da esquerda para a direita:

Um modelo é treinado nos dados históricos de rotatividade do cliente (período de evento para features X e janela de desempenho para variável de destino).
Todos os meses, a base de clientes ativos é passada para o Modelo Preditivo de Machine Learning para retornar a probabilidade de churn para cada cliente (no jargão empresarial, isso às vezes é chamado de pontuação de rotatividade - score of churn).

A lista será classificada do maior para o menor valor de probabilidade (ou score como eles dizem) e as equipes de retenção de clientes começarão a se envolver com o cliente para interromper a rotatividade, normalmente oferecendo algum tipo de promoção, gift card, etc. para reter mais alguns anos.
Os clientes que têm uma probabilidade muito baixa de rotatividade (ou essencialmente o modelo prevê não rotatividade - no-churn) são clientes satisfeitos. Nenhuma ação é executada sobre eles.

Etapas
1- Instalação de bibliotecas;

2- Importação das bibliotecas;

3- Importação da base de dados;

4- Análise Exploratória dos dados;

5- Transformações dos dados;

6- Modelagem dos dados (separação de dados de treino e teste, reamostragem dos dados, treinamento dos algoritmos e avaliação dos modelos);

7- Conclusão.

