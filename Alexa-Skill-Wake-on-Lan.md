# **ALEXA SKILL - WAKE ON LAN**
## Descripción de la aplicación:
### **OBJETIVO**
---
Implementar en Amazon Alexa, mediante la tienda de skills, el uso del protocolo WoL (Wake on LAN) para realizar el encendido y apagado remoto, de computadoras compatibles o televisores , de manera automática usando la voz. 

#### **ALCANCE DEL PROYECTO**

* Mundial, o en su defecto, personas que cuenten con dispositivos Alexa Echo.

#### **LIMITACIONES DEL PROYECTO**

* Conocimiento escaso de desarrollo
* Tiempo limitado
* La posibilidad de que los dispositivos no sean compatibles con el protocolo Wol
* Los dispostivos necesitan estar conectados a ethernet

### **USUARIOS**
---

Según las estadísticas de los altavoces inteligentes, Amazon Echo tuvo 40,6 millones de usuarios en 2020, más que Google Home y otros usuarios de altavoces inteligentes juntos.Instalar un Amazon Echo en tu casa significa que tendrás que utilizar la aplicación Alexa. Los usuarios de iPhone en el Reino Unido descargaron la aplicación más de 91.000 veces solo en febrero de 2020. Algunos de los principales aspectos del uso de Alexa son su disponibilidad, sus prácticas funciones y el uso de datos. 

* El 24% de los estadounidenses de entre 18 y 29 años tenía un Amazon Echo en 2018.
* Debido a su creciente popularidad, muchos usuarios de altavoces inteligentes se han interesado en probar Amazon Echo. Los altavoces inteligentes son más populares entre las generaciones más jóvenes.
* Según estadísticas de Amazon Alexa 2020, se vendieron 53,6 millones de altavoces Amazon Echo en el mismo año. Se espera que el número aumente a 65 millones en 2021.
* La demografía de los usuarios de Amazon Echo comenzó a cambiar en 2017 cuando más mujeres comenzaron a comprarlo. Más concretamente, el 50% de los ingresos procedieron de consumidoras en diciembre de 2017.Además, los Gen Xers y Baby Boomers han representado el 31% de las compras de Echo desde 2015.

### **CLIENTES**
---

* El 70% de los usuarios de altavoces inteligentes en USA utilizaron Echo en 2020.
* Según las recientes estadísticas de Amazon Echo, alrededor de 100.000 dispositivos domésticos inteligentes son compatibles con Alexa.
* Deben de contar con entrada ethernet para acceder a la tarjeta de red.

### **INNOVACIÓN/CREATIVIDAD**
---
Los asistentes virtuales no se crearon con el fin de satisfacer necesidades, se crearon para facilitarle la vida a los usuarios en tareas simples, como obtener información rápida, leer un libro o controlar la reproducción de música.

Ya hay una aplicación existente de Wake On Lan, pero la calidad de esta es muy baja y no cumple con su cometido. Esta skill tiene reseñas muy bajas, contando con una calificación de 2.5 estrellas entre más de 150 reseñas de usuarios, es una skill que no está ordenada ni claras sus instrucciones, llegando a fallar con su propósito principal, haciéndola una opción poco viable para la cantidad de usuarios que desearían tener esta skill funcional.

A parte de la anterior mencionada, no existe otra aplicación similar que aproveche la tecnología Wake on Lan, haciendo que si logramos hacer un sistema funcional, atractivo y eficiente, sería la aplicación principal de esta tecnología en el servicio de Amazon, Alexa. No se busca crear algo completamente nuevo, sino ofrecer una mejor alternativa a un producto ya existente.

Buscamos agilizar el encendido y apagado de las computadoras y laptops, utilizando la función de wake on lan que tienen los dispositivos, siendo compatible con la mayoría de los sistemas operativos tantos actuales como más antiguos (Windows xp, vista , 7), mediante el asistente virtual Alexa podemos iniciar esta función con un simple comando de voz, desde cualquier lugar mediante nuestro dispositivo móvil optimizando tiempos de espera para poder iniciar a usar la computadora.

## **REQUERIMIENTOS Y/O HISTORIAS DE USUARIO**

### **HISTORIAS DE USUARIO**

Las historias de usuario son una forma de buscar necesidades y preferencias que desean los usuarios y/o clientes a los que va dirigido nuestro proyecto, formulamos muchas de las que tenemos mediante reseñas de una skill parecida y testimonios de usuarios interesados. Decidimos hacerlas al igual que los requerimientos ya que es igual importante el feedback de la gente para un proyecto con constante mantenimiento.

* Como usuario de Alexa, quiero ser capaz de encender mi computadora desde el baño para poder aprovechar más mi tiempo.

* Como usuario de Alexa, quiero poder automatizar el encendido de mi computadora para ser más eficiente.

* Como usuario de Alexa, quiero automatizar el apagado de mi computadora para ahorrar tiempo en mi día a día.

* Como usuario de Alexa, quiero poder controlar varios dispositivos para tener un mayor control y conveniencia.

* Como usuario de Alexa, quiero programar un horario de encendido para que mis dispositivos estén acoplados a mi rutina y pueda aprovechar mi tiempo al máximo.

