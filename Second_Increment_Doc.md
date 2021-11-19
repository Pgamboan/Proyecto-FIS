# Alexa Skill Wake on Lan.

## 2nd Increment.

![image](https://i.imgur.com/SqLLo7gl.png)


### Software Engineering Fundamentals

### Team Members: 

* Pablo Gamboa Nieto
* José de Jesús Chi Quintal
* Diego Francisco Arreola Hernández
* Diego Alberto Alamilla Osorio
* Abraham Raymundo Cruz Colli


*Mérida, Yucatán. Novemeber 18th, 2021.*


### Summary of the progress between the first and second increment. 

When we chose our project, an Alexa skill that takes advantage of the Wake On Lan technology of the devices, we started an investigation of what we were going to need to start developing it, taking into account the technologies and software concepts to make a real software project.
Throughout the first increment there were many discussions about the specification of requirements and the roles that each member would occupy, but an agreement was reached to continue working together and keep progressing based on the scrum methodology.

In this second increment the tracking of the activities was modified to a calendar that was filled together with the logbook notes. Likewise, there were some changes to the requirements according to the difficulty and needs that we found when making the prototype.

### Redesign of the project requirements.

There was a rework of the requeriments based on what the team deemed achievable in the amount of time we had at our disposal and our joint and individual capabilities: We decided that we won't use the Microsoft Azure plataform to host our web app and instead use another host. After carefull consideration we came to the conclusion that the ip address wasn't 100% necessarry to execute the skill, so we decided to remove it's requeriment. Due to lack of necessity, the team decided to scrap the idea of a bot. With the
removal of the bot and it's associated non-functional requeriments, a requirement of a tutorial on how to find the user's MAC address was added. The functional requirement on the the tutorial of the skill's initialization was modified to be a non-functional requeriment of the web app and it's associated non-functional requeriment was deleted.

#### Old:

* FR001: The skill will be able to control the on/off options menu of WoL protocol compatible devices through the Alexa assistant. 

   * (NFR001): The user will be able to control the skill from any Alexa-enabled device. 

   * (NFR002): The user can specify the type of action to be performed: startup, shutdown, sleep, restart and hibernate. 

* FR002: Implement, through Microsoft Azure services, a web application where the IP/MAC addresses of the devices will be entered. 
(US006, US007) **(C)**

   * (NFR003): The Azure platform will notify the developers of any error with the application. 
   
   * (NFR004): Only developers have access to the database/platform. 
   
   * (NFR005): The user will have to log in with their Amazon account to link their data with Alexa. 

* FR003: Implement, through the web application, a bot wizard to help the user enter the IP and MAC address into the database.  

   * (NFR006): The bot will assist by means of a tutorial, the way in which the corresponding addresses should be entered. 

   * (NFR007): As a "pop up" the bot will issue a message in case of entering a wrong IP/MAC address. 

* FR004: There will be a tutorial to show users how to initialize the Alexa skill inside their devices.

   * (NFR008): The tutorial will be opened automatically when the user indicates the corresponding addresses in the bot database. 

#### New:

* FR001: The skill will be able to control the on/off options menu of WoL protocol compatible devices through the Alexa assistant. 

  * (NFR001): The user will be able to control the skill from any Alexa-enabled device. 

  * (NFR002): The user can specify the type of action to be performed: startup, shutdown, sleep, restart and hibernate. 

* FR002: Develop a web application where the MAC address of the devices will be registered. 

  * (NFR004): Only developers have access to the database/platform. 

  * (NFR005): The user will have to log in with their Amazon account to link their data with Alexa. 

  * (NFR005): There will be a tutorial on how to find and register the Mac address.

  * (NFR006):There will be a tutorial to show users how to initialize the Alexa skill inside their devices. 

### Design phase.

In this process we focused on using the information collected in the analysis stage to design the product. Our main task in the design stage is to develop an accurate for the product.

#### Deployment diagram:
Description: This diagram show how hardware and software interact with each other to work properly. To a large extent, these diagrams perfectly describe how the software fits into and interacts with a hardware system. Also, they help show which software element is being deployed by a particular type of hardware.


![image](https://i.imgur.com/IKyvIJ3.png)

#### Sequence diagram:
Description: With this diagram we intend to display the expected interaction between the user and the diferent sections of our product in order to get to the desired result.
The web app was developed in order to give the users a way to provide the information necessarry to the skill's functioning, with the Amazon Web Services beign the bridge for 
such data to be attainable for Alexa.


![image](https://i.imgur.com/fVA3fTc.png)

### Implementation

The proyect's development was divided into two products: the web app were users enter the required data and the alexa skill, that control the devices using said data.

The first step was to create and design the web app. We decided to keep the design simple in order to avoid confusion from the user and save time. It consists of a home page where users can log into their amazon account. This was possible by using the *Login with Amazon* interface provided by Amazon, that lets us link the user's account to the website. But in order to implement the interface, it was necessarry to create a security profile and a privacy policy first.


![image](https://i.imgur.com/MvuSnHQ.png)

Then, when the *Login with Amazon* interface was implemented, we created a button to allow users to login.

Once users are logged in, the web app will redirect them to a new page where they can introduce their devcice's name and MAC address. In the same page the user will find tutorials for each platform in case they don't know how to find their device's MAC address.

### Tests

Because the primary the goal of the website is to link the users infomration with the skill, we decided to postpone tests like usability and instead carry out a conexion module acceptance test.

### Subject Proficiencies

#### GENERAL PROFICIENCIES
<br>

* Communicates in Spanish in oral and written form on their professional interventions and in their personal life, using the language correctly:

 Communication is a key factor when transmitting ideas, this was carried out through orderly, precise and respectful participations. On the other hand, a correct and organized writing is fundamental, so grammatical revisions were constantly maintained during the delivery of tasks assigned to each member.

 * Use ICTs in their professional interventions and in their personal lives in a responsible manner.

 To improve the workflow, tools such as Google meet, Visual Studio Code, Git, Github or ClickUp were used for development, control, project management and teamwork.

 * Manage knowledge in their professional interventions and in their personal life in a relevant way.

 The teamwork has taken advantage of the skills of all members, resulting in a cooperative work, enriched by the constant exchange of knowledge and creativity in carrying out the activities assigned to each member.

 * Works with others in multi-, inter- and trans-disciplinary environments in a cooperative manner:

 The activities were assigned jointly so that each one made their contributions exploiting their skills and knowledge; the exchange of ideas and procedures was an important part of the coordination.

 * Making decisions in their professional and personal practice, in a responsible manner.

 Throughout the delivery certain decisions were made in relation to the development or time estimation, so relevance was given to the skills of each member, deadlines and difficulty of the development stages of the project, whether documentation, coding and / or testing.

<br> 

#### SPECIFIC PROFICIENCIES
<br>

* Identify the concepts related to the phases of requirements, design, development, testing and maintenance, according to the recognized bodies in the discipline.

The knowledge acquired in class was complemented with the use of information sources such as SWEBOK or IEEE, thus tracing the route followed during the development of this stage of the project. 

* Identify the concepts linked to the estimation, planning, monitoring, control, quality and configuration processes, according to what is acceptable by recognized organizations in the discipline: 

Mentor assistance, resources and individual research were used to apply standard concepts, practices and criteria at each stage of the project to improve the control of the development of each phase, and consequently, to better understand the activities that were performed.

* Identify the human factors involved in the software development processes that affect the success of software projects:

At all times the skills of each member were taken into account and therefore focus their strengths in the assigned tasks. The importance was given to the contributions of each one and in the same way, feedback was given to each activity as a whole, thus reaching the desired level of satisfaction.

* The members of the group were constantly encouraged to use the terminology of Software Engineering in their professional interventions.

The members were constantly encouraged to make use of appropriate terminology in each oral and written intervention; in case of not knowing the appropriate term, they were instructed in research, use of tools such as the IEEE glossary and also had the help of the mentor who guided us throughout this stage.

<br>

