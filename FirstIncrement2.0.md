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

#### **Objective**

We want to implement in Amazon Alexa, through the skills store, the use of the WoL (Wake on LAN) protocol to remotely turn on and off compatible computers or televisions automatically using voice. 


#### **Project Reachability**

* Global.


#### **Project Limitations**

* The possibility of devices not being compatible with the WoL protocol.
* Inability to use outside the Alexa Skill.
* Contents will be in Spanish (tutorials, web/bot platform).


#### **Users**

We determined that the users of our skill are all those people who have an Amazon Alexa device or the Alexa app and therefore have access to the skill store. According to smart speaker statistics, Amazon Echo had 40.6 million users in 2020, more than Google Home and other smart speaker users combined. Installing an Amazon Echo in your home means you will need to use the Alexa app. Some of the main aspects of Alexa usage are its availability, handy features, and data usage. 

*Estimated growth of potential users.*
*According to Amazon Alexa 2020 statistics, 53.6 million Amazon Echo speakers were sold in the same year. The number is expected to increase to 65 million in 2021.


#### **Customers**

As such we do not have a specific customer because there is no external person interested in the development behind the project. So we decided that basically our future users will be considered as our customers. Therefore we will use surveys and forms to survey potential customers and be able to provide in a good way the requirements and features that a customer demands to give depth to the development of the project. 


#### **Innovation/Creativity**

Virtual assistants were not created to satisfy needs, they were created to make life easier for users for simple tasks, such as getting quick information, reading a book or controlling music playback.

There is already an existing Wake On Lan application, but the quality of this one is very low and does not fulfill its purpose. This skill has very low reviews, with a rating of 2.5 stars among more than 150 user reviews, it is a skill that is not tidy or clear instructions, coming to fail with its main purpose, making it an unviable option for the number of users who would like to have this skill functional.

Apart from the previous mentioned, there is no other similar application that takes advantage of Wake on Lan technology, making that if we manage to make a functional, attractive and efficient system, it would be the main application of this technology in Amazon's service, Alexa. We are not looking to create something completely new, but to offer a better alternative to an existing product.

We seek to streamline the on and off of computers and laptops, using the wake on lan function that the devices have, being compatible with most operating systems both current and older (Windows xp, vista, 7), through the virtual assistant Alexa we can start this function with a simple voice command, from anywhere using our mobile device optimizing waiting times to start using the computer.


### **Priority Method**
---

We use the MoSCoW method to prioritize requirements and user stories. This method integrates very well with our team and project due to the agile methodology we use. The prioritization that MoSCoW handles is divided into 4 categories:

* Must Have: Features without which the project cannot work.

* Should Have: Features that are important in the project, but are not indispensable.

* Could Have: Characteristics that would increase the value of the project if they are present, but are not of great importance.

* Won't have: Features that are not important at present, but could be implemented later.

To make the prioritization as efficient as possible, we held a session with the project owner to discuss where each one should go, based on how feasible it is to implement. The results of that discussion can be seen below:

### **User Stories**
User stories are a way to look for needs and preferences that the users and/or clients that our project is aimed at want, we formulated many of the ones we have through reviews of a similar skill and testimonials from interested users. We decided to make them as well as the requirements since it is equally important the feedback of the people for a project with constant maintenance.

* US001: As an Alexa user, I want to be able to automate the on/off of my computer to be more efficient. **(M)**
* US002: As an Alexa user, I want to be able to turn on my computer from another location so I can make more use of my time. **(M)**
* US003: As an Alexa user, I want to be able to control other devices such as televisions to have more control over all my devices. **(S)**
* US004: As an Alexa user, I want to have instructions to help me to be able to implement the skill.  **(S)**
* US005: As an Alexa user, I want to schedule a power-on time so that my devices are coupled with my routine and I can make the most of my time. **(C)**
* US006: As an Alexa user, I want to be able to customize the name to devices so that controlling them is easier. **(C)**
* US007: As an Alexa user, I want to control multiple devices for more control and convenience. **(C)**
* US008: As an Alexa user, I want to be able to ask questions within the comments area of the skill to help me solve my doubts. **(W)**

### **REQUIREMENTS SPECIFICATION**
--- 

Requirements are a fundamental instrument in the correct development of a software project. They are of great help, both for the client and the development team, to have a concise vision of what features the product is required to have and how they relate to the user.

###### (FR) stands for "Functional Requirements".
###### (NFR) stands for "Non Functional Requirements".

Due to the simplicity that represents the execution of our product, there are not a large number of requirements that we could devise, but we made them in a way that they fulfill the main characteristics of a requirement. After an extended process of discussion, elaboration and verification, we have agreed on the following requirements for our project:

* FR001: The skill will be able to control the on/off options menu of WoL protocol compatible devices through the Alexa assistant. (US001, US002, US003, US005) **(M)**.

   * (NFR001): The user will be able to control the skill from any Alexa-enabled device. **(M)**

   * (NFR002): The user can specify the type of action to be performed: startup, shutdown, sleep, restart and hibernate. **(M)**

* FR002: Implement, through Microsoft Azure services, a web application where the IP/MAC addresses of the devices will be entered. 
(US006, US007) **(C)**

   * (NFR003): The Azure platform will notify the developers of any error with the application. **(C)**

   * (NFR004): Only developers have access to the database/platform. **(M)**

   * (NFR005): The user will have to log in with their Amazon account to link their data with Alexa. **(M)**

* FR003: Implement, through the web application, a bot wizard to help the user enter the IP and MAC address into the database. (US007) **(S)**

   * (NFR006): The bot will assist by means of a tutorial, the way in which the corresponding addresses should be entered. **(C)**

   * (NFR007): As a "pop up" the bot will issue a message in case of entering a wrong IP/MAC address. **(W)**

* FR004: There will be a tutorial to show users how to initialize the Alexa skill inside their devices. (US004, US008) **(S)**

   * (NFR008): The tutorial will be opened automatically when the user indicates the corresponding addresses in the bot database. **(C)**

<br>

### **USE CASE DIAGRAM**
---

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

