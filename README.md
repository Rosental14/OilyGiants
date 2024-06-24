# OilyGiants  

## Descrição  

O objetivo deste projeto é encontrar os melhores lugares para o desenvolvimento de novos poços de petróleo. Utilizando dados sobre amostras de petróleo de três regiões, construiremos um modelo de regressão linear para prever o volume de reservas em novos poços e, assim, escolher a região com a margem de lucro mais alta. A técnica de Bootstrapping será utilizada para analisar o lucro potencial e os riscos.

Informações extras: Ao explorar a região, um estudo de 500 pontos será realizado e os melhores 200 pontos são selecionados para calcular o lucro. O orçamento para o desenvolvimento de 200 poços de petróleo é de 100 milhões de dólares. Um barril de petróleo bruto traz 4.5 dólares de receita. A receita de uma unidade de produto é 4.500 dólares (o volume de reservas está em milhares de barris).  


## Instalação  

### Pré-requisitos  

* **Python 3.x:** (Qualquer versão do Python 3, como 3.6, 3.7, 3.8, etc.)  
  
* **Bibliotecas Python:**  
  
  * pandas
  * numpy
  * scikit-learn
  * matplotlib
  * seaborn  

### Instruções de Instalação  

1.	**Clone o repositório:** git clone https://github.com/Rosental14/OilyGiants.git
2.	**Navegue até o diretório do projeto**
3.	**Instale as dependências:** pip install -r requirements.txt

## Uso  

1. **Abra o Jupyter Notebook**
2. **Navegue até o arquivo:** projeto_oilygiant.ipynb e abra-o.
3. **Execute as células sequencialmente para reproduzir a análise e a criação do modelo.**  
   
## Funcionalidades  

### Etapas Iniciais  

* **Importação de Bibliotecas:** pandas, numpy, scikit-learn, matplotlib e seaborn.    
* **Leitura dos Dados:** Carregamento dos arquivos geo_data_0.csv, geo_data_1.csv e geo_data_2.csv e visualização das primeiras linhas dos DataFrames.   
* **Informações Gerais:** Impressão das informações gerais dos DataFrames para conferir tipos de dados e valores ausentes.  


### Treinamento e Validação do Modelo  
* **Divisão dos Dados:** Divisão dos dados em conjuntos de treinamento e validação na proporção 75:25;  
* **Padronização dos Dados:** transformação dos dados para escalar padronizadas evitando a interpretação equivocada por parte do modelo;  
* **Treinamento do Modelo:** Treinamento de um modelo de regressão linear com os dados de treinamento;  
* **Predições:** Realização de predições com o conjunto de validação;  
* **Avaliação do Modelo:** Impressão do volume médio previsto de reservas, do volume médio real e do REQM do modelo;  
* **Análise dos Resultados:** Análise dos resultados obtidos para cada região;  


### Preparação para o Cálculo de Lucro  

* **Cálculo do Mínimo Volume Médio Necessário:** Volume médio necessário para evitar prejuízos e comparação com o volume médio de cada região;  
* **Conclusões Preliminares:** Fornecimento de conclusões sobre a etapa de preparação para o cálculo de lucro.  


### Cálculo de Lucro  

* **Seleção dos Melhores Poços:** Seleção de uma amostra aleatória de 500 pontos e posterior escolha dos 200 poços com os valores mais altos previstos em cada uma das 3 regiões;  
* **Soma do Volume de Reservas:** Sumarização do volume alvo de reservas de acordo com as predições;  
* **Cálculo do Lucro:** Cálculo do lucro potencial dos 200 melhores poços por região;  
* **Conclusões:** Sugestão de uma região para o desenvolvimento de poços de petróleo e justificativa da escolha.  


### Análise de Riscos e Lucros  

* **Técnica de Bootstrapping:** Uso da técnica de bootstrapping com 1.000 amostras para encontrar a distribuição de lucros;   
* **Cálculo de Métricas:** Cálculo do lucro médio, intervalo de confiança de 95% e risco de prejuízo;  
* **Conclusões Finais:** Sugestão de uma região para o desenvolvimento de poços de petróleo e justificativa da escolha, verificando se a escolha corresponde à etapa anterior.  

## Créditos
* **Autor:** Renan Rosental  

## Contato
Para dúvidas e feedback, entre em contato via e-mail: renan.engal@gmail.com