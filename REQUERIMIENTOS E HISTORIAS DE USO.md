### **REQUERIMIENTOS E HISTORIAS DE USUARIO**
---
#### **MÉTODO DE PRIORIDAD**
---

Utilizamos el metodo MoSCoW para priorizar los requerimientos y las historias de usuario. Este metodo se integra muy bien a nuestro equipo y proyecto debido a la metodologia agil que utilizamos. La priorizacion que maneja MoSCoW se divide en 4 categorias:

* Must Have: Caracteristicas sin las cuales el proyecto no puede funcionar

* Should Have: Caracteristicas que son importantes en el proyecto, pero que no son indispensables

* Could Have: Caracteristicas que aumentarian el valor del proyecto si se tienen, pero que no son de gran importancia

* Won't have: Caracteristicas que no son importantes en el presente, pero que podrian implementarse mas tarde

Para que la priorizacion fuera lo mas eficiente posible, realizamos una sesion con el proyect owner para discutir en donde deberia ir cada una, basado en que tan factible es su implementacion. A continuacion se pueden apreciar los resultados de esa discusion:

<br>

#### **HISTORIAS DE USUARIO**
Las historias de usuario son una forma de buscar necesidades y preferencias que desean los usuarios y/o clientes a los que va dirigido nuestro proyecto, formulamos muchas de las que tenemos mediante reseñas de una skill parecida y testimonios de usuarios interesados. Decidimos hacerlas al igual que los requerimientos ya que es igual importante el feedback de la gente para un proyecto con constante mantenimiento.

* HU001: Como usuario de Alexa, quiero poder automatizar el encendido/apagado de mi computadora para ser más eficiente. **(M)**
* HU002: Como usuario de Alexa, quiero ser capaz de encender mi computadora desde otro sitio para poder aprovechar más mi tiempo. **(M)**
* HU003: Como usuario de Alexa, quiero poder controlar otros dispositivos como televisiones para tener un mayor control sobre todos mis dispositivos. **(S)**
* HU004: Como usuario de Alexa, quiero tener instrucciones para que me ayuden a poder implementar la skill.  **(S)**
* HU005: Como usuario de Alexa, quiero programar un horario de encendido para que mis dispositivos estén complados a mi rutina y pueda aprovechar mi tiempo al máximo. **(C)**
* HU006: Como usuario de Alexa, quiero ser capaz de personalizar el nombre a los dispositivos para que el control de ellos sea más fácil.**(C)**
* HU007: Como usuario de Alexa, quiero controlar varios dispositivos para tener un mayor control y conveniencia.**(C)**
* HU008: Como usuario de Alexa, quiero poder realizar preguntas dentro del área de comentarios de la skill que me ayuden a resolver mis dudas. **(W)**

#### **ESPECIFICACIÓN DE REQUERIMIENTOS**

Los requerimientos son un instrumento fundamental en el correcto desarrollo de un proyecto de software. Son de gran ayuda, tanto para el cliente como el equipo de desarrollo, para tener una visión concisa de que características se requiere que tenga el producto y como estas se relacionan con el usuario.

Debido a la simpleza que representa la ejecución de nuestro producto, no hay una gran cantidad de requerimientos que podamos idear, pero los hicimos de manera que cumplan con las caracteristicas principales de un requisito. Tras un extendido proceso de discusión, elaboración y verificación, hemos concordado en los siguientes requisitos para nuestro proyecto:

* RF001: La skill podrá controlar el menu de opciones de encendido y apagado de los dispositivos compatibles con el protocolo WoL a través de el asistente Alexa. (HU001, HU002, HU003, HU005) **(M)**

   * (RNF001): El usuario podrá controlar la skill desde cualquier dispositivo con Alexa. **(M)**

   * (RNF002): El usuario podrá especificar el tipo de acción a realizar: inicio, apagado, suspensión, reinicio e hibernar. **(M)**

* RF002: Se implementará los servicios de Microsoft Azure para hostear y manejar la base datos de la aplicación web donde se introducirán las direcciones IP/MAC de los dispositivos. (HU006, HU007) **(C)**

   * (RNF003): La plataforma Azure le notificará a los desarolladores de algún error con la aplicación. **(C)**

   * (RNF004): Solo los desarrolladores tienen acceso a la base de datos/plataforma. **(M)**

   * (RNF005): El usuario tendrá que loguearse con su cuenta de Amazon para vincular sus datos con alexa. **(M)**

* RF003: Se usará un bot asistente para ayudar al usuario a introducir la dirección IP y MAC dentro de su base de datos. (HU007) **(S)**

   * (RNF006): El bot asistirá por medio de un tutorial, la manera en la que se deben ingresar las direcciones correspondientes. **(C)**

   * (RNF007): A manera de “pop up” el bot emitirá un mensaje en caso de ingresar alguna dirección IP/MAC erronea. **(W)**

* RF004: Se contará con un tutorial para mostrarle a lo usuarios como inicializar la alexa skill dentro de sus dispositivos. (HU004, HU008) **(S)**

   * (RNF008): El tutorial se abrirá autómaticamente cuando el usuario indique las direcciones correspondientes dentro de la base de datos del bot. **(C)**

<br>
