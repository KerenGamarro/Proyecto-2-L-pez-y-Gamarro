# Proyecto-2-López-y-Gamarro
Proyecto 2 – Comunicación Serial Utilizando los microcontroladores ESP32 y NUCLEO-F446RE
Con este proyecto se busca que el estudiante experimente y aplique los conocimientos adquiridos del curso integrando un sistema de comunicación entre un ESP32, una
NUCLEO-F446RE y una computadora.
# Parte 1 Comunicación UART.
La Nucleo debe comunicarse con una computadora utilizando comunicación UART, estocon el objetivo de desplegar un menú de opciones en una terminal serial y así enviarle
instrucciones a la Nucleo. El menú debe contener las siguientes opciones:
1. Controlar dispositivo SPI
2. Obtener medición de Sensor I2C

# Parte 2 Comunicación SPI.
En esta parte se simulará un dispositivo con protocolo de comunicación SPI utilizando el ESP32 y 3 LEDs. El comando que se enviará al dispositivo servirá para controlar el tiempo de encendido de los LEDs. Cuando el usuario seleccione la opción 1 del menú principal, se deberá mostrar un sub- menú en el que se solicite un comando de control para el dispositivo, el comando debe contener el LED a encender y el tiempo en milisegundos que deber permanecer encendido (Ej: “1,500” -> encender LED1 por 500ms). Luego de que el usuario ingrese el comando en la terminal, este debe enviarse por SPI al ESP32 para ser ejecutado. Al terminar la ejecución del comando, mostrar nuevamente el menú.

# Parte 3 Comunicación I2C.
En esta parte se simulara un sensor con protocolo de comunicación I2C utilizando el ESP32 y un potenciometro. Cuando el usuario seleccione la opción 2 del menú principal, la Nucleo deberá solicitarle el valor del potenciometro al ESP32 por medio de la comunicación I2C, el ESP32 deberá realizar una medición del canal analógico y devolver el valor capturado. Luego de que la Nucleo reciba ese valor, desplegarlo en la terminal serial y volver a desplegar el menú.

# Parte 4 Pantalla LCD.
En esta, utilizando una pantalla LCD Hitachi 16x2, se desplegará lo siguiente:
- El valor del potenciómetro en voltios
- El valor del potenciómetro en bits
- La iniciar del color del último LED que se encendió
Importante: La verificación de los datos ingresados en la terminal debe hacerse en la Nucleo.
