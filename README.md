# Projeto da Fonte de Tensão

## Objetivos

Projetar uma fonte de tensão ajustável que varie de 3V a 12V e que suporte uma corrente de pelo menos 100mA.

**Aluno:** Thales Darini Souza - 10747562

## Circuito no Falstad
**[Link do circuito no Falstad](http://tinyurl.com/y722ua49)**

**[Link do vídeo explicativo](https://youtu.be/_xOmkor7MkY)**

![Circuito no Falstad](circuit_falstad.png)

## Componentes utilizados

|Nome|Especificações|Descrição|Preço|
|---|---|---|---|
|Transformador|12V+12V 300mA|Utilizado para converter a tensão da tomada de 127V AC para 24V AC. Com esses 24V de pico é possível garantir que o zener fique constantemente ligado, considerando as quedas de tensão e ainda com uma boa margem de segurança.|[R$ 16,45](https://www.baudaeletronica.com.br/transformador-trafo-12v-12v-300ma-110-220vac.html)|
|Diodos|1N4001|Utilizados para formar a ponte de diodos a fim de aproveitar ambos os ciclos negativo e positivo da corrente alternada. Juntamente com o capacitor, a ponte retificadora é responsável por transformar a tensão de AC para CC e retificá-la.|[4x R$ 0,14 = R$ 0,56](https://www.baudaeletronica.com.br/diodo-1n4001.html)| 
|Diodo Zener|BZX55C 13V|A função deste zener será manter uma tensão constante de 13V entre seus polos, que, com a ajuda de um potenciômetro, poderá ser ajustada no intervalo de 3V a 12V para a carga, como desejado.|[R$ 0,09](https://www.baudaeletronica.com.br/diodo-zener-bzx55c-13v-0-5w.html)|
|Capacitor Eletrolítico|330uF 35V|O capacitor armazena energia ao longo de cada oscilação para garantir que sempre seja fornecida energia ao restante do circuito. Foi escolhido o de 330uF para a tensão de ~24V provinda do transformador por ser suficiente para manter o zener ligado o tempo todo sem oscilações.|[R$ 0,34](https://www.baudaeletronica.com.br/capacitor-eletrolitico-330uf-35v.html)|
|Potenciômetro|10K|É com o potenciômetro que ajustamos a tensão final fornecida à carga, variando de 3V a 12V.|[R$ 1,46](https://www.baudaeletronica.com.br/potenciometro-linear-de-10k-10000.html)|
|Resistor|2K2 (1/4W)|Este resistor regula a corrente que passa pelo zener, mantendo-a abaixo de 5mA.|[R$ 0,08](https://www.baudaeletronica.com.br/resistor-2k2-5-1-4w.html)|
|Resistor|5K6 (1/4W)|A função deste resistor é limitar a tensão mínima fornecida à carga em 3V quando o potênciometro está no seu limite inferior.|[R$ 0,08](https://www.baudaeletronica.com.br/resistor-5k6-5-1-4w.html)|
|Resistor|560R (1/4W)|Usado para ligar o LED difuso no final do circuito. Especificação do fabricante para uma tensão de 12V.|[R$ 0,08](https://www.baudaeletronica.com.br/resistor-560r-5-1-4w.html)|
|LED difuso|3mm verde|Conectado ao fim do circuito para indicar que a fonte está ligada. Além disso, a intensidade de seu brilho é diretamente proporcional à tensão que passa pela carga, que varia de 3V a 12V.|[R$ 0,24](https://www.baudaeletronica.com.br/led-difuso-3mm-verde.html)|
|Transistor NPN|BC635|Este transistor é usado para manter a tensão desejada de até 12V na carga a partir da tensão provinda do zener e do potenciômetro e, ao mesmo tempo, permitir a passagem da corrente desejada de 100mA.|[R$ 0,33](https://www.baudaeletronica.com.br/transistor-npn-bc635.html)|
|**Total**|||**R$ 19,71**|

## Esquemático no Eagle 

![Esquemático no Eagle](esquematico_eagle.png)

## PCB no Eagle

![PCB Eagle](PCB_eagle.png)


