# Modelagem de preços de casas com AutoML

![image](https://user-images.githubusercontent.com/89540415/222198945-ba864d09-36db-4278-8f67-f0e19e20e4ae.png)

Nesse pequeno projeto serão aplicadas ferramentas de análise, processamento de modelagem em um conjunto de dados de uma competição da Kaggle, que tem por objetivo a modelagem de preços de casas com métodos de regressão.

São ao todo cerca de 79 variáveis explicativas que descrevem (quase) todos os aspectos de casas residenciais em Ames, Iowa. Esses dados são uma versão ampliada do conjunto de dados Boston Housing. É disponibilizado ao participante cerca de dois datasets, um de treino e outro de teste. O dataset de treino além das features para treinamento do algoritmo, há também a variável target ou alvo (o preço da casa). Na dataset de teste (que será usado para gerar as previsões) apenas as features.

# Dados
Os dados da competição podem ser encontrados [aqui](https://www.kaggle.com/c/house-prices-advanced-regression-techniques/data). São 79 features e 1 variável target são:

SalePrice : o preço de venda da propriedade em dólares (Essa é a variável alvo)

MSSubClass : A classe de construção

MSZoning : A classificação geral de zoneamento

LotFrontage : pés lineares de rua conectados à propriedade

LotArea : tamanho do lote em pés quadrados

Rua : Tipo de acesso rodoviário

Beco : Tipo de acesso ao beco

LotShape : forma geral da propriedade

LandContour : Planicidade da propriedade

Utilities : Tipo de utilitários disponíveis

LotConfig : configuração do lote

LandSlope : declive de propriedade

Neighborhood : localizações físicas dentro dos limites da cidade de Ames

Condition1 : Proximidade da estrada principal ou ferrovia

Condition2 : Proximidade da estrada principal ou ferrovia (se houver um segundo)

BldgType : Tipo de habitação

HouseStyle : Estilo de habitação

OverallQual : Qualidade geral do material e acabamento

OverallCond : classificação geral das condições

Yearbuilt : data de construção original

YearRemodAdd : data de remodelação

RoofStyle : Tipo de telhado

RoofMatl : Material do telhado

Exterior1st : revestimento exterior em casa

Exterior2nd : Cobertura externa da casa (se houver mais de um material)

MasVnrType : Tipo de folheado de alvenaria

MasVnrArea : Área de folheado de alvenaria em pés quadrados

ExterQual : Qualidade do material exterior

ExterCond : Condição atual do material no exterior

Foundation : Tipo de fundação

BsmtQual : Altura do porão

BsmtCond : Condição geral do porão

BsmtExposure : Paredes subterrâneas no nível da entrada ou do jardim

BsmtFinType1 : Qualidade da área acabada do porão

BsmtFinSF1 : pés quadrados com acabamento tipo 1

BsmtFinType2 : Qualidade da segunda área finalizada (se presente)

BsmtFinSF2 : Tipo 2 pés quadrados com acabamento

BsmtUnfSF : pés quadrados inacabados da área do porão

TotalBsmtSF : pés quadrados totais da área do porão

Heating : Tipo de aquecimento

HeatingQC : Qualidade e condição do aquecimento

CentralAir : ar condicionado central

Electrical : Sistema elétrico

1stFlrSF : Primeiro andar pés quadrados

2ndFlrSF : Segundo andar, pés quadrados

LowQualFinSF : pés quadrados acabados de baixa qualidade (todos os pisos)

GrLivArea : Área útil acima do nível do solo (pés quadrados)

BsmtFullBath : banheiros completos no porão

BsmtHalfBath : lavabos no porão

FullBath : banheiros completos acima da série

HalfBath : banhos de meia acima da série

Bedroom : Número de quartos acima do nível do porão

Kitchen : Número de cozinhas

KitchenQual : Qualidade da cozinha

TotRmsAbvGrd : total de quartos acima da classe (não inclui banheiros)

Funcional : classificação de funcionalidade doméstica

Fireplaces : Número de lareiras

FireplaceQu : qualidade da lareira

GarageType : Localização da garagem

GarageYrBlt : ano em que a garagem foi construída

GarageFinish : Acabamento interior da garagem

GarageCars : tamanho da garagem em capacidade do carro

GarageArea : tamanho da garagem em pés quadrados

GarageQual : Qualidade da garagem

GarageCond : Condição de garagem

PavedDrive : Entrada de automóveis pavimentada

WoodDeckSF : área de deck de madeira em pés quadrados

OpenPorchSF : área de varanda aberta em pés quadrados

EnclosedPorch : área de alpendre fechado em pés quadrados

3SsnPorch : Área da varanda de três estações em pés quadrados

ScreenPorch : Área da varanda da tela em pés quadrados

PoolArea : Área da piscina em pés quadrados

PoolQC : Qualidade da piscina

Fence : qualidade da cerca

MiscFeature : Recurso variado não coberto em outras categorias

MiscVal : $ Valor do recurso diverso

MoSold : Mês Vendido

YrSold : Ano Vendido

SaleType : Tipo de Venda

SaleCondition : Condição de Venda

# Etapas do projeto
1. Importação das bibliotecas;

2. Importação dos dados;

3. Análise Exploratória dos dados;

4. Tratamento dos dados;

5. Modelagem de AutoML;

6. Avaliação do modelo;

# Resultados

![image](https://user-images.githubusercontent.com/89540415/222199317-57d8bca0-4239-4cd7-8bbf-62df6c7bfd9d.png)

