# Especifcación de requerimientos.

* RF001: La skill podrá controlar de manera remota los dispositivos compatibles con el protocolo WoL a través de el asistente Alexa.
  * (RNF): El usuario podrá controlar la skill desde cualquier dispositivo con Alexa.
  * (RNF): El usuario podrá especificar el tipo de acción a realizar: Inicio, a

* RF002: La skill contará con una interfaz para introducir la dirección IP y MAC del dispositivo en cuestión.
  * (RNF): Se podrá acceder a esta herramienta por medio de un bot externo a la aplicación que active el interfaz. 
  * (RNF): Se tendra que añadir por separado la información de cada dispositivo a configurar.
  * (RNF): A manera de “pop up” la skill emitirá un mensaje en el cual se avisará al usuario que solo podrá controlar dispositivos con una tarjeta de red compatible con el  protocolo WoL. 

* RF003: Emplear la librera "AquilaWolLibrary" para ejecutar las funciones que ofrece la skill.
* (RNF): 
