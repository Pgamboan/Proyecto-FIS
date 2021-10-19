# Especifcación de requerimientos.

* RF001: La skill podrá encender y apagar de manera remota los dispositivos compatibles con el protocolo WoL.
  * (RNF): Al inicializarse la skill dará la bienvenida al usuario por medio de un mensaje predeterminado.
  * (RNF): A manera de “pop up” la skill emitirá un mensaje en el cual se avisará al usuario que solo podrá controlar dispositivos con una tarjeta de red compatible con el protocolo WoL. 
  * (RNF): La skill contará con un comando de voz que enlista a manera de ayuda un instructivo para utilizar el sistema. 
  * (RNF): El usuario podrá controlar la skill desde cualquier dispositivo con Alexa.

* RF002: La skill podrá automatizar el encendido y apagago de sus dispositivos compatibles con el protocolo WoL.
  * (RNF): Se podrán configurar diferentes horas y rutinas para ejecutar la funcionalidad de nuestra skill.

* RF003: La skill contará con una interfaz para introducir la dirección IP del dispositivo en cuestión.
  * (RNF):Se podrá acceder a esta herramienta por medio de un comando de voz que active el interfaz. 

* RF004: La skill contará con un interfaz externa en la que se podrá añadir la dirección MAC de la tarjeta de red de cada dispositivo.
  * (RNF): La skill solo podrá controlar dispositivos dentro de la misma red que el dispositivo Amazon Alexa.

* RF005: La skill tendrá un sistema para reconocer la compatibilidad de los dispositivos que se están configurando (computadores y TVs).
  * (RNF): El usuario podrá configurar sus dispositivos con el nombre que quiera.
  * (RNF): En caso de ser necesario la skill a manera de “pop up” emitirá un mensaje en el cual se avisará al usuario que el dispositivo que se está tratando de configurar no es compatible.
