# Aplicando Auto Machine Learning (PyCaret) para previsão de risco de câncer cervical

![image](https://user-images.githubusercontent.com/89540415/218786314-acbb3960-0963-4921-8798-243a18c67550.png)

O câncer cervical ou câncer do colo do útero é um tipo de tumor maligno que afeta as mulheres e é causado pelo papiloma vírus humano (ou vírus HPV). As pessoas que fazem sexo sem proteção, que têm múltiplos parceiros sexuais, ou tiveram as primeiras relações sexuais em idade precoce são mais propensas a contrair HPV e desenvolver câncer cervical; além disso pessoa portadoras de HIV também possuem um alto risco de contrair essa enfermidade. Outros fatores tabém influencia como : fumo, histórico familiar de câncer cervical e histórico de doenças sexualmente transmissíveis. Entretanto mesmo sendo comum entre mulheres ainda é considerado um tumor raro, havendo menos de 150 mil casos por ano no Brasil.

Como todo tipo de câncer é necessário um diagnóstico médico para que haja a identificação e quanto mais cedo a detecção desse tipo de câncer, maiores serão as chances de sucesso de cura, pois o tratamento pode ser feito a tempo de evitar etapas consideradas críticas, como a metástase (etapa em que os tumores malignos chagam para outros órgãos do corpo).

# Base de dados
A base de dados pode ser obtida [aqui](https://www.kaggle.com/datasets/loveall/cervical-cancer-risk-classification). Essa base possui 858 linhas e 36 colunas.

Este arquivo contém uma lista de fatores de risco para câncer cervical que leva a um exame de biópsia.

Cerca de 11.000 novos casos de câncer cervical invasivo são diagnosticados a cada ano nos Estados Unidos. No entanto, o número de novos casos de câncer cervical tem diminuído constantemente nas últimas décadas. Embora seja o tipo de câncer mais evitável, a cada ano o câncer cervical mata cerca de 4.000 mulheres nos Estados Unidos e cerca de 300.000 mulheres em todo o mundo. Nos Estados Unidos, as taxas de mortalidade por câncer cervical caíram 74% de 1955 a 1992, graças ao aumento da triagem e detecção precoce com o teste de Papanicolaou.

**IDADE**: Cinquenta por cento dos diagnósticos de câncer cervical ocorrem em mulheres de 35 a 54 anos e cerca de 20% em mulheres com mais de 65 anos. A idade média do diagnóstico é 48 anos. Cerca de 15% das mulheres desenvolvem câncer cervical entre as idades de 20 a 30 anos. O câncer cervical é extremamente raro em mulheres com menos de 20 anos. No entanto, muitas mulheres jovens são infectadas com vários tipos de vírus do papiloma humano, o que pode aumentar o risco de contrair câncer cervical no futuro. Mulheres jovens com alterações iniciais anormais que não realizam exames regulares apresentam alto risco de câncer localizado aos 40 anos e de câncer invasivo aos 50 anos.

**FATORES SOCIOECONÔMICOS E ÉTNICOS**: Embora a taxa de câncer cervical tenha diminuído entre os caucasianos e mulheres afro-americanas nas últimas décadas, permanece muito mais prevalente em afro-americanas - cujas taxas de mortalidade são duas vezes mais altas que as mulheres brancas. As mulheres hispano-americanas têm mais de duas vezes o risco de câncer cervical invasivo do que as mulheres brancas, também devido a uma menor taxa de rastreamento. Essas diferenças, no entanto, quase certamente se devem a diferenças sociais e econômicas. Numerosos estudos relatam que altos níveis de pobreza estão associados a baixas taxas de rastreamento. Além disso, a falta de seguro saúde, transporte limitado e dificuldades com a linguagem impedem o acesso de uma mulher pobre aos serviços de rastreamento.

**ALTA ATIVIDADE SEXUAL:** O vírus do papiloma humano (HPV) é o principal fator de risco para o câncer cervical. Em adultos, o fator de risco mais importante para o HPV é a atividade sexual com uma pessoa infectada. As mulheres com maior risco de câncer cervical são aquelas com histórico de múltiplos parceiros sexuais, relações sexuais com 17 anos ou menos, ou ambos. Uma mulher que nunca foi sexualmente ativa tem um risco muito baixo de desenvolver câncer cervical. A atividade sexual com vários parceiros aumenta a probabilidade de muitas outras infecções sexualmente transmissíveis (clamídia, gonorreia, sífilis). Estudos descobriram uma associação entre a clamídia e o risco de câncer cervical, incluindo a possibilidade de a clamídia prolongar a infecção por HPV.

**HISTÓRICO DA FAMÍLIA:** As mulheres têm maior risco de câncer cervical se tiverem um parente de primeiro grau (mãe, irmã) que teve câncer cervical.

**USO DE CONTRACEPTIVOS ORAIS:** Estudos relataram uma forte associação entre câncer cervical e o uso de contracepção oral (ACO) em longo prazo. Mulheres que tomam pílulas anticoncepcionais por mais de 5 a 10 anos parecem ter um risco muito maior de infecção por HPV (até quatro vezes maior) do que aquelas que não usam ACOs. (Mulheres que tomam ACO por menos de 5 anos não têm um risco significativamente maior.) As razões para esse risco do uso de ACO não são totalmente claras. Mulheres que usam ACOs podem ter menos probabilidade de usar diafragma, preservativos, ou outros métodos que oferecem alguma proteção contra doenças sexualmente transmissíveis, incluindo HPV. Algumas pesquisas também sugerem que os hormônios nos OCs podem ajudar o vírus a entrar no material genético das células cervicais.

**TER MUITOS FILHOS:** Estudos indicam que ter muitos filhos aumenta o risco de desenvolver câncer cervical, principalmente em mulheres infectadas com HPV.

**FUMO:** Fumar está associado a um risco maior de alterações pré-cancerosas (displasia) no colo do útero e de progressão para câncer cervical invasivo, especialmente para mulheres infectadas com HPV.

**IMUNOSUPPRESSÃO:** Mulheres com sistema imunológico fraco (como aquelas com HIV/AIDS) são mais suscetíveis a adquirir HPV. Pacientes imunocomprometidos também apresentam maior risco de desenvolver pré-câncer cervical rapidamente para câncer invasivo.

**DIETHYLSTILBESTROL (DES):** De 1938-1971, dietilestilbestrol (DES), um medicamento relacionado ao estrogênio, foi amplamente prescrito para mulheres grávidas para ajudar a prevenir abortos espontâneos. As filhas dessas mulheres correm maior risco de câncer cervical. O DES não é mais prescrito.

O objetivo desse projeto será utilizar a biblioteca de Auto Machine Learning Pycaret para gerar um modelo que possa prever
