# Especifcación de requerimientos.

* RF001: La skill podrá controlar el menu de opciones de encendido y apagado de los dispositivos compatibles con el protocolo WoL a través de el asistente Alexa.
  * (RNF): El usuario podrá controlar la skill desde cualquier dispositivo con Alexa.
  * (RNF): El usuario podrá especificar el tipo de acción a realizar: inicio, apagado, suspensión, reinicio e hibernar.

* RF002: Se contará con una interfaz para introducir la dirección IP y MAC del dispositivo en cuestión.
  * (RNF): Se podrá acceder a la inferfaz por medio de un bot que asista en introducir las direcciones correspondientes. 
  * (RNF): El usuario tendra que añadir uno por uno las direcciones correspondientes dentro del bot.
  * (RNF): A manera de “pop up” el bot emitirá un mensaje en el cual se avisará al usuario que solo podrá controlar dispositivos con una tarjeta de red compatible con el  protocolo WoL. 

* RF003: Emplear la librera pública "AquilaWolLibrary" para ejecutar las funciones que ofrece la skill.

