<div align="center">
<img src="images/pngwing.com.png" width=200>

# Desafio Alura Data Science Semana 2 Análise Exploratória dos Dados
<div align="left">
Plotagem de gráficos para melhor entendimento da correlação entre as demais variáveis e nossa variável alvo.
 
## Tecnologia

O software  usado neste projeto foi:

* Python version  3.9.5

## Serviços Usados

* Github
* Google Colab

## Bibliotecas Python

* Pandas
* Seaborn
* Matplotlib
* Dython

## Como foi feito

Será descrito abaixo através de textos e imagens.

Após importar os dados vamos plotar a distribuição de nossas variáveis. Assim, vamos plotar a distribuição da variável alvo.


<img src="images/img_001.png" width=300>

Há um desbalanceamento das variáveis assim seria possível utilizar metodologias como, UNDERSAMPLING,  OVERRSAMPLING ou SMOTE, mas optamos por manter a base adotar medidas para minimizar o desbalanceamento apenas em projetos futuros. Este projeto é apenas para criação de um modelo inicial. Mas devemos ficar atentos pois existe esta possibilidade de melhoria de modelo.
 
Após definir uma função simples para plotar os dados para visualizarmos o comportamento de algumas variáveis, começamos a plotar nossas variáveis.
Nesta variável abaixo o gráfico é muito similar assim ela parece ter pouca correlação, o que seria surpreendente até certo ponto, pois o cliente sênior tende a ter um padrão de consumo diferente, mas isso não influência sua permanência ou não na empresa.
 
<img src="images/comparativo maior 65.png">

Usando o método nomalize, podemos desempacotar as informações e exportá-las em colunas individuais, como podemos ver na imagem abaixo, o mesmo método foi aplicado em todas as colunas que possuíam esta mesma característica.

<img src="images/comparativo meses contrato.png">
Depois cada parte desempacotada foi adicionada a base principal e as colunas mãe forma excluídas, ficando com um aspecto melhor como podemos observar na imagem abaixo.

<img src="images/comparativo gasto mensal.png">
Começamos a etapa de procurar por inconsistências de dados, não localizamos valores vazios, tipo NaN ou Null.
depois verificamos que tínhamos ao invés de valores vazios ' ' simplesmente um espaço como valor. como podemos ver na imagem abaixo.

<img src="images/heat_map.png">
 
 Continuamos verificando valores e na coluna Senior, encontramos 0 e 1 em vez de yes e no então corrigimos padronizando a base.

<img src="images/churn_yes.png">

 Fizemos algumas checagens para verificar nas colunas com valores numéricos valores discrepantes ou negativos.
 mas não encontramos valores deste tipo.

<img src="images/churn_no.png">

Checamos qual o percentual do valor nulo, como o cliente informou que essa seria a variável alvo optamos por excluir as linhas pois elas representavam apenas perto de 3%

<img src="images/comparativo tipo contrato.png">

Verificamos que uma das variáveis numéricas estava com os valores armazenados como texto e convertemos o tipo para sanar esta inconsistência

<img src="comparativo internet.png">




## Recursos Usados

  - Importação de Database
  - Limpeza de dados
  - Criação de arquivo .csv
  

## Links

  - Repositório: https://github.com/Alexandremsn/desafio_alura_data_science/
  - Se for encontrado um bug, favor entrar em contato alexandremsneto1986@gmail.com


## Versioning

1.0.0.0


## Autor

* **Alexandre Machado da Silva Neto**: @alexandremsn (https://github.com/alexandremsn)
