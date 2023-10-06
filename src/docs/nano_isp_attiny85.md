# Guía para usar Arduino Nano como ISP para programar ATtiny85

En esta guía, aprenderás cómo utilizar un Arduino Nano como programador ISP (In-System Programmer) para programar un ATtiny85. Este proceso te permitirá cargar programas en un ATtiny85 utilizando el Arduino Nano como un programador ISP.

## Requisitos

Antes de comenzar, asegúrate de tener los siguientes elementos:

1. Arduino Nano.
2. ATtiny85 microcontrolador.
3. Cables de conexión.
4. Software Arduino IDE instalado en tu computadora.
5. Librería "ArduinoISP" instalada en tu Arduino Nano. Puedes instalarla desde el menú "Herramientas" -> "Gestor de tarjetas" en el Arduino IDE.

## Conexión Hardware

Sigue estos pasos para conectar tu Arduino Nano al ATtiny85:

1. Conecta el Arduino Nano a tu computadora mediante un cable USB.
2. Conecta los pines de la siguiente manera:

|Arduino Nano | label | ATtiny85 | label |
|PIN 10       | SS    | PIN 1    | RESET |
|PIN 11       | MOSI  | PIN 5    | MOSI  |
|PIN 12       | MISO  | PIN 6    | MISO  |
|PIN 13       | SCK   | PIN 7    | SCK   |


![Conexiones](ruta_a_tu_imagen1.png)

## Programación del Arduino Nano como ISP

Sigue estos pasos para cargar el programa "ArduinoISP" en tu Arduino Nano:

1. Abre el Arduino IDE.
2. Selecciona "Archivo" -> "Ejemplos" -> "ArduinoISP" para abrir el código de ejemplo.
3. Verifica que la tarjeta seleccionada sea "Arduino Nano" y el puerto USB correcto esté seleccionado.
4. Carga el código en tu Arduino Nano haciendo clic en el botón "Subir".

![Cargar ArduinoISP](ruta_a_tu_imagen2.png)

## Programación del ATtiny85

Ahora que has programado tu Arduino Nano como ISP, puedes utilizarlo para programar el ATtiny85:

1. Conecta el ATtiny85 a las conexiones mencionadas anteriormente.
2. En el Arduino IDE, selecciona "Herramientas" -> "Programador" -> "Arduino as ISP".
3. Abre o crea tu proyecto para el ATtiny85 en el Arduino IDE.
4. Selecciona "Herramientas" -> "Placa" -> "ATtiny85".
5. Selecciona "Herramientas" -> "Procesador" -> "ATtiny85".
6. Carga tu programa en el ATtiny85 haciendo clic en el botón "Subir".

¡Eso es todo! Tu Arduino Nano actuará como un programador ISP para cargar programas en el ATtiny85. Asegúrate de que las conexiones estén correctamente establecidas antes de cargar el programa en el ATtiny85.

![Programar ATtiny85](ruta_a_tu_imagen3.png)

¡Ahora estás listo para programar tu ATtiny85 utilizando tu Arduino Nano como programador ISP!