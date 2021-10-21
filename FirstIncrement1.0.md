# **ALEXA SKILL - WAKE ON LAN**

![image](https://i.imgur.com/SqLLo7gl.png)


### Software Engineering Fundamentals

### First Increment

### Team Members: 

* Pablo Gamboa Nieto
* José de Jesús Chi Quintal
* Diego Francisco Arreola Hernández
* Diego Alberto Alamilla Orosco
* Abraham Raymundo Cruz Colli


*Mérida, Yucatán. October 21st, 2021.*



### Application definition:
---

#### **OBJECTIVE**

We want to implement in Amazon Alexa, through the skills store, the use of the WoL (Wake on LAN) protocol to remotely turn on and off compatible computers or televisions automatically using voice. 


#### **PROJECT REACHABILTY**

* Global, or in this case, people who have Alexa Echo devices.


#### **PROJECT LIMITATIONS**

* The possibility of devices not being compatible with the WoL protocol.
* Inability to use outside the Alexa Skill.
* Contents will be in Spanish (tutorials, web/bot platform).


#### **USERS**

We determined that the users of our skill are all those people who have an Amazon Alexa device or the Alexa app and therefore have access to the skill store. According to smart speaker statistics, Amazon Echo had 40.6 million users in 2020, more than Google Home and other smart speaker users combined. Installing an Amazon Echo in your home means you will need to use the Alexa app. Some of the main aspects of Alexa usage are its availability, handy features, and data usage. 

*Estimated growth of potential users.*
*According to Amazon Alexa 2020 statistics, 53.6 million Amazon Echo speakers were sold in the same year. The number is expected to increase to 65 million in 2021.


#### **CUSTOMERS**

Como tal nosotros no tenemos un cliente específico porque detrás del proyecto no hay ninguna persona pagando o interesada por el desarrollo. Por lo cual decidimos que básicamente nuestros futuros usuarios serán considerados como nuestros clientes. Por lo cual usaremos encuestas y formularios para sondear a los potenciales clientes y ser capaces de proporcionar de una buena manera las exigencias y caracteristicas que demanda un cliente para darle profundidad al desarrollo del proyecto. 


#### **INNOVATION/CREATIVITY**

Virtual assistants were not created to satisfy needs, they were created to make life easier for users for simple tasks, such as getting quick information, reading a book or controlling music playback.

There is already an existing Wake On Lan application, but the quality of this one is very low and does not fulfill its purpose. This skill has very low reviews, with a rating of 2.5 stars among more than 150 user reviews, it is a skill that is not tidy or clear instructions, coming to fail with its main purpose, making it an unviable option for the number of users who would like to have this skill functional.

Apart from the previous mentioned, there is no other similar application that takes advantage of Wake on Lan technology, making that if we manage to make a functional, attractive and efficient system, it would be the main application of this technology in Amazon's service, Alexa. We are not looking to create something completely new, but to offer a better alternative to an existing product.

We seek to streamline the on and off of computers and laptops, using the wake on lan function that the devices have, being compatible with most operating systems both current and older (Windows xp, vista, 7), through the virtual assistant Alexa we can start this function with a simple voice command, from anywhere using our mobile device optimizing waiting times to start using the computer.


### **REQUIREMENTS AND USER CASES**

#### **USER CASES**

User stories are a way to look for needs and preferences that the users and/or clients that our project is aimed at want, we formulated many of the ones we have through reviews of a similar skill and testimonials from interested users. We decided to make them as well as the requirements since it is equally important the feedback from people for a project with constant maintenance.

* As an Alexa user, I want to be able to turn on my computer from the bathroom so I can make more use of my time.

* As an Alexa user, I want to be able to automate turning on my computer so I can be more efficient.

* As an Alexa user, I want to be able to automate turning off my computer to save time in my day to day life.

* As an Alexa user, I want to be able to control multiple devices for greater control and convenience.

* As an Alexa user, I want to schedule a power-on schedule so that my devices are paired with my routine and I can make the most of my time.

* As an Alexa user, I want to be able to customize the name to the devices to make controlling them easier.

* As an Alexa user, I want to have instructions to help me be able to implement the skill.

* As an Alexa user, I want to be able to ask questions to help me solve my doubts.

* As an Alexa user, I want to be able to control other devices such as TVs to have more control over all my devices.


#### **REQUIREMENTS SPECIFICATION**

Requirements are a fundamental instrument in the correct development of a software project. They are of great help, both for the client and the development team, to have a concise vision of what features the product is required to have and how they relate to the user.

Due to the simplicity that represents the execution of our product, there are not a large number of requirements that we could devise, but we made them in a way that they fulfill the main characteristics of a requirement. After an extensive process of discussion, elaboration and verification, we have agreed on the following requirements for our project:

###### (FR) stands for "Functional requirements".
###### (NFR) stands for "Non functional requirements".

* FR001: The skill will be able to control the on/off option menu of WoL protocol compatible devices through the Alexa assistant.

   * (NFR): The user will be able to control the skill from any Alexa-enabled device.

   * (NFR): The user will be able to specify the type of action to be performed: startup, shutdown, sleep, reboot and hibernate.

* FR002: Microsoft Azure services will be implemented to host and manage the web application database where the IP/MAC addresses of the devices will be entered.

   * (NFR): The Azure platform will notify the developers of any error with the application.

   * (NFR): Only developers have access to the database/platform.

   * (NFR): The user will have to log in with his Amazon account to link his data with alexa.

* FR003: A wizard bot will be used to help the user enter the IP and MAC address into your database.

   * (NFR): The bot will assist by means of a tutorial, the way in which the corresponding addresses should be entered.

   * (NFR): As a "pop up" the bot will issue a message in case of entering a wrong IP/MAC address.

* FR004: There will be a tutorial to show users how to initialize the alexa skill inside their devices.

   * (NFR): The tutorial will open automatically when the user enters the corresponding addresses into the bot database.


### **PRIORIZATION METHOD**

We use the MoSCoW method to prioritize requirements and user stories. This method integrates very well with our team and project due to the agile methodology we use. The prioritization that MoSCoW handles is divided into 4 categories:

* Must Have: Features without which the project cannot work.

* Should Have: Features that are important in the project, but are not indispensable.

* Could Have: Features that would increase the value of the project if they are present, but are not of great importance.

* Won't have: Features that are not important at present, but could be implemented later.

To make the prioritization as efficient as possible, we held a session with the project owner to discuss where each one should go, based on how feasible it is to implement. Below you can see the results of that discussion:

#### REQUIREMENTS:
##### Must have:
* The skill will be able to control the on/off menu options of WoL protocol compatible devices through the Alexa assistant.
* Only developers have access to the database/platform.
* User will be able to control the skill from any Alexa enabled device.
* The user will be able to specify the type of action to perform: startup, shutdown, sleep, reboot and hibernate.
* The user will have to log in with his Amazon account to link his data with alexa.
##### Should have:
* A tutorial will be provided to show users how to initialize the alexa skill within their devices.
* A bot will be used to help the user enter the IP and MAC address into their database.
##### Could have:
* The bot will assist by means of a tutorial, the way in which the corresponding addresses must be entered.
* The tutorial will open automatically when the user enters the corresponding addresses into the bot database.
* Microsoft Azure services will be implemented to host and manage the web application database where the IP/MAC addresses of the devices will be entered.
* The Azure platform will notify the developers of any error with the application.
##### Won't have but would like to in the future:
* As a "pop up" the bot will emit a message in case of entering a wrong IP/MAC address.


#### USER CASES:
##### Must have:
* As an Alexa user, I want to be able to automate turning on/off my computer to be more efficient.
* As an Alexa user, I want to be able to turn on my computer from somewhere else so I can make more use of my time.
##### Should have:
* As an Alexa user, I want to be able to control other devices such as TVs to have more control over all my devices.
* As an Alexa user, I want to have instructions to help me implement the skill.
##### Could have:
* As an Alexa user, I want to schedule a power-on schedule so that my devices are paired with my routine and I can make the most of my time.
* As an Alexa user, I want to be able to customize the name to devices to make controlling them easier.
* As an Alexa user, I want to control multiple devices for greater control and convenience.
##### Won't have but would like to in the future:
* As an Alexa user, I want to be able to ask questions in the comments area of the skill to help me solve my doubts.


### **USE CASE DIAGRAM**

![Diagrama de casos de uso](Casos.png)

### **ARTIFACTS USED BY THE DEVELOPMENT TEAM**
---

* [X] Google Forms.
* [X] Use case diagram.
* [X] Use case exceptions.
* [X] Brainstorming.

### **USE CASE EXCEPTIONS**

1. If the user wants to name 2 devices the same way, the system will warn the user that a device with that name already exists.

2. In case the user cannot connect to the device, the skill will notify the user that there has been an error.

3. If the user says a device name that he does not recognize, the system will notify the user that the device does not exist.

4. In the event that the user enters the wrong IP and/or Mac address, the system will notify the user that the connection was not successful.

## **DEVELOPMENT PROCESS**

### Methodology


The methodology implemented for the project was based on "SCRUM", which **was adapted to the project** as it is known as an agile methodology, it focuses on how the team members should work in order to produce a flexible system in a constantly changing environment.

At the beginning, a meeting was established to know the skills of the team and the ideas that each member wanted to apply to the project, which through a vote was selected.

Subsequently, and within the Product backlog, a kind of routine was established where the Product Owner established and prioritized the tasks to be performed, thus generating a plan of 2 sprints which were performed in a period of no more than 2 weeks (per sprint). Within the process, the content was created in the form of a "draft" because at first it was done within a Google Docs so that later the Product Owner and the team members could validate the information, then it was introduced into the branch of the member who made it (Github). To control the progress, 2 sessions were held per week, however in case of needing any extra revision or change in the information within the repository, the Product Owner held specific meetings with the corresponding members to discuss the topics to be changed or renewed. At the end of each sprint process, a 30-minute "sprint retrospective meeting" was held and, failing that, each team member shared their difficulties and achievements within the project. The Monday.com tool was used to measure and manage the activities within the sprints.


### Team Roles:


Product Owner:


* Pablo Gamboa Nieto.



SCRUM masters:


* Diego Francisco Arreola Hernández.



* José De Jesús Chi Quintal.


SCRUM team:


* Abraham Raymundo Cruz Colli.


* Diego Alamilla Osorio.


~~An adaptation to the roles assigned by the SCRUM methodology was established, since the role of Product Owner was added to the creation of the Github repository. In the case of SCRUMS masters: facilitating calls and helping to assign tasks to each team member and, failing that, updating the Monday tool in an active way (in less than 3 days).~~

