# Alexa Skill Wake on Lan.

## 3nd Increment.

![image](https://i.imgur.com/SqLLo7gl.png)


### Software Engineering Fundamentals

### Team Members: 

* Pablo Gamboa Nieto
* José de Jesús Chi Quintal
* Diego Francisco Arreola Hernández
* Diego Alberto Alamilla Osorio
* Abraham Raymundo Cruz Colli


*Mérida, Yucatán. December 6th, 2021.*

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

![image](https://i.imgur.com/IKyvIJ3.png)

On the other hand, we use the sequence diagram focused on our website, showing the expected interaction (actions to be performed) between the user and the different areas that make up the entire product.


![image](https://i.imgur.com/fVA3fTc.png)

These diagrams helped us to have an accurate design of what would be the final product, all with information previously collected in the previous phases of development.


# Implementation


Within the implementation phase, we developed our web application in JavaScript, here users can find help, skill information, customize the name of their devices and enter their MAC address; so they can synchronize the essential data for the operation of the skill with the account linked to their Amazon Alexa device.

![image](https://i.imgur.com/4NSgWLj.png)


Our web application was designed to be simple, therefore it has the minimum necessary to function, without neglecting the visual section; likewise, thinking about security it has SSL certificate and also with the service "Login with Amazon", which facilitates the user login with your Amazon account, in a reliable way.

![image](https://i.imgur.com/SWorcIl.png)

![image](https://i.imgur.com/MvuSnHQ.png)

# Testing

## Connection module test (Login):

By using the LwA (Login with Amazon with Javascript) interface, the login button connection module test was performed without attaching any test code. Simply evaluating that the conditions are met so that through the SDK the code is executed and the button with the id=" LoginWithamazon" has functionality. So, through and the SDK was thrown to the Amazon authorized page "Index2" indicating a successful login. However, a test code was also implemented, given the LwA interface, to corroborate that the login had been successful; this threw a greeting message, the account email and additionally the Amazon ID (unique per user), also indicating that the implemented code was correct. Giving the test as finished, ensuring the operation and reliability of the module.


# Subject Proficiencies

## General Proficiencies

### Communicates in Spanish in oral and written form in their professional interventions and in their personal life, using the language correctly.
During the development of our project, communication was a key factor, this was put into action at the moment of transmitting ideas through orderly, respectful and simple participations, facilitating the contribution of each member as well as making the management of information within the team more efficient. Likewise, the orderly and clear writing was vital for us, since the ideas contributed, in most cases, were written directly in the documents of the corresponding deliverables, as well as maintaining constant grammatical revisions.

### Use of ICTs in their professional interventions and in their personal lives in a responsible manner.
Thanks to the tools implemented throughout the life of the project, the workflow was improved and the management of data and information was made more efficient. Tools such as Google meet, Visual Studio Code, Git, Github, office package, monday, lucid chart were considered vital as they provided us with the necessary help in each phase of the project.

### Manage knowledge in their professional interventions and in their personal life in a relevant way:
Thanks to the use of the skills of all members, there has been cooperative work, enriched thanks to the constant exchange of knowledge and creativity in carrying out the activities assigned to each member.

### Work with others in multi-, inter- and trans-disciplinary environments in a cooperative manner:
During the development of the entire project we have shared experiences with people from different municipalities/states thus giving that the activities are a joint way and that each one makes their contributions exploiting their capabilities and knowledge; the exchange of ideas, knowledge, experiences and coordination was vital to function as a team.

### Make decisions in their professional and personal practice, in a responsible manner:
The basis of the team throughout the development was decision making as it helped the formation and distribution of information through continuous communication of each member. Likewise, decisions were prioritized based on deadlines, difficulties in the development stages of the project and general documentation.

## Specific Proficiencies

### Identifies the concepts related to the phases of requirements, design, development, testing and maintenance, according to the recognized organizations in the discipline:
In general, each of the members performed correctly during all phases, knowing each of the phases and their implementation. Also the knowledge acquired in class was complemented with the use of information sources such as SWEBOK or IEEE, in this way the route that was followed during the development of this stage of the project was traced.

### Identifies the concepts related to the estimation, planning, monitoring, control, quality and configuration processes, according to what is acceptable by recognized organizations in the discipline:
Mentor assistance, resources and individual research was taken to apply standard concepts, practices and criteria at each stage of the project to improve the control of the development of each phase, consequently, to better understand the activities that were performed.

### Identifies the human factors involved in software development processes that affect the success of software projects:
At all times the skills of each member were taken into account and therefore focus their strengths in the assigned tasks. Importance was given to the contributions and availability of each one and in the same way, feedback was given to each activity as a whole in order to reach the desired level of satisfaction.

### The terminology of Software Engineering was used appropriately in their professional interventions:
The members were constantly encouraged to make use of appropriate terminology in each oral and written intervention; in case of not knowing the appropriate term, research was instructed, use of tools such as the IEEE glossary and likewise we had the help of the mentor who guided us throughout this stage.
