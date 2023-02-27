# TPOT para classificação de preços de celulares
O objetivo desse projetio é utilizar uma biblioteca de AutoML (Auto Machine Learning) para criar um modelo de classificação para o preço de celulares. A biblioteca se chama TPOT e a sua função é automatizar todo processo de pipeline de machine learning e gerando um modelo com o melhor desempenho, por meio de algoritmos genéticos; ao invés de usar várias técnicas, vários parâmetros e realizar várias etapas dos processos, a biblioteca TPOT testa todos esses recursos, o que dá uma economia de tempo. Outra vantagem é que não é necessário escolher vários modelos (que nesse caso, são de classificação) de forma antecipada.

# Dados
Os dados usados nesse projeto podem ser obtidos [aqui](https://www.kaggle.com/datasets/iabhishekofficial/mobile-price-classification). São dados com características de celulares e são ao todo 20 features que são:

battery_power: Energia total que uma bateria pode armazenar de uma só vez, medida em mAh;

blue : Tem bluetooth ou não;

clock_speed: velocidade na qual o microprocessador executa instruções;

dual_sim: Tem suporte para dual sim ou não;

fc: Mega pixels da câmera frontal;

four_g: Tem 4G ou não;

int_memory: Memória interna em Gigabytes;

m_dep: Profundidade móvel em cm;

mobile_wt: Peso do telefone móvel;

n_cores: Número de núcleos do processador;

pc: Mega pixels da câmera principal;

px_height: Altura da resolução de pixels;

px_width: Largura de resolução de pixel;

ram: Memória de acesso aleatório em mega bytes;

sc_h: Altura da tela do celular em cm;

sc_w: Largura da tela do celular em cm;

talk_time: tempo que uma única carga de bateria durará;

three_g: Tem 3G ou não;

touch_screen: Possui tela sensível ao toque ou não;

wifi:Tem wifi ou não;

---



E o target (price_range, que é o preço) está definido da seguinte forma:

a) 0 (baixo custo);

b) 1 (custo médio);

c) 2 (alto custo);

d) 3 (custo muito alto).

---


