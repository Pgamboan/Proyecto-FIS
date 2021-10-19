# Especifcación de requerimientos.

* RF001: La skill podrá controlar el menu de opciones de encendido y apagado de los dispositivos compatibles con el protocolo WoL a través de el asistente Alexa.
* (RNF): El usuario podrá controlar la skill desde cualquier dispositivo con Alexa.
* (RNF): El usuario podrá especificar el tipo de acción a realizar: inicio, apagado, suspensión, reinicio e hibernar.

* RF002: Se implementará los servicios de Microsoft Azure para hostear y manejar la base datos de la aplicación web donde se introducirán las direcciones IP/MAC de los dispositivos.
* (RNF): La plataforma Azure le notificará a los desarolladores de algún error con la aplicación.
* (RNF): Solo los desarrolladores tienen acceso a la base de datos/plataforma.
* (RNF): El usuario tendrá que loguearse con su cuenta de Amazon para vincular sus datos con alexa.

* RF003: Se usará un bot asistente para ayudar al usuario a introducir la dirección IP y MAC dentro de su base de datos.
* (RNF): El bot asistirá por medio de un tutorial, la manera en la que se deben ingresar las direcciones correspondientes. 
* (RNF): A manera de “pop up” el bot emitirá un mensaje en caso de ingresar alguna dirección IP/MAC erronea. 

* RF004: Se contará con un tutorial para mostrarle a lo usuarios como inicializar la alexa skill dentro de sus dispositivos.
* (RNF): El tutorial se abrirá autómaticamente cuando el usuario indique las direcciones correspondientes dentro de la base de datos del bot.


