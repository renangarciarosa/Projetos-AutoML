# Aplicando AutoML para classificação de saúde fetal
A redução da mortalidade infantil está refletida em vários Objetivos de Desenvolvimento Sustentável das Nações Unidas e é um indicador chave do progresso humano. A ONU espera que, até 2030, os países acabem com as mortes evitáveis ​​de recém-nascidos e crianças menores de 5 anos de idade, com todos os países visando reduzir a mortalidade de menores de 5 anos para pelo menos 25 por 1.000 nascidos vivos.

Paralela à noção de mortalidade infantil está, naturalmente, a mortalidade materna, que é responsável por 295.000 mortes durante e após a gravidez e o parto (em 2017). A grande maioria dessas mortes (94%) ocorreu em locais com poucos recursos e a maioria poderia ter sido evitada.

Diante do exposto, os Cardiotocogramas (CTGs) são uma opção simples e de baixo custo para avaliação da saúde fetal, permitindo aos profissionais de saúde atuarem na prevenção da mortalidade infantil e materna. O próprio equipamento funciona enviando pulsos de ultrassom e lendo sua resposta, lançando luz sobre a frequência cardíaca fetal (FCF), movimentos fetais, contrações uterinas e muito mais.

![image](https://user-images.githubusercontent.com/89540415/221207377-65e0b411-6268-405c-87e9-25d33aa1c1b2.png)

## Dados
As variáveis da base de dados são :

baseline value : Frequência cardíaca fetal basal (FHR);

accelerations: Número de acelerações por segundo;

fetal_movement: Número de movimentos fetais por segundo;

uterine_contractions: Número de contrações uterinas por segundo;

light_decelerations: Número de LDs por segundo;

severe_decelerations: Número de SDs por segundo;

prolongued_decelerations: Número de PDs por segundo;

abnormal_short_term_variability: Porcentagem de tempo com variabilidade anormal de curto prazo;

mean_value_of_short_term_variability: Valor médio da variabilidade de curto prazo;

percentage_of_time_with_abnormal_long_term_variability: Porcentagem de tempo com variabilidade anormal de longo prazo;

mean_value_of_long_term_variability: Valor médio da variabilidade de longo prazo;

histogram_width: Largura do histograma feito usando todos os valores de um registro;

histogram_min: Valor mínimo do histograma;

histogram_max: Valor máximo do histograma;

histogram_number_of_peaks: Número de picos no histograma do exame;

histogram_number_of_zeroes: Número de zeros no histograma do exame;

histogram_mode: Moda histograma;

histogram_mean: Média histagrama;

histogram_median: mediana histograma;

histogram_variance: Variação histórica;

histogram_tendency: Tendência do histograma;

fetal_health: Saúde fetal(1 - Normal, 2 - Suspeito, 3 - Patológico).

[Este conjunto de dados](https://www.kaggle.com/code/karnikakapoor/fetal-health-classification/data) contém 2.126 registros de características extraídas de exames de cardiotocograma.
