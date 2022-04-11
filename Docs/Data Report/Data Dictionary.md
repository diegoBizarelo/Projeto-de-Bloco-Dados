# Dicionário dos Dados

## Estrutura dos dados dados em RAW

* Em Data/RAW encontra-se o arquivo D202 em formato csv para leitura dos dados

* Estrutura do dataset:
	* TYPE - Esta é uma coluna de informações. O valor é 'Uso elétrico' para todas as observações.
	* DATE - Data do consumo elétrico. Não há carimbo de data/hora neste campo.
	* START TIME - Hora de início do consumo.
	* END TIME - Horário de término do consumo
	* USAGE - Consumo em kWh
	* UNITS  - Esta coluna indica a unidade de medida. É kWh para todas as observações.
	* COST  - Custo de consumo em $ (DOLLAR).
	* NOTES  - Principalmente uma coluna vazia
	
![]('DATA_RAW.png')

## Tratamento dos dados
Os dados são tratados através do script Limpar_de_Dados em \Code\DataPrep.
Objetivo é representar o consumo diário de energia e a meta mensal que é definido no dispositivo.

## Estrtura dos dados em Processed

* Estrutura do dataset processado:
	* DATE - Data do consumo elétrico agrupo dia dia.
	* COMSUPTION_KWH - Quantidade de energia consumida em KWH no dia.
	* COST - Custo de consumo em $ (DOLLAR).
	* MOUNTH_GOAL - Meta de Consumo do mês
	
![]('DATA_Processed.png')
