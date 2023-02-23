# Remote Virus Disinfection System
Esta guía contiene el código de configuración de un sistema de desinfección remoto. 

![diagrama](https://github.com/faviles7/disinfection_system/blob/main/diagrama_ds.jpg)

## Configuración del arduino (sensores y actuadores).
*Revisar el archivo arduino

La automatización de la cabina se realiza y controla con el arduino UNO. A continuación, se detallan los pines utilizados y su respectiva función: 
- Pin 8: Entrada señal del sensor de presencia 
- Pin 0: rx lcd módulo i2c SCL 
- Pin 1: tx lcd módulo i2c SDA 
- Pin 7: Activación del relé de la bomba de agua 
- Pin 9: rx señal de activación del ESP 8266 
- Pin 12 y 13: Señalización led
## Configuración del ESP8266 (control inalámbrico).
*Revisar el archivo esp8266

La tarjeta inalámbrica NodeMCU basada en ESP8266 es la encargada de establecer la comunicación entre el sistema de desinfección y un dispositivo móvil.

A continuación, se detallan los pines utilizados y su respectiva función: 
- Pin 15: conexión del relé de alimentación de la placa ESP 8266 
- Pin 21: conexión del relé de alimentación del arduino 
- Pin 18 y 19: Tx y Rx de datos
