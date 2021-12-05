# Introducción // Justificación del proyecto

Somos el equipo de Alexa Wake On LAN. Actualmente la tecnología ha evolucionado a un paso muy grande durante la vida del ser humano, no es de pensar que hasta hace menos de un siglo el internet fue concebido y consigo una nueva forma de vida y automatización. Por ello como equipo buscábamos una manera de contribuir con la automatización y agilizar procesos cotidianos. Así mismo consideramos a la situación pandémica que nos rige y a la virtualización de muchos procesos comunes dentro del área social (trabajo, escuela, documentación, etc.). Gracias a esto nació la idea de realizar una “habilidad” que permita a los usuarios automatizar el proceso de encendido/apagado de sus dispositivos que cumplan con la compatibilidad hacia el protocolo WoL (Wake on Lan), misma que se implementaría dentro de una interfaz robusta y accesible hacia los usuarios de Alexa.

# Resumen del producto 

## Organización del proyecto. 

Durante el desarrollo del producto, nos apoyamos en la metodología SCRUM, sin embargo, realizamos ciertas modificaciones para que se adaptará a las características y limitaciones de nuestro proyecto, el punto de utilizar una metodología ágil, se centra en cómo deben de  trabajar los miembros del equipo para producir un sistema flexible en un entorno en cambios constantes.


## Seguimiento de los avances.

La asignación de roles dentro del equipo fue una etapa muy importante, Para controlar el avance de cada sprint se utilizó la herramienta Monday.com, sin embargo en caso de necesitar alguna revisión extra o cambio urgente en la información del repositorio, se realizaron reuniones específicas con los miembros correspondientes para discutir los temas a cambiar o renovar sin ser tomados en cuenta dentro de las tareas del grupo. Al final de cada sprint, se organizaba una "reunión retrospectiva del sprint" de 30 minutos y, en su defecto, cada miembro del equipo compartía sus dificultades y logros dentro del proyecto.

## Explicación de las métricas de contribución individual

Para medir la contribución de cada uno de los integrantes al proyecto se realizaron 2 tablas. En la primera se introdujeron todas las actividades que realizó cada integrante y se calificaron de acuerdo a su relevancia en el proyecto y el desempeño que se tuvo durante la realización de la actividad,obteniendo dos promedios finales para cada integrante: el de relevancia con valor de 55% y el de desempeño con valor de 30%; el porcentaje restante se divide en un 10% con el hecho de haber cumplido con las actividades asignadas y el último 5% con respecto a la asistencia registrada en las reuniones del equipo.

En la segunda tabla en una contabilizamos todos estos factores, posteriormente realizabamos una regla de tres para obtener valores que sumados sean igual al 100%.

Se esperaba que al final de cada incremento cada miembro del equipo aportará con un 20%, al final del tercer incremento realizamos las métricas de contribución individual con respecto a todo el progreso del proyecto. 

# Herramientas SCRUM
# Requirements

The first step in the development process was to create a list of requirements to have a vision of what we want to accomplish with our product. But given that none of the team members had any concrete ideas we decided to make user stories using the comments of the failed skill first:

* US001: As an Alexa user, I want to be able to automate the on/off of my computer to be more efficient.

* US002: As an Alexa user, I want to be able to turn on my computer from another location so I can make more use of my time. 

* US003: As an Alexa user, I want to be able to control other devices such as televisions to have more control over all my devices. 

* US004: As an Alexa user, I want to have instructions to help me to be able to implement the skill. 

* US005: As an Alexa user, I want to schedule a power-on time so that my devices are coupled with my routine and I can make the most of my time. 

* US006: As an Alexa user, I want to be able to customize the name to devices so that controlling them is easier. 

* US007: As an Alexa user, I want to control multiple devices for more control and convenience. 

* US008: As an Alexa user, I want to be able to ask questions within the comments area of the skill to help me solve my doubts. 


The next step was to create a use case diagram in order to view how the step sisystem xd would communicate, behave and interact with the user:


![Imagen 1](https://i.imgur.com/pro31ZN.png)


Once the team had a better idea of what our product should be able to do, we continued on to the creation of the system’s functional and non-functional requirements:

* FR001: The skill will be able to control the on/off options menu of WoL protocol compatible devices through the Alexa assistant.
  * (NFR001): The user will be able to control the skill from any Alexa-enabled device.
  * (NFR002): The user can specify the type of action to be performed: startup, shutdown, sleep, restart and hibernate.
* FR002: Implement, through Microsoft Azure services, a web application where the IP/MAC addresses of the devices will be entered.              
  * (NFR003): The Azure platform will notify the developers of any error with the application.
  * (NFR004): Only developers have access to the database/platform.
  * (NFR005): The user will have to log in with their Amazon account to link their data with Alexa.
* FR003: Implement, through the web application, a bot wizard to help the user enter the IP and MAC address into the database.
  * (NFR006): The bot will assist by means of a tutorial, the way in which the corresponding addresses should be entered.
  * (NFR007): As a "pop up" the bot will issue a message in case of entering a wrong IP/MAC address.
* FR004: There will be a tutorial to show users how to initialize the Alexa skill inside their devices.
  * (NFR008): The tutorial will be opened automatically when the user indicates the corresponding addresses in the bot database.


Although we now had a better idea of the product, the requirements still needed refinement. So we had team discussions on how viable were the requirements from the first sprint, what it was going to take to fully develop our product and of our own skills we made a redesign of the system’s requirements:

* FR001: The skill will be able to control the on/off options menu of WoL protocol compatible devices through the Alexa assistant.
  * (NFR001): The user will be able to control the skill from any Alexa-enabled device.
  * (NFR002): The user can specify the type of action to be performed: startup, shutdown, sleep, restart and hibernate.
* FR002: Develop a web application where the MAC address of the devices will be registered.
  * (NFR004): Only developers have access to the database/platform.
  * (NFR005): The user will have to log in with their Amazon account to link their data with Alexa.
  * (NFR006): There will be a tutorial on how to find and register the Mac address.
  * (NFR007):There will be a tutorial to show users how to initialize the Alexa skill inside their devices.


## Diseño

La etapa de diseño tuvimos dos formas de verla a lo largo del desarrollo, mediante el diseño arquitectónico y diseño de datos, para llegar a una forma de expresar lo necesario de estos dos conceptos, optamos por emplear diagramas que expresaran la información que queríamos. 
Se realizó un diagrama de despliegue que muestra cómo el hardware y el software interactúan entre sí.
(ingrese foto del diagrama)
Y el diagrama de secuencia lo utilizamos enfocado con nuestra página web, mostrando la interacción (acciones a realizar)  esperada entre el usuario y las diferentes áreas que conforman todo el producto.
(ingrese foto del diagrama)
Estos diagramas nos ayudaron a tener un diseño preciso de lo que sería el producto final. todo con información previamente recolectada en las anteriores fases del desarrollo.


## Implementación 


Dentro de la fase de implementación, desarrollamos nuestra aplicación web en JavaScript, aquí los usuarios podrán encontrar ayuda, información de la skill,  personalizar el nombre de sus dispositivos e ingresar su dirección MAC; así poder sincronizar los datos indispensables para el funcionamiento de la skill con la cuenta vinculada a su dispositivo Amazon Alexa.

Nuestra aplicación web se diseñó para ser simple, por ende esta tiene lo mínimo necesario para funcionar, sin descuidar el apartado visual; de igual forma, pensando en la seguridad ésta cuenta con certificado SSL y también con el servicio de “Login with Amazon”, que facilita el inicio de sesión del usuario con su cuenta de Amazon, de una forma confiable

