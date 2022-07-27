Recebemos para este desfio uma base de dados em json, começamos importando a biblioteca pandas que vamos usar nesta limpeza
e na sequência importamos a base de dados que vamos usar

<img src="images/001.png">

Abaixo podemos ver o estado inicial do arquivo, ele continha diversos níveis de dicionários com especificações dos dados de cada coluna, primeiramente precisavamos desenpacotar estas informações

<img src="images/002.png">

usando o método nomalize, podemos desempacotar as informações e exporta-las em colunas individuais, como podemos ver na imagem abaixo, o mesmo método foi aplicado em todas as colunas que possuiam esta mesma característica.

<img src="images/003.png">
depois cada parte desenpacotada foi adicionada a base principal e as colunas mãe forma excluidas, ficando com um apécto melhor como podemos observar na imagem abaixo.

<img src="images/004.png">
Começamos a etapa de procurar por inconsitêcnias de dados, não localizamos valores vazios, tipo NaN ou Null.
depois verificamos que tinhamos ao invez de valores vazios ' ' simplesmente um espaço como valor. como podemos ver na imagem abaixo.

<img src="images/005.png">
 
 continuamos verificando valores e na coluna Senior, encontramos 0 e 1 ao invez de yes e no então corrigimos padronizando a base.

<img src="images/006.png">

 fizemos algumas checagens para verificar nas colunas com valores numéricos valores descrepantes ou negativos.
 mas não encontramos valores deste tipo.

<img src="images/007.png">

checamos qual o percentual do valor nulo, como o cliente informou que essa seria a variável alvo optamos por excluir as linhas pois elas representavam apenas perto de 3%

<img src="images/008.png">

verificamos que uma das variáveis numéricas estava com os valores armazenados como texto e convertemos o tipo para sanar esta inconsistência

<img src="images/009.png">

realizamos a tradução dos rótulos das colunas

<img src="images/010.png">

depois criamos a varíavel de gasto diário

<img src="images/011.png">

reordenadmos as colunas para que ficasse com a gradação gasto diario, mensal, total,
depois exportamos a base para ser usada futuramente.
