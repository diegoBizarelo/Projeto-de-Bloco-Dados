# Projeto-de-Bloco-Dados

O Projeto consiste em analisar o consumo de energia.

Estrutura do dataset:
data hora ano-mês-dia hora: minuto: segundo
Eletrodomésticos, uso de energia em Wh
luzes, uso de energia de luminárias na casa em Wh
T1, Temperatura na área da cozinha, em Celsius
RH1, Umidade na área da cozinha, em% T2, Temperatura na área da sala, em Celsius RH2, Umidade na área da sala, em%
T3, Temperatura na área da lavanderia
RH3, Umidade na área da lavanderia, em% T4, Temperatura na sala do escritório, em Celsius RH4, Umidade na sala do escritório, em%
T5, Temperatura no banheiro, em graus Celsius
RH5, Umidade no banheiro, em% T6, Temperatura fora do prédio (lado norte), em Celsius RH6, Umidade fora do prédio (lado norte), em%
T7, Temperatura na sala de engomar, em Celsius
RH7, Umidade na sala de engomar, em% T8, Temperatura no quarto adolescente 2, em Celsius RH8, Umidade no quarto adolescente 2, em%
T9, Temperatura no quarto dos pais, em graus Celsius
RH9, Umidade no quarto dos pais, em% a, Temperatura externa (da estação meteorológica de Chievres), em Celsius Pressão (da estação meteorológica de Chievres), 
  em mm Hg RHout, Umidade externa (da estação meteorológica de Chievres), em%
Velocidade do vento (da estação meteorológica de Chievres), em m / s
Visibilidade (da estação meteorológica de Chievres), em km
Tdewpoint (da estação meteorológica de Chievres), ° C
rv1, variável aleatória 1, não dimensional
rv2, variável aleatória 2, não dimensional

Onde indicado, os dados horários (então interpolados) da estação meteorológica do aeroporto 
  mais próximo (Aeroporto de Chievres, Bélgica) foram baixados de um conjunto de dados público em Reliable Prognosis,
  rp5.ru. A permissão foi obtida do Reliable Prognosis para a distribuição dos 4,5 meses de dados meteorológicos.
