# Segmentação de Clientes com Auto Machine Learning

Segmentação de clientes é a divisão de clientes e potenciais cliente em segumentos ou grupos. Esses grupos possuem características comuns e isso irá facilitar o trabalho da área de Marketing e de Vendas. Com a segmentação de clientes a empresa pode focar naquele grupo que é mais responsável pelo lucro da empresa e permite a formulação de estratégias de preços, promoções, formas de fidelizar esses clientes, etc.

![image](https://user-images.githubusercontent.com/89540415/220916118-17f30870-fae1-487e-ab58-3fa9dd08cb65.png)

Algumas vantagens de segmentação de clientes:

* gera otimização de tempo e de recursos (esforços podem ser direcionados para um grupo menor de clientes, mas esse grupo pode ser mais rentável para a empresa), que permite um maior sucesso para a área comercial;

* Permite identificação de futuros clientes com mais similaridades com clientes atuais mais rentáveis;

* Melhora o desempenho da empresa em relação aos seus concorrentes, visto que consegue administrar melhor os seus clientes.

Há algumas técnicas podem ser usadas para esse trabalho de agrupamento, como a geográfica (segmentar os clientes pela sua localização, filtrando por bairro, cidade, estado ou País), demográfica (B2B e B2C), Psicográfica (estilo de vida, opiniões, valores, etc.) e Comportamental (gostos, preferências e hábitos).

Nesse projeto irei trabalhar com a base de dados com dados de 9000 titulares de cartão de crédito ativo em um período de seis meses. Ao todo são 18 variáveis comportamentais. Entretanto, ao invés utilizar as técnicas convencionais de segmentação irei utilizar modelos de machine learning de agrupamento para gerar clusters de clientes para definir uma estratégia de marketing.

As variáveis da base de dados são:

---



CUST ID : Identificação do titular do cartão de crédito (categórico);

BALANCE : Saldo restante na conta para fazer compras;

BALANCEFREQUENCY : com que frequência o saldo é atualizado, pontuação entre 0 e 1 (1 = atualizado com frequência, 0 = não atualizado com frequência);

PURCHASES : Valor das compras realizadas a partir da conta;

ONEOFFPURCHASES : Valor máximo da compra realizada de uma só vez;

INSTALLMENTSPURCHASES : Valor da compra realizada a prazo;

CASHADVANCE : Antecipação dado pelo usuário;

PURCHASESFREQUENCY: Frequência com que as compras estão sendo feitas, pontuação entre 0 e 1 (1 = frequentemente comprado, 0 = não frequentemente comprado);

ONEOFFPURCHASESFREQUENCY : Com que frequência as compras acontecem de uma vez (1 = frequentemente comprado, 0 = não frequentemente comprado);

PURCHASESINSTALLMENTSFREQUENCY : Frequência com que as compras a prazo estão sendo feitas (1 = frequentemente, 0 = não frequentemente);

CASHADVANCEFREQUENCY : Frequência com que o dinheiro é pago

antecipadamente .

CASHADVANCETRX : Número de transações feitas com "Cash in Advance"

PURCHASES TRX : Numéro de transações de compra feito;

CREDITLIMIT : Limite do Cartão de Crédito para;

PAYMENTS : Valor do pagamento feito pelo usuário;

MINIMUM_PAYMENTS : Valor mínimo dos pagamentos feitos pelo usuário;

PRCFULLPAYMENT : Porcentagem do pagamento total pago pelo usuário;

TENURE : Posse do serviço de cartão de crédito para o usuário

---



A base de dados pode ser acessada em [aqui](https://www.kaggle.com/datasets/arjunbhasin2013/ccdata).
