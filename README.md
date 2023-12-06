<h1> Parcial Arduino </h1>

![image_text](https://github.com/LucianoBardallo/Parcial-Arguino/blob/main/img/ArduinoTinkercad.jpg?raw=true)

<h3> Integrantes </h3>

- Luciano Bardallo

<h3> Proyecto Parcial </h3>

![image_text](https://github.com/LucianoBardallo/Parcial-Arguino/blob/main/img/Parcial%20Arduino%20PT3.png?raw=true)

<h3> Descripcion </h3>

- Suma y resta de numeros mostrados en dos 7 segmentos y conectados con botones
- Cambio de modo con un swtich (Numeros normales y Numeros primos)
- Motor de afisionado que funciona en una direccion u otra dependiendo el boton presionado
- Sensor de fuerza que cambia el tiempo de delay dependiendo de su valor
- Sensor de luz que muestra algo en el monitor serial dependiendo de su valor y cual boton se presiona
 

<h3> Funcion Principal </h3>

Esta funcion se encarga de encender y apagar los display dependiendo del numero que se le inserte.

prenderDisplay y printNum son 2 importantes partes del proyecto que se encargan de hacer funcionar los display, uno se encarga de saber que display se tiene que prender y el otro que numero se va a ver en dicho display.

````
void imprimirCuenta(int num)
{
  prenderDisplay(APAGADO);
  printNum(num/10);
  prenderDisplay(UNIDAD);
  delay(50);
  prenderDisplay(APAGADO);
  printNum(num - 10*((int)num/10));
  prenderDisplay(DECENA);
  delay(50);
}

````

<h3> Link del proyecto </h3>

https://www.tinkercad.com/things/2krpvcpMDTp-parcial-arduino-pt3/editel?returnTo=%2Fdashboard%3Ftype%3Dcircuits%26collection%3Ddesigns&sharecode=_vNSzYql4ZAnRe9fWm14ci_250Q3tIYyi8gOyxexC3g