* Como usuario de Alexa, quiero ser capaz de personalizar el nombre a los dispositivos para que el control de ellos sea más fácil

* Como usuario de Alexa, quiero tener instrucciones para que me ayuden a poder implementar la skill.

* Como usuario de Alexa, quiero poder realizar preguntas para que me ayuden a resolver mis dudas

* Como usuario de Alexa, quiero poder controlar otros dispositivos como televisiones para tener un mayor control sobre todos mis dispositivos.

### **REQUERIMIENTOS FUNCIONALES Y NO FUNCIONALES**

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


### **MÉTODO DE PRIORIDAD**

Utilizamos el metodo MoSCoW para priorizar los requerimientos y las historias de usuario. Este metodo se integra muy bien a nuestro equipo y proyecto debido a la metodologia agil que utilizamos. La priorizacion que maneja MoSCoW se divide en 4 categorias:

* Must Have: Caracteristicas sin las cuales el proyecto no puede funcionar

* Should Have: Caracteristicas que son importantes en el proyecto, pero que no son indispensables

* Could Have: Caracteristicas que aumentarian el valor del proyecto si se tienen, pero que no son de gran importancia

* Won't have: Caracteristicas que no son importantes en el presente, pero que podrian implementarse mas tarde

Para que la priorizacion fuera lo mas eficiente posible, realizamos una sesion con el proyect owner para discutir en donde deberia ir cada una, basado en que tan factible es su implementacion. A continuacion se pueden apreciar los resultados de esa discusion:

### REQUIRIMIENTOS:
#### Must have:
* La skill podrá controlar el menu de opciones de encendido y apagado de los dispositivos compatibles con el protocolo WoL a través de el asistente Alexa.
* Solo los desarrolladores tienen acceso a la base de datos/plataforma.
* El usuario podrá controlar la skill desde cualquier dispositivo con Alexa.
* El usuario podrá especificar el tipo de acción a realizar: inicio, apagado, suspensión, reinicio e hibernar.
* El usuario tendrá que loguearse con su cuenta de Amazon para vincular sus datos con alexa.
#### Should have:
* Se contará con un tutorial para mostrarle a lo usuarios como inicializar la alexa skill dentro de sus dispositivos.
* Se usará un bot asistente para ayudar al usuario a introducir la dirección IP y MAC dentro de su base de datos.
#### Could have:
* El bot asistirá por medio de un tutorial, la manera en la que se deben ingresar las direcciones correspondientes.
* El tutorial se abrirá autómaticamente cuando el usuario indique las direcciones correspondientes dentro de la base de datos del bot.
* Se implementará los servicios de Microsoft Azure para hostear y manejar la base datos de la aplicación web donde se introducirán las direcciones IP/MAC de los dispositivos.
* La plataforma Azure notificará a los desarolladores de algún error con la aplicación.
#### Won't have but would like to in the future:
A manera de “pop up” el bot emitirá un mensaje en caso de ingresar alguna dirección IP/MAC erronea.
### HISTORIAS DE USUARIO:
#### Must have:
* Como usuario de Alexa, quiero poder automatizar el encendido/apagado de mi computadora para ser más eficiente.
* Como usuario de Alexa, quiero ser capaz de encender mi computadora desde otro sitio para poder aprovechar más mi tiempo.
#### Should have:
* Como usuario de Alexa, quiero poder controlar otros dispositivos como televisiones para tener un mayor control sobre todos mis dispositivos.
* Como usuario de Alexa, quiero tener instrucciones para que me ayuden a poder implementar la skill.
#### Could have:
* Como usuario de Alexa, quiero programar un horario de encendido para que mis dispositivos estén acoplados a mi rutina y pueda aprovechar mi tiempo al máximo.
* Como usuario de Alexa, quiero ser capaz de personalizar el nombre a los dispositivos para que el control de ellos sea más fácil.
* Como usuario de Alexa, quiero controlar varios dispositivos para tener un mayor control y conveniencia.
#### Won't have but would like to in the future:
* Como usuario de Alexa, quiero poder realizar preguntas dentro del área de comentarios de la skill que me ayuden a resolver mis dudas.


### **DIAGRAMA DE CASOS DE USO**

![Diagrama de casos de uso](Casos.png)

### **ARTEFACTOS UTILIZADOS POR EL EQUIPO DE DESARROLLO**
---

* [X] Formulario.
* [X] Diagrama de casos de uso.
* [X] Excepcinones de casos de uso.
* [X] Lluvia de ideas.

### **EXCEPCIONES DE CASOS DE USO**

1. Si el ususario quiere nombrar a 2 dispositvos de la misma forma, el sistema le avisará que ya existe un dispositivo con ese nombre

2. En el caso de que no pudiera conectarse con el dispositivo, la skill le notificará al usuario que hubo un error

3. Si el usuario le dice un nombre de dispositivo que no reconoce, el sistema le avisara al usuario que no existe ese dispositivo

4. En el caso de que el usuario introduzca una dirección IP y/o Mac erronea, el sistema le notificara que la conexión no fue exitosa

## **PROCESO DE DESARROLLO**
