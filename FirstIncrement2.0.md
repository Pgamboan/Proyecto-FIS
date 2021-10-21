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
Use case diagrams are necessary to demonstrate in a simple way the communication, behavior and interaction of the system with the users or the different actors involved. Therefore, we chose to use this tool because of its simplicity and readability to understand the operation of our system; then, we defined the use cases and these were written in common/natural language, so that everyone who sees this diagram understands its basic operation.

<br>

![Diagrama de casos de uso](https://i.imgur.com/pro31ZN.png)

<br>

### **ARTEFACTOS UTILIZADOS POR EL EQUIPO DE DESARROLLO**
---
An artifact is a tool deliberately created by the team to solve needs or facilitate certain tasks during the development process of a project. It can also be considered as a work product that provides a description and a definition for tangible work products, i.e. that are well defined.  

* User stories with acceptance criteria (Google Forms): Online forms are an excellent way to reach a specific audience. In our case it was very useful because the results of the online survey are ready to be analyzed at any time and it was a great reference for us to make the user stories. Below we will attach some images that demonstrate the use of this tool.

![grafico](https://i.imgur.com/MQKkYnT.jpeg)
![grafico](https://i.imgur.com/zjUi6H2.jpeg)
![grafico](https://i.imgur.com/u39HJW9.jpeg)

* Use case exceptions: Exceptions were paramount because they helped us to identify potential situations in which we need to prevent in the use case. We anticipated errors that could occur during the execution of the use case.
* Brainstorming: Brainstorming allowed each team member to think more freely. This practice encourages open and continuous collaboration to solve problems and generate innovative ideas. Brainstorming was instrumental in quickly generating a large number of ideas, which can be refined and merged to create the ideal solution for the project.

<br>

### **USE CASE EXCEPTIONS**

1. If the user wants to name 2 devices the same way, the system will warn the user that a device with that name already exists.

2. In case the user cannot connect to the device, the skill will notify the user that there has been an error.

3. If the user says a device name that he does not recognize, the system will notify the user that the device does not exist.

4. In the event that the user enters the wrong IP and/or Mac address, the system will notify the user that the connection was not successful.

## **DEVELOPMENT PROCESS**

**METHODOLOGY**.


The methodology implemented for the project was based on "SCRUM", which **was adapted to the project** because it is known as an agile methodology, it focuses on how the team members should work in order to produce a flexible system in a constantly changing environment.

At the beginning, a meeting was established to know the skills of the team and the ideas that each team member wanted to apply to the project, which was selected through a vote.

Subsequently, the product backlog was established where the Product Owner established and prioritized the tasks to be performed throughout the project, so through sprint planning, the creation of 2 sprint (Definition Process and Development) was estimated, which were planned in a period of no more than 2 weeks (per sprint). Within the process, the content was created in the form of a "draft" because it was initially created within a Google Docs so that all the project members could validate the information and then it was introduced within the branch of the member who created it (Github). To control the progress of each sprint the Monday.com tool was used, however in case of needing any extra revision or urgent change in the repository information, specific meetings were held with the corresponding members to discuss the topics to be changed or renewed without being taken into account within the group tasks. At the end of each sprint, a 30-minute "sprint retrospective meeting" was organized and, failing that, each team member shared their difficulties and achievements within the project. 

<br>

#### **TEAM ROLES:**
---

Product Owner:


* Pablo Gamboa Nieto.



SCRUM masters:


* Diego Francisco Arreola Hernández.



* José De Jesús Chi Quintal.


Developers:


* Abraham Cruz Colli


* Diego Alamilla.

Within the process some team members performed 2 or more roles, i.e., there were occasions where the Product Owner performed the function of SCRUM master, while during the first sprint, the SCRUM Master: José Chi Quintal performed the function of Owner due to the need to make decisions about the product and its content.

<br>

### **PROCESS MANAGEMENT** 
---

<br>

#### **MONITORING TOOLS**

* Monday: Helped us to maintain order in the activities, noting the responsible parties, delivery times and status of the task.

* Google Meet: We used the platform to hold meetings with the tutor and team to work together and present progress.

* WhatsApp: We communicate to arrange meetings, give notices and solve team doubts.

* Github: We used Markdown to create the files, storing and organizing in the repository the contributions of each team member.

* Excel: Helped us in the creation of metrics.

* Word: We elaborated files in this application while we familiarized ourselves with Markdown.

<br>

#### **TASKS**
---


Within the Sprint : Defition Process, the following activities were elaborated:

![Image 1](https://i.imgur.com/fAibM47.png)

Within the Sprint : Development, the following activities were elaborated:


![Image 2](https://i.imgur.com/7urBGDJ.png)


Thus, a contribution metric was contemplated within which each activity was prioritized according to its relevance to the project.

<br>

## **EVIDENCE OF MEETINGS**
---

<br>

### Meeting 1 - Integration
*Date: Tuesday, September 21st, 2021.
* Description: The idea of this meeting was to get to know each other as team members and talk about how we need to engage in order to be successful in the project.
* Agreements/Conflict resolution: 
* Activities: No activities were designated at this meeting.


### Meeting 2 - Brainstorming
* Date: Monday, September 27th, 2021 * Description.
* Description: At this meeting we began brainstorming to agree on how we would each research attractive project ideas to propose.
* Activity: General research of proposals. *(deadline: 09/30/2021)*.

### Meeting 3 - Proposals / Project Selection
*Date: Thursday, September 30, 2021.
* Description: For this meeting, each of us came with a proposal that had caught our attention and the point was to try to convince the rest of the team why that project was the best, in the end we took a vote and chose Alexa's skill.
* Activities: No activities were designated at this meeting.


### Meeting 4 - Review of checklist and delivery 1.
* Date: Sunday, October 3, 2021.
* Description: We started by going through the checklist of the whole project to be clear about what we should do, after that we assigned tasks to start the first deliverable.
* Activities: 
    * Pablo Gamboa - Clients and users *(deadline: 6/10/2021)*
    * Jose Chi - Objective, scope and limitations. (deadline: 6/10/2021)*
    * Diego Arreola - Innovation and creativity. *(deadline: 6/10/2021)* 
    * Diego Alamilla - Innovation and creativity. *(deadline: 6/10/2021)* 
    * Abraham Cruz - Objective, scope and limitations. *(deadline: 6/10/2021)* 
