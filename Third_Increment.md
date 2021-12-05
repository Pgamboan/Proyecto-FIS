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

## Subject Proficiencies

### General Proficiencies
#### Se comunica en español en forma oral y escrita en sus intervenciones profesionales y en su vida personal, utilizando correctamente el idioma.

Durante el desarrollo de nuestro proyecto la comunicación fue un factor clave, esto fue puesto en marcha al momento de transmitir ideas mediante participaciones ordenadas, respetuosas y sencillas, facilitando la aportación de cada integrante así como hacer más eficiente el manejo de información dentro del equipo. Igualmente la redacción ordenada y clara fue vital para nosotros, pues las ideas aportadas, en la mayoría de los casos, se redactaban directamente en los documentos de las entregas correspondientes, así mismo mantuvieron revisiones gramaticales de manera constante.

#### Usa las TIC en sus intervenciones profesionales y en su vida personal de manera responsable.
Gracias a las herramientas implementadas durante toda la vida del proyecto, se mejoró el flujo de trabajo y haciendo más eficaz el manejo de datos e información. Herramientas como Google meet, Visual Studio Code, Git, Github, paquete office, monday, lucid chart fueron consideradas vitales ya que nos brindaron ayuda necesaria en cada fase del proyecto.
#### Gestiona el conocimiento en sus intervenciones profesionales y en su vida personal de manera pertinente:
Gracias al aprovechamiento de las habilidades de todos los integrantes, se ha dado trabajo cooperativo, enriquecido gracias al intercambio constante de conocimiento y creatividad al realizar las actividades asignadas a cada integrante.
#### Trabaja con otros en ambientes multi, inter y transdisciplinarios de manera cooperativa:
Durante el desarrollo de todo el proyecto hemos compartido experiencias con personas de distintos municipios/estados dando así que las actividades sean manera conjunta y que cada uno realice sus aportes explotando sus capacidades y conocimiento; el intercambio de ideas, conocimientos, experiencias y coordinación fue vital para funcionar como equipo.
#### Toma decisiones en su práctica profesional y personal, de manera responsable:
La base del equipo durante todo el desarrollo fue la toma de decisiones ya que ayudó a la formación y distribución de información mediante la comunicación continua de cada integrante. Así mismo se dio prioridad a decisiones en base a fechas límite, dificultades en las etapas de desarrollo del proyecto y documentación general.

### Specific Proficiencies

#### Identifica los conceptos vinculados con las fases de requisitos, diseño, desarrollo, pruebas y mantenimiento, de acuerdo los organismos reconocidos en la disciplina:
De manera general, cada uno de los integrantes se desempeñó de manera correcta durante todas las fases, conociendo cada uno de las fases y su implementación. Así también los conocimientos adquiridos en clase fueron complementados con el uso de fuentes de información como el SWEBOK o la IEEE, de esta manera se trazó la ruta que se siguió durante el desarrollo de esta etapa del proyecto.
#### Identifica los conceptos vinculados con los procesos de estimación, planificación, seguimiento, control, calidad y configuración, de acuerdo con lo aceptable por organismos reconocidos en la disciplina:
Se tuvo ayuda del mentor, recursos e investigaciones individuales para así aplicar conceptos, prácticas y criterios estándar en cada etapa del proyecto para así mejorar el control del desarrollo de cada fase, en consecuencia, poder comprender mejor las actividades que se realizaron.
#### Identifica los factores humanos inmersos en los procesos de desarrollo de software que inciden en el éxito de proyectos de software:
En todo momento se tomó en cuenta las habilidades de cada integrante y por lo tanto focalizar sus fortalezas en las tareas asignadas. Se dio importancia a las aportaciones y la disponibilidad de cada uno y de igual manera, se retroalimentó cada actividad en conjunto para llegar al nivel de satisfacción deseado.
#### Utiliza adecuadamente la terminología propia de la Ingeniería de Software en sus intervenciones profesionales:
Se estimuló constantemente a los integrantes a hacer uso de terminología adecuada en cada intervención oral y escrita; en caso de desconocer el término apropiado se instruyeron investigaciones, uso de herramientas como el glosario de la IEEE e igual se contó con la ayuda del mentor quién nos orientó durante toda esta etapa.
