# HC-SR04-Ultrasonic-Distance-Sensor

![]('https://img.dxcdn.com/newprdimgs/20201222/11addabbf77d0d9ff7757832f45a25fb.jpg')
![Sensor HC-SR04](https://github.com/rick1660/Sensor-HC-SR04-Ultrasonic-Distance-Sensor/blob/main/senseor2.jpg)

## Como trabaja el Sensor HC-SR04

### Los sensores ultrasónicos usan sonido para determinar la distancia entre el sensor y el objeto más cercano en su camino. ¿Cómo hacen esto los sensores ultrasónicos? Los sensores ultrasónicos son esencialmente sensores de sonido, pero operan a una frecuencia por encima del oído humano. El sensor HC-SR04 esta compuesto por un emisor y un receptor de ultrasonidos. Estos nos ayuda a medir la distancia a la que se encuentra un objeto justo frente a el, enviando un pulso de ultrasonidos y midiendo el tiempo que transcurre hasta que vuelve dicho pulso.

![Sensor HC-SR04](https://github.com/rick1660/Sensor-HC-SR04-Ultrasonic-Distance-Sensor/blob/main/diagrama1.jpg)

## Descripcion de los pines del sensor

| Nombre del Pin |                Descripcion              |
| ---------------| ----------------------------------------|
|Vcc             | Pin de alimentacion. (5v)               |
|Trigger         | Pin de disparo, este pin es una entrada | 
|Echo            | Este pin es una salida del sensor       |
|Gnd             | Pin negativo de alimentacion            |


## Caracteristicas electricas

| Nombre del Pin        |                Descripcion              |
| ----------------------| ----------------------------------------|
|Voltaje de trabajo     | 5v                                      |
|Corriente de trabajo   | 15mA                                    | 
|Frecuencia de trabajo  | 40KHz                                   |
|Rango de funcionamiento| 2 a 500 cm                              |
|Ángulo de detección    | 15 a 20 grados                          |

## Funcionamiento y Diagrama de temporización

### En el diagrama de temporización se aprecia como solo es necesario aplicar un pulso de 10uS en el pin trigger para comenzar con la medición. A continuación el sensor envía una serie de 8 pulsos de 40KHz y pone el pin de Echo a nivel alto. El pin Echo permanecerá a nivel alto hasta que se reciba el eco de los pulsos de 40KHz. Para saber a la distancia a la que se encuentra el objeto, solo hay que medir el tiempo al que está el pin Echo a nivel alto y aplicar la siguiente formula. 

### Centimetros = uS*0,01715

![Diagrama](https://github.com/rick1660/Sensor-HC-SR04-Ultrasonic-Distance-Sensor/blob/main/diagrama2.png)



                                          



