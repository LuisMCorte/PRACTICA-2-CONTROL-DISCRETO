# PRACTICA-2-CONTROL-DISCRETO

Corte Luis
Misacango Bryam

En este repositorio se presenta la implementación de dos sistemas basados en la placa Controllino: un control de LEDs mediante botones y un sistema de semáforo utilizando una máquina de estados finitos (FSM). En la Parte A, se describe el control de una secuencia de LEDs activada por tres botones, empleando variables predefinidas de la librería Controllino.h, punteros y enums. En la Parte B, se detalla un sistema de semáforo con dos conjuntos de luces, implementado con una FSM, enums, estructuras y retardos no bloqueantes. Se incluye un diagrama de estados y los códigos desarrollados como anexos.


Parte A: Control de LED por dos botones

El sistema controla una secuencia de nueve LEDs conectados a los pines de la placa Controllino, utilizando tres botones para alternar entre tres modos: normal, inverso y reinicio. En el modo normal, los LEDs se encienden secuencialmente desde el primero CONTROLLINO_D0 hasta el último CONTROLLINO_D7 con un intervalo de 500 ms. En el modo inverso, la secuencia se invierte, comenzando desde el último LED. El modoreinicio enciende todos los LEDs brevemente, los apaga, y retorna al modo previo normal o inverso. La implementación utiliza una máquina de estados finitos (FSM) basada en un enum para gestionar los modos, con temporización no bloqueante mediante millis().


Parte B: Parte B: Reto de control de semáforo con FSM
El sistema de semáforo utiliza una máquina de estados finitos con cinco estados. Los estados son: Inicial (ambos semáforos en rojo), Verde A (semáforo A en verde, B en rojo), Amarillo A (A en amarillo, B en rojo), Verde B (A en rojo, B en verde) y Amarillo B (A en rojo, B en amarillo).A continuación se muestra el diagrama de estados de manera grafica.

![image](https://github.com/user-attachments/assets/99d08508-26bd-4c2a-9c47-e5d1a0ba39e9)

