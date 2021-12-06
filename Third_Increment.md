# Introduction

We are the Alexa Wake On LAN team. Currently technology has evolved at a very fast pace during the life of the human being, it is not to think that less than a century ago the internet was conceived and with it a new way of life and automation. Therefore, as a team we were looking for a way to contribute to automation and streamline everyday processes. We also considered the pandemic situation that governs us and the virtualization of many common processes within the social area (work, school, documentation, etc.). Thanks to this was born the idea of creating a "skill" that allows users to automate the on/off process of their devices that comply with the WoL (Wake on Lan) protocol compatibility, which would be implemented within a robust and accessible interface to Alexa users.


# Summary of the product.

## Project Organization.

During product development, we relied on the SCRUM methodology, however, we made certain modifications to adapt it to the characteristics and limitations of our project, the point of using an agile methodology is focused on how team members should work to produce a flexible system in a constantly changing environment.


## Progress Monitoring.

The assignment of roles within the team was a very important stage. To monitor the progress of each sprint, the Monday.com tool was used, however in case of needing any extra revision or urgent change in the repository information, specific meetings were held with the corresponding members to discuss the issues to be changed or renewed without being taken into account within the group tasks. At the end of each sprint, a 30-minute "sprint retrospective meeting" was organized and, failing that, each team member shared their difficulties and achievements within the project.


## Explanation of individual contribution metrics.

To measure the contribution of each of the members to the project, two tables were created. In the first one we entered all the activities performed by each member and rated them according to their relevance in the project and the performance they had during the activity, obtaining two final averages for each member: relevance with a value of 55% and performance with a value of 30%; the remaining 15% is divided into 10% with the fact of having fulfilled the assigned activities and the last 5% to the attendance recorded in the team meetings.

In the second table we counted all these factors in one, then made a cross multiplication to obtain values that added together equal 100%.

It was expected that at the end of each increment each team member would contribute 20%, at the end of the third increment we made the individual contribution metrics with respect to the whole project progress. And the variation wasn´t that remarkable so we can assume that the workload was evenly distributed during the project.


# SCRUM Tools.
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


# Design

The design stage we had two ways to see it throughout the development, through architectural design and data design, to reach a way to express the necessary of these two concepts, we chose to use diagrams to express the information we wanted. 
A deployment diagram was made to show how the hardware and software interact with each other.
(ingrese foto del diagrama)
On the other hand, we use the sequence diagram focused on our website, showing the expected interaction (actions to be performed) between the user and the different areas that make up the entire product.
(ingrese foto del diagrama)
These diagrams helped us to have an accurate design of what would be the final product, all with information previously collected in the previous phases of development.


# Implementation


Within the implementation phase, we developed our web application in JavaScript, here users can find help, skill information, customize the name of their devices and enter their MAC address; so they can synchronize the essential data for the operation of the skill with the account linked to their Amazon Alexa device.

Our web application was designed to be simple, therefore it has the minimum necessary to function, without neglecting the visual section; likewise, thinking about security it has SSL certificate and also with the service "Login with Amazon", which facilitates the user login with your Amazon account, in a reliable way.

# Subject Proficiencies

## General Proficiencies
### Se comunica en español en forma oral y escrita en sus intervenciones profesionales y en su vida personal, utilizando correctamente el idioma.

Durante el desarrollo de nuestro proyecto la comunicación fue un factor clave, esto fue puesto en marcha al momento de transmitir ideas mediante participaciones ordenadas, respetuosas y sencillas, facilitando la aportación de cada integrante así como hacer más eficiente el manejo de información dentro del equipo. Igualmente la redacción ordenada y clara fue vital para nosotros, pues las ideas aportadas, en la mayoría de los casos, se redactaban directamente en los documentos de las entregas correspondientes, así mismo mantuvieron revisiones gramaticales de manera constante.

### Usa las TIC en sus intervenciones profesionales y en su vida personal de manera responsable.
Gracias a las herramientas implementadas durante toda la vida del proyecto, se mejoró el flujo de trabajo y haciendo más eficaz el manejo de datos e información. Herramientas como Google meet, Visual Studio Code, Git, Github, paquete office, monday, lucid chart fueron consideradas vitales ya que nos brindaron ayuda necesaria en cada fase del proyecto.

### Gestiona el conocimiento en sus intervenciones profesionales y en su vida personal de manera pertinente:
Gracias al aprovechamiento de las habilidades de todos los integrantes, se ha dado trabajo cooperativo, enriquecido gracias al intercambio constante de conocimiento y creatividad al realizar las actividades asignadas a cada integrante.

### Trabaja con otros en ambientes multi, inter y transdisciplinarios de manera cooperativa:
Durante el desarrollo de todo el proyecto hemos compartido experiencias con personas de distintos municipios/estados dando así que las actividades sean manera conjunta y que cada uno realice sus aportes explotando sus capacidades y conocimiento; el intercambio de ideas, conocimientos, experiencias y coordinación fue vital para funcionar como equipo.

### Toma decisiones en su práctica profesional y personal, de manera responsable:
La base del equipo durante todo el desarrollo fue la toma de decisiones ya que ayudó a la formación y distribución de información mediante la comunicación continua de cada integrante. Así mismo se dio prioridad a decisiones en base a fechas límite, dificultades en las etapas de desarrollo del proyecto y documentación general.

## Specific Proficiencies

### Identifica los conceptos vinculados con las fases de requisitos, diseño, desarrollo, pruebas y mantenimiento, de acuerdo los organismos reconocidos en la disciplina:
De manera general, cada uno de los integrantes se desempeñó de manera correcta durante todas las fases, conociendo cada uno de las fases y su implementación. Así también los conocimientos adquiridos en clase fueron complementados con el uso de fuentes de información como el SWEBOK o la IEEE, de esta manera se trazó la ruta que se siguió durante el desarrollo de esta etapa del proyecto.

### Identifica los conceptos vinculados con los procesos de estimación, planificación, seguimiento, control, calidad y configuración, de acuerdo con lo aceptable por organismos reconocidos en la disciplina:
Se tuvo ayuda del mentor, recursos e investigaciones individuales para así aplicar conceptos, prácticas y criterios estándar en cada etapa del proyecto para así mejorar el control del desarrollo de cada fase, en consecuencia, poder comprender mejor las actividades que se realizaron.

### Identifica los factores humanos inmersos en los procesos de desarrollo de software que inciden en el éxito de proyectos de software:
En todo momento se tomó en cuenta las habilidades de cada integrante y por lo tanto focalizar sus fortalezas en las tareas asignadas. Se dio importancia a las aportaciones y la disponibilidad de cada uno y de igual manera, se retroalimentó cada actividad en conjunto para llegar al nivel de satisfacción deseado.

### Utiliza adecuadamente la terminología propia de la Ingeniería de Software en sus intervenciones profesionales:
Se estimuló constantemente a los integrantes a hacer uso de terminología adecuada en cada intervención oral y escrita; en caso de desconocer el término apropiado se instruyeron investigaciones, uso de herramientas como el glosario de la IEEE e igual se contó con la ayuda del mentor quién nos orientó durante toda esta etapa.
