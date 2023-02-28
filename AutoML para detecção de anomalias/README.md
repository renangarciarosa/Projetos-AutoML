# Identificando fraudes com PyCaret
É importante que as empresas de cartão de crédito sejam capazes de reconhecer transações fraudulentas com cartão de crédito para que os clientes não sejam cobrados por itens que não compraram. Essas fraudes podem ocorrer por conta da falta de atenção dos clientes das operadores de cartão quando os cartões ou informações do cartão foram fornecidos.

O Brasil é o segundo país com mais fraudes em cartão de crédito em toda América Latina, atrás do México. Principalmente, durante a pandemia do coronavírus, provavelmente por conta da alta demanda de serviços digitais e e-commerce, o número de casos de fraudes de cartão de crédito e débito dispararam e mais do que dobraram.

# Sobre o projeto
Nesse projeto eu irei aplicar modelos de detecção de anomalias, ou seja, valores que são discrepantes ou muitos diferentes da população que temos e depois analisarei quais desses resultados são ou não fraudes; visto que já tenho os resultados rotulados irei os comparar com as anomalias detectadas.

A atividade de detecção de anomalias é um processo não supervisionado, semelhante ao processo de agrupamento, mas no nosso caso irei usar também métricas de avaliação de modelos de classificação para ver o desempenho dos modelos.

# Base de dados
Os dados foram obtidos [aqui](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud) e a base de dados possui 31 features.

Conforme informações do link:

Os conjuntos de dados contêm transações feitas por cartões de crédito em setembro de 2013 por titulares de cartões europeus. Este conjunto de dados apresenta as transações que ocorreram em dois dias, onde temos 492 fraudes em 284.807 transações. O conjunto de dados é altamente desequilibrado, a classe positiva (fraudes) é responsável por 0,172% de todas as transações.

Ele contém apenas variáveis ​​de entrada numéricas que são o resultado de uma transformação PCA. Infelizmente, devido a questões de confidencialidade, não podemos fornecer os recursos originais e mais informações básicas sobre os dados. Os recursos V1, V2,… V28 são os componentes principais obtidos com o PCA, os únicos recursos que não foram transformados com o PCA são 'Tempo' e 'Quantidade'. O recurso 'Tempo' contém os segundos decorridos entre cada transação e a primeira transação no conjunto de dados. O recurso 'Amount' é o Amount da transação, esse recurso pode ser usado por exemplo, aprendizado dependente de custos. O recurso 'Classe' é a variável de resposta e assume o valor 1 em caso de fraude e 0 em caso contrário.

