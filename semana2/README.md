<div align="center">
<img src="images/clipart571406.png" width=100>

# Desafio Alura Data Science Semana 1 Limpeza de dados
<div align="left">
Limpeza de uma base de dados e exportação para arquivo .csv para realizar análises e plotagens na semana seguinte.

## Tecnologia

O software  usado neste projeto foi:

* Python version  3.9.5

## Serviços Usados

* Github


## Bibliotecas Python

* Pandas


## Como foi feito

Será descrito abaixo através de textos e imagens.


Recebemos para este desfio uma base de dados em json, começamos importando a biblioteca pandas que vamos usar nesta limpeza
e na sequência importamos a base de dados que vamos usar

<img src="images/001.png">

Abaixo podemos ver o estado inicial do arquivo, ele continha diversos níveis de dicionários com especificações dos dados de cada coluna, primeiramente precisávamos desempacotar estas informações

<img src="images/002.png">

Usando o método nomalize, podemos desempacotar as informações e exportá-las em colunas individuais, como podemos ver na imagem abaixo, o mesmo método foi aplicado em todas as colunas que possuíam esta mesma característica.

<img src="images/003.png">
Depois cada parte desempacotada foi adicionada a base principal e as colunas mãe forma excluídas, ficando com um aspecto melhor como podemos observar na imagem abaixo.

<img src="images/004.png">
Começamos a etapa de procurar por inconsistências de dados, não localizamos valores vazios, tipo NaN ou Null.
depois verificamos que tínhamos ao invés de valores vazios ' ' simplesmente um espaço como valor. como podemos ver na imagem abaixo.

<img src="images/005.png">
 
 Continuamos verificando valores e na coluna Senior, encontramos 0 e 1 em vez de yes e no então corrigimos padronizando a base.

<img src="images/006.png">

 Fizemos algumas checagens para verificar nas colunas com valores numéricos valores discrepantes ou negativos.
 mas não encontramos valores deste tipo.

<img src="images/007.png">

Checamos qual o percentual do valor nulo, como o cliente informou que essa seria a variável alvo optamos por excluir as linhas pois elas representavam apenas perto de 3%

<img src="images/008.png">

Verificamos que uma das variáveis numéricas estava com os valores armazenados como texto e convertemos o tipo para sanar esta inconsistência

<img src="images/009.png">

Realizamos a tradução dos rótulos das colunas

<img src="images/010.png">

Depois criamos a variável de gasto diário

<img src="images/011.png">

Reordenamos as colunas para que ficasse com a gradação gasto diário, mensal, total,
depois exportamos a base para ser usada futuramente.



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
