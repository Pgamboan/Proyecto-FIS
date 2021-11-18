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


### Summary of the progress in the second increment. 

When we chose our project, an Alexa skill that takes advantage of the Wake On Lan technology of the devices, we started an investigation of what we were going to need to start developing it, taking into account the technologies and software concepts to make a real software project.
Throughout the first increment there were many discussions about the specification of requirements and the roles that each member would occupy, but an agreement was reached to continue working together and keep progressing based on the scrum methodology.

In this second increment the tracking of the activities was modified to a calendar that was filled together with the logbook notes. Likewise, there were some changes to the requirements according to the difficulty and needs that we found when making the prototype.

### Redesign of the project requirements.

There was a rework of the requeriments based on what the team deemed achievable in the amount of time we had at our disposal and our joint and individual capabilities: We decided that we won't use the Microsoft Azure plataform to host our web app and instead use another host. After carefull consideration we came to the conclusion that the ip address wasn't 100% necessarry to execute the skill, so we decided to remove it's requeriment. Due to lack of necessity, the team decided to scrap the idea of a bot. 

Old:

New:

FR001: The skill will be able to control the on/off options menu of WoL protocol compatible devices through the Alexa assistant. (US001, US002, US003, US005) (M).

(NFR001): The user will be able to control the skill from any Alexa-enabled device. (M)

(NFR002): The user can specify the type of action to be performed: startup, shutdown, sleep, restart and hibernate. (M)

FR002: Develop a web application where the MAC address of the devices will be registered. (US006, US007) (C)

(NFR004): Only developers have access to the database/platform. (M)

(NFR005): The user will have to log in with their Amazon account to link their data with Alexa. (M)

FR003: There will be a tutorial on how to find and register the Mac address.(S)

(NFR006):-------(C)

(NFR007): As a "pop up" the web app will issue a message in case of entering a wrong MAC address. (W)

FR004: There will be a tutorial to show users how to initialize the Alexa skill inside their devices. (US004, US008) (S)

(NFR008): The tutorial will be opened automatically when the user indicates the corresponding address in the web app. (C)

### Design phase.

In this process we focused on using the information collected in the analysis stage to design the product. Our main task in the design stage is to develop an accurate for the product.

#### Deployment diagram.
Description: This diagram show how hardware and software interact with each other to work properly. To a large extent, these diagrams perfectly describe how the software fits into and interacts with a hardware system. Also, they help show which software element is being deployed by a particular type of hardware.


![image](https://i.imgur.com/pKhaADq.png)

#### Sequenze diagram.
Description: With this diagram we intend to display the expected interaction between the user and the diferent sections of our product in order to get to the desired result.
The web app was developed in order to give the users a way to provide the information necessarry to the skill's functioning, with the Amazon Web Services beign the bridge for 
such data to be attainable for Alexa.




![image](https://i.imgur.com/fVA3fTc.png)

### Implementation

*introducir labia acá*
