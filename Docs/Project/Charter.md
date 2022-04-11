# Project Charter

## Objetivo
O Projeto consiste em analisar o consumo de energia de um domícilio.
Caso o consumo diário ultrapasse a média do dia estimada daquele mês é emitido um alerta.


## Arquitetura
* Dados
  * Dados obtedos no kaggle de sensores inteligentes para 
* Movimentação de dados do ambiente local para AWS usando script para enviar dados.
  * Todos os dados,
  * Após alguma pré-agregação no ambiente local.

* Ferramentas e recursos utilizados
  * Python para construção de recursos, agregação e amostragem
  * AWS IoT para envio de dados e sinalização de um consumo alto no dia através do device shadow
  * Jupter Notebook para criação dos scripts.
  * AWS IoT
  
## Scripts
Os scripts do projeto foram escritos em phyton e salvos em formato de notebook.

## Fluxo de execução do projeto
Os dados base se encontram no diretório Data\RAW do projeto. Não sendo necessário baixar.

![]('Digrama_Projeto.png')

*Ordem de execução dos scripts
	1. Ir ao diretório Code\DataPrep e abrir o notebook 'Limpar_de_Dados' e excutar os scripts
		dados filtrados serão armazenados em Data\Processed
	2. Ir ao diretório Code\Operationalization e abrir o notebook 'connect_to_aws' e excutar os scripts
		para enviar dados a AWS.
	3. O Modelo de predição se encontra em Code\Model em formato de notebook.

*Comandos para bibliotecas necessárias
pip install Prophet
pip install awscrt
pip install awsiotsdk


## Procolos de comunicação
* Protocolo mqqt para enviar dados à AWS

## Pessoas envolvidas
* Quem está envolvido no projeto:
	* Diego Bizarelo
		* Data Scientist
		* Lider de Projeto
	* Fernando Ferreira
		* Professor