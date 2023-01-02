# Processamento de Imagem e Visão Computacional 

  é uma disciplina fornecidade pelo Centro de Engenharia Elétrica e Informática ao curso de Engenharia elétrica. Disciplina que dedica a apresentação de algoritmos para processamento de imagens. O intuito que tenho com essa cadeira é obter conhecimento básico para **processamento de sinais** de maneira geral. Nessa disciplina o sinal trabalhado é apenas a imagem.


##  Objetivo Principal

  O repositório tem como objetivo ajudar com o entendimento dos algoritmos utilizados em **processamento de imagem e visão computacional**. Os algoritmos apresentados aqui serão construidos do zero e comentados com o intuito de que se possa entender como o algoritmo foi aplicado a imagem foi construido e funciona.

##  Objetivo Secundário
  Como estudante de Engenharia, deve-se levara serio uma das seguintes características do enegenheiro: capacidade de analisar e solucionar problemas. construir os algoritmos de processamento de imagem do zero é um desafio para aprimorar minha capacidade de analisar o problema e solucionar com as ferramentas minimas disponíveis.
  
 
***

serão apresentados os algoritmos dos seguintes filtros ja desenvolvidos:

1. Fltro Convolucional
*
*
...

# 1. Filtro Convolucional
consiste na aplicação da operação de convolução para obter um novo resultado para a imagem. haverá uma imagem e um filtro que transformará as características da imagem. observe o seguinte exemplo:

<div align = "center">
<img src = "https://github.com/JWchester/Processamento-de-Imagem/blob/main/Convolu%C3%A7%C3%A3o%20em%20Uma%20Imagem(Forma%20Anal%C3%ADtica).png" width = 1000px /> </div> 


o centro do filtro(matriz que irá sobrepor a imagem) será posicionado em todos os pixels da imagem. os pixels que serão captados pelo filtro serão multiplicados e somados para resultar na transdormação de um único pixel. dessa forma, a cada iteração do filtro sobre a imagem será obtido a transformação do pixel daquele posição. Observe os passos de uma convolução entre uma imagem e um filtro genéricos:

<div align = "center">
<img align = "center" src = "https://github.com/JWchester/Processamento-de-Imagem/blob/main/conv1.png" width = 1000px /> 
<img align = "center" src = "https://github.com/JWchester/Processamento-de-Imagem/blob/main/conv2.png" width = 1000px /> 
<img align = "center" src = "https://github.com/JWchester/Processamento-de-Imagem/blob/main/conv3.png" width = 1000px />  
<img align = "center" src = "https://github.com/JWchester/Processamento-de-Imagem/blob/main/conv4.png" width = 1000px /> </div>

***

A operação continua até passar por todos os pixels da imagem. baseado nisso, tem-se o filtro convolucional.
para utilizar o filtro convolucional será utilizado o filtro blur que consiste em uma matriz de 1´s onde cada posição é multiplicada por $\ \huge{ 1 \over {Elementos}}$. a matriz de convolução dever ser quadrada e composta  por dimensões impares acima maiores ou iguais a 3. observe o exemplo: 


<div align = "center">
<img align = "center" src = "https://github.com/JWchester/Processamento-de-Imagem/blob/main/Filtro%20blur(3x3%20e%205x5).png" width = 700px /> </div> 


