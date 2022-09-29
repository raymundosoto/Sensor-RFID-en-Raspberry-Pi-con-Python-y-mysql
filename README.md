# Sensor-RFID-en-Raspberry-Pi-y-Python
Este repositorio contiene el material necesario para usar un sensor RFID MFRC522 en la raspberry pi 4 usando como lenguaje de programación Python la base de datos mysql

## Introducción
RFID es el acrónimo de «radio-frequency identification» (identificación por radiofrecuencia) y se refiere a una tecnología mediante la cual los datos digitales codificados en etiquetas RFID o etiquetas inteligentes son capturados por un lector RFID a través de ondas de radio.

Un sistema RFID pertenece a un grupo de tecnologías conocidas como Identificación Automática y Captura de Datos (AIDC). Los métodos AIDC identifican automáticamente los objetos, recopilan datos sobre ellos e introducen esos datos directamente en los sistemas informáticos sin necesidad de intervención humana.

Los sistemas RFID constan de tres componentes: una etiqueta RFID o etiqueta inteligente, un lector RFID y una antena RFID. Las etiquetas RFID contienen un circuito integrado y una antena, que se utilizan para transmitir datos al lector RFID. El lector entonces convierte las ondas de radio en una forma de datos más utilizable. La información recogida de las etiquetas se transfiere a través de una interfaz de comunicaciones a un sistema informático principal, donde la información puede ser almacenada en una base de datos y analizada posteriormente.

Las etiquetas RFID tienen una gran variedad de formas y tamaños. Las más comunes son las etiquetas pasivas y las activas. Las etiquetas RFID pasivas son las más utilizadas, ya que son más pequeñas y menos costosas de implementar. Las etiquetas pasivas están «alimentadas» por el lector RFID antes de que puedan transmitir datos. A diferencia de las etiquetas pasivas, las etiquetas RFID activas tienen una fuente de alimentación integrada (por ejemplo, una batería), lo que les permite transmitir datos en todo momento.
Etiquetas RFID Pasivas

Las etiquetas pasivas se componen de tres elementos: un circuito integrado o chip, una antena y un soporte.
El Chip

El chip RFID almacena datos y realiza tareas específicas. Dependiendo de su diseño, el chip puede ser sólo de lectura, de una sola escritura, de lectura múltiple o de lectura y escritura . Normalmente, los chips RFID transportan 96 bits de memoria, pero pueden oscilar entre 2 y 1000 bits.
La Antena

Conectado al chip está el segundo componente, la antena, cuyo propósito es absorber las ondas de radiofrecuencia de la señal del lector y enviar y recibir datos. El rendimiento pasivo de las etiquetas RFID depende en gran medida del tamaño de la antena: cuanto más grande sea la antena, más energía podrá recoger y luego devolver. Las antenas más grandes, por lo tanto, tienen rangos de lectura mayores (aunque no tan altos como los de las etiquetas activas).

La forma de la antena también es importante para el rendimiento de la etiqueta. Las antenas de baja y alta frecuencia (LF y HF, respectivamente) son generalmente bobinas porque estas frecuencias son predominantemente magnéticas. Las antenas de frecuencia UHF, por otro lado, se parecen a las antenas de TV antiguas porque las frecuencias ultrahigh son solamente eléctricas en el medio.
El Soporte

El tercer componente de una etiqueta RFID pasiva se denomina soporte, que suele ser de plástico. Tanto la antena como el chip están unidos al sustrato, que puede considerarse como el «pegamento» que mantiene unidas todas las piezas de la etiqueta.
Etiquetas RFID Activas

Al igual que las etiquetas RFID pasivas, las etiquetas activas tienen un microchip y una antena. Los chips, sin embargo, suelen ser de mayor tamaño y tienen mayores capacidades que los chips RFID de las etiquetas pasivas.

Las etiquetas activas tienen dos componentes adicionales que las diferencian de las etiquetas pasivas: una fuente de alimentación incorporada y una parte electrónica incorporada.
La Fuente de Alimentación Incorporada

La fuente de alimentación suele ser una batería, aunque también puede ser solar. La fuente de alimentación incorporada permite que la etiqueta transmita datos a un lector por sí sola, sin necesidad de extraer energía del propio lector como lo hacen las etiquetas pasivas. Además, las etiquetas activas se pueden leer desde distancias de 30 metros o más, mientras que las etiquetas pasivas sólo se pueden leer desde una distancia de hasta 7 metros. 

## Material necesario

- Raspberry pi 4
- Sensor MFRC522
- Protoboard
- Cable de conexi+on de raspberry pi de 20 pines
- Cables jumper
- Un led
- En la raspeberry habilitar en protocolo de conexión SPI
## Software necesario

Software para lectura del tag RFID
- Python 3.9
- Biblioteca mfrc522
  sudo pip3 install mfrc522
 - [Código de lectura básica del sensor](https://github.com/raymundosoto/Sensor-RFID-en-Raspberry-Pi-con-Python-y-mysql/blob/main/codigo_lectura_basica.py)
 - [Código de escritura de texto en el sensor](https://github.com/raymundosoto/Sensor-RFID-en-Raspberry-Pi-con-Python-y-mysql/blob/main/script_escritura.py)

## Esquema de conexión

Realiza las siguientes conexiones

![imagen](https://user-images.githubusercontent.com/72757419/193123436-4b4d51b5-e0c8-4c2d-acab-58bf5fdc1aea.png)

El circuito final debe quedar de la siguiente forma

![imagen](https://user-images.githubusercontent.com/72757419/193123940-c8ac2846-1aff-4a7a-bd12-325ef62550d3.png)

## Salidas en terminal del funcionamiento del RFID

### Ejemplo de lectura 

![imagen](https://user-images.githubusercontent.com/72757419/193126420-17508cd2-be39-4cbc-a3d6-ad20c4452dae.png)

### Ejemplo de escritura

![imagen](https://user-images.githubusercontent.com/72757419/193126636-35c79045-531a-435a-951e-65068fec19c1.png)





