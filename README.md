# Arduino 

## Concepto byte & PWM

### Byte

El byte es la unidad de información digital formada generalmente por ocho bits (serie de ceros y unos). Estos 8 bits permiten 256 combinaciones.  

![byte](../.vuepress/public/img/byte.png "Byte")  

El byte es la unidad que las computadoras utilizan para representar un caracter como una letra, un número y otros símbolos. El byte es la unidad de datos más pequeña con significado y la menor unidad de memoria. Es uno de los fundamentos del IDE de arduino (Integrated Development Environment o Entorno de Desarrollo Integrado) trabajaremos con bytes para controlar los pines PWM (pulse width modulation o modulación por ancho de pulso) que explicaremos más adelante. Otra relación con los bytes es que cada byte representa un carácter o una tecla o grupo de tecla.
  
    

![caracter](../.vuepress/public/img/Caracter.png "Caracter")

### PWM (puse with modulation)  

Para emular una señal analógica se cambia el ciclo de trabajo (el tiempo que permanece encendido y apagado de tal forma que el valor promedio de la señal sea el voltaje aproximado que se desea obtener, pudiendo entonces enviar hasta 256 voltajes diferentes entre 0 y 5 voltios.
  
    

![PWM](../.vuepress/public/img/PWM.gif "PWM")

## Concepto pin de Arduino

En arduino encontramos 3 tipos de pines.

### Digitales (entrada o salida)

Son en los que tenemos dos posibilidades 0 ó 5 voltios en arduino lo veremos como "low" o "high", como apagado o encendido

### PWM (salida)

Son los que podemos tener 256 voltajes diferentes entre 0 y 5 voltios.

### Analógico (entrada)

Son convertidores de señales analogicas en señales digitales a diferencia de PWM que utilizan 8 bits en analógico utilizamos 10 bits con lo que tenemos 1024 intervalos voltajes entre 0 y 5 voltios.

## Concepto sensor-actuador

### Sensores

Un sensor es un dispositivo con alguna propiedad eléctrica capaz de detectar magnitudes físicas o químicas, por ejemplo, la temperatura, una distancia, intensidad lumínica, aceleración, inclinación…
  
    
![Sensor](../.vuepress/public/img/sensores.png "Sensores")

En arduino se configuran siempre como entrada y nos proporciona información que procesaremos generalmente para dar una respuesta a un actuador/es.

En róbotica educativa se utilizan mucho los sensores de ultrasonidos (HC-SR04) para evitar obstáculos y los infrarrojos(TCRT5000) para seguir líneas. Otros muy utilizados en kits de iniciación son el de temperatura (TMP36), temperatura y humedad (DHT11) y fotoresistencia LDR.

### Actuadores

Por otro lado los actuadores son la respuesta al procesamiento de la programación transformando un valor digital o seudoanalógico (PWM) en un movimiento mecánico (motores, servos ...), la producción de sonido (buzzers)...

En arduino los programaremos junto con sensores para dar algún tipo de respuesta con la información que nos proporcionan, por ejemplo, con los sensores de ultrasonidos podríamos detectar un obstáculo y hacer que retroceda y gire robot para salvarlo.

En robótica educativa los que más solemos utilizar son los motores, los servos, buzzer y leds