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

### **Requirements Specification**
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

### **Use Case Diagram**
---
Use case diagrams are necessary to demonstrate in a simple way the communication, behavior and interaction of the system with the users or the different actors involved. Therefore, we chose to use this tool because of its simplicity and readability to understand the operation of our system; then, we defined the use cases and these were written in common/natural language, so that everyone who sees this diagram understands its basic operation.

<br>

![Diagrama de casos de uso](https://i.imgur.com/pro31ZN.png)

<br>

### **Artifacts used by the development team.**
---
An artifact is a tool deliberately created by the team to solve needs or facilitate certain tasks during the development process of a project. It can also be considered as a work product that provides a description and a definition for tangible work products, i.e. that are well defined.  

* User stories with acceptance criteria (Google Forms): Online forms are an excellent way to reach a specific audience. In our case it was very useful because the results of the online survey are ready to be analyzed at any time and it was a great reference for us to make the user stories. Below we will attach some images that demonstrate the use of this tool.

![grafico](https://i.imgur.com/MQKkYnT.jpeg)
![grafico](https://i.imgur.com/zjUi6H2.jpeg)
![grafico](https://i.imgur.com/u39HJW9.jpeg)

* Use case exceptions: Exceptions were paramount because they helped us to identify potential situations in which we need to prevent in the use case. We anticipated errors that could occur during the execution of the use case.
* Brainstorming: Brainstorming allowed each team member to think more freely. This practice encourages open and continuous collaboration to solve problems and generate innovative ideas. Brainstorming was instrumental in quickly generating a large number of ideas, which can be refined and merged to create the ideal solution for the project.

<br>

### **Use Case Exceptions**

1. If the user wants to name 2 devices the same way, the system will warn the user that a device with that name already exists.

2. In case the user cannot connect to the device, the skill will notify the user that there has been an error.

3. If the user says a device name that he does not recognize, the system will notify the user that the device does not exist.

4. In the event that the user enters the wrong IP and/or Mac address, the system will notify the user that the connection was not successful.

## **Development Process**

**Methodology**


The methodology implemented for the project was based on "SCRUM", which **was adapted to the project** because it is known as an agile methodology, it focuses on how the team members should work in order to produce a flexible system in a constantly changing environment.

At the beginning, a meeting was established to know the skills of the team and the ideas that each team member wanted to apply to the project, which was selected through a vote.

Subsequently, the product backlog was established where the Product Owner established and prioritized the tasks to be performed throughout the project, so through sprint planning, the creation of 2 sprint (Definition Process and Development) was estimated, which were planned in a period of no more than 2 weeks (per sprint). Within the process, the content was created in the form of a "draft" because it was initially created within a Google Docs so that all the project members could validate the information and then it was introduced within the branch of the member who created it (Github). To control the progress of each sprint the Monday.com tool was used, however in case of needing any extra revision or urgent change in the repository information, specific meetings were held with the corresponding members to discuss the topics to be changed or renewed without being taken into account within the group tasks. At the end of each sprint, a 30-minute "sprint retrospective meeting" was organized and, failing that, each team member shared their difficulties and achievements within the project. 

<br>

#### **Team Roles:**
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

### **Process Management** 
---

<br>

#### **Monitoring Tools**

* Monday: Helped us to maintain order in the activities, noting the responsible parties, delivery times and status of the task.

* Google Meet: We used the platform to hold meetings with the tutor and team to work together and present progress.

* WhatsApp: We communicate to arrange meetings, give notices and solve team doubts.

* Github: We used Markdown to create the files, storing and organizing in the repository the contributions of each team member.

* Excel: Helped us in the creation of metrics.

* Word: We elaborated files in this application while we familiarized ourselves with Markdown.

<br>

#### **Tasks**
---


Within the Sprint : Defition Process, the following activities were elaborated:

![Image 1](https://i.imgur.com/fAibM47.png)

Within the Sprint : Development, the following activities were elaborated:


![Image 2](https://i.imgur.com/7urBGDJ.png)


Thus, a contribution metric was contemplated within which each activity was prioritized according to its relevance to the project.

<br>

## **Evidence of Meetings**
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
*Date: Thursday, September 30th, 2021.
* Description: For this meeting, each of us came with a proposal that had caught our attention and the point was to try to convince the rest of the team why that project was the best, in the end we took a vote and chose Alexa's skill.
* Activities: No activities were designated at this meeting.


### Meeting 4 - Review of checklist and delivery 1.
* Date: Sunday, October 3rd, 2021.
* Description: We started by going through the checklist of the whole project to be clear about what we should do, after that we assigned tasks to start the first deliverable.
* Activities: 
    * Pablo Gamboa - Clients and users *(deadline: 10/06/2021)*
    * Jose Chi - Objective, scope and limitations. (deadline: 10/06/2021)*
    * Diego Arreola - Innovation and creativity. *(deadline: 10/06/2021)* 
    * Diego Alamilla - Innovation and creativity. *(deadline: 10/06/2021)* 
    * Abraham Cruz - Objective, scope and limitations. *(deadline: 10/06/2021)* 

### Meeting 5 - Preparation for video call with mentor, clarifications sprint 1. 
*Date: Wednesday, October 6th, 2021. 
* Description: We reviewed the progress of deliverable number one, clarified the team's doubts and discussed the last details we wanted to land with our mentor Jose Luis.
* Activities: No tasks were designated in this meeting.


### Meeting 6 - First contact with the mentor, receive feedback on the project.
*Date: Wednesday, October 6th, 2021 * Description: We met our mentor Jose Luis.
* Description: We met our mentor Jose Luis and introduced him to our project idea, we talked about the scope and limitations of the project, we also downloaded the app "monday" to keep track of the progress for the activities.
* Activities: 
    * Pablo Gamboa Nieto - Elaboration of the google forms. *(deadline: 10/12/2021)*
    * Jose Chi - Tracking tool configuration. *(deadline: 10/12/2021)* 
    * Diego Alamilla - Quality control review. *(deadline: 10/12/2021)* 
    * Abraham Cruz - Elaboration of markdown cheatsheet. *(deadline: 10/12/2021)*

### Meeting 7 - User Stories, Requirements and Markdown.
#### Ending of Sprint #1
    * Challenges: Innovation, achievability and determining our customers.
    * Progress: Project description.
    * Achievements: We understood more in depth the objective of the project.
* Date: Tuesday, October 12th, 2021 * Date: Tuesday, October 12, 2021 * Date: Tuesday, October 12, 2021 * Date.
* Description: In this meeting the team discussed user stories and prioritization methods. We also started to familiarize ourselves with Markdown to start adding the project information to the Github repository.
* Activities: 
    * Pablo Gamboa - Add log to the repository and investigate non-functional requirements. * (deadline: 10/14/2021)* 
    * Jose Chi - Writing user stories. *(deadline: 10/14/2021)* 
    * Diego Arreola - Functional requirements research. *(deadline: 10/14/2021)*
    * Diego Alamilla - User story writing. *(deadline: 10/14/2021)*
    * Abraham Cruz - In-depth investigation of the operation of a use case diagram. *(deadline: 10/14/2021)*

### Meeting 8 - Elaboration of branches for individual contributions in Markdown. 
*Date: Thursday, October 14th, 2021.
* Description: In this meeting we form different branches for each team member to keep a control panel in the repository, we start the elaboration of the markdown previews and clarify the concept of the use case diagram.
* Activities: 
    * Pablo Gamboa - Add the first version of the repository requirements. *(deadline: 10/16/2021)*
    * Jose Chi - Add the user stories to the repository. *(deadline: 10/16/2021)* 
    * Diego Arreola - Add the first version of the repository requirements. *(deadline: 10/16/2021)*
    * Diego Alamilla - Add product description to the repository. *(deadline: 10/16/2021)*
    * Abraham Cruz - Use case diagram. *(deadline: 10/16/2021) *(deadline: 10/16/2021)*

### Meeting 9 - Validation of project requirements.
*Date: Saturday, October 16th, 2021.
* Description: Together we review the requirements specification document and begin to tie together the different parts of the project into the first delivery branch of the github repository.
* Activities: 
    * Pablo Gamboa - Requirements verification. *(deadline: 10/18/2021)*
    * Jose Chi - Requirements verification. *(deadline: 10/18/2021)*
    * Diego Arreola - Verification of requirements. *(deadline: 10/18/2021)*
    * Diego Alamilla - Markdown merging progress. *(deadline: 10/18/2021)*
    * Abraham Cruz - Markdown merging progress. *(deadline: 10/18/2021)*

### Meeting 10 - Redesign of MoSCoW requirements and method.
*Date: Monday, October 18th, 2021.
* Description: During this meeting we took care of modifying the last details of the requirements specification list, we found the need to remove several requirements that were not quite in line with our idea. We used the moscow method to prioritize the user stories. 
* Activities: 
    * Diego Alamilla - Prioritization of user stories. *(deadline: 10/19/2021)*
    * Abraham Cruz - Prioritization of user stories. *(deadline: 10/19/2021)*
    * Jose Chi - Requirements prioritization with MosCoW. *(deadline: 10/19/2021)*
    * Diego Arreola - MosCoW requirements prioritization. *(deadline: 10/19/2021)*


### Meeting 11 - Method of prioritization of requirements. 
*Date: Tuesday, October 19th, 2021. (07:30 a.m.) *.
* Description: In this meeting, we reviewed the prioritization of functional and non-functional requirements with the MoSCoW method and made the assignment of tasks within the Monday platform to keep track and get organized.
* Activities: 
    * Pablo Gamboa - Redesign of the customer section. *(deadline: 10/19/2021)*
    * Diego Alamilla - Drafting of quality control method. *(deadline: 10/19/2021)*
    * Diego Arreola - Writing of subject competencies. *(deadline: 10/19/2021)*


### Meeting 12 - Preparation of the deliverable document.
Date: Tuesday, October 19th, 2021 (18:00 p.m.)* * Description: We reviewed with the checklist the elements we had to fulfill.
* Description: We reviewed with the checklist the elements that we had to comply with.
* Activities: 
    * Pablo Gamboa - Translation of the deliverable into English. *(deadline: 10/20/2021)* 
    * Jose Chi - Description of the process. *(deadline: 10/20/2021)* 
    * Diego Arreola - Prioritization method description. *(deadline: 10/20/2021)* 
    * Diego Alamilla - Transcription of the metrics table to markdown. *(deadline: 10/20/2021)* 
    * Abraham Cruz - Description of use case diagram. *(deadline: 10/20/2021)* 

### Meeting 13 - Presentation of progress with the mentor. 
*Date: Tuesday, October 20th, 2021 (08:00 a.m.)*.
* Description: In this meeting we presented our document to Professor Jose Luis and received feedback and adjusted according to the correct specifications of the agile methodology. We also numbered all the user stories and non-functional requirements to relate them to each other. Finally we designated tasks to work on during the course of the day and present them in the afternoon meeting.
* Activities: 
    * Pablo Gamboa - Restructuring of the individual metrics table. *(deadline: 10/20/2021)*
    * Jose Chi - Scrum Methodology.  *(deadline: 10/20/2021)*
    * Diego Arreola - Detail the subject competencies.   *(deadline: 10/20/2021)*
    * Diego Alamilla - Relate user stories with requirements.   *(deadline: 10/20/2021)*
    * Abraham Cruz - Relate user stories with requirements.   *(deadline: 10/20/2021)*

### Meeting 14 - Final product and video recording.
#### Ending of Sprint #2 
    * Difficulties: Coordinating assignments and reaching agreements with all the team regarding to the project specifications.
    * Progress: Completed all the checklist items.
    * Accomplishments: Broad understanding of the development process and learned the importance of correctly applying the SCRUM methodology. 
Date: Tuesday, October 20th, 2021.(17:00 p.m.)* * Description: Presentation and finalization of the SCRUM methodology.
* Description: Presentation and we finalized the contribution tracker.
* Activities: 
    * Pablo Gamboa - Contribution tracker and log detailing. *(deadline: 10/20/2021)*
    * Jose Chi - Finalize the description of the process, contribute to the presentation and editing of the video *(deadline: 10/20/2021)*
    * Diego Arreola - Elaboration of the presentation. *(deadline: 10/20/2021)*
    * Diego Alamilla - Document binding and quality control. *(deadline: 10/20/2021)*
    * Abraham Cruz - Contribution tracker and markdown document ordering. *(deadline: 10/20/2021)*

<br>


### **Quality Control**
---

To verify the quality and that the project met our expectations, when performing tasks, we checked that all members of the team were in agreement with the result.
If there were mistakes, correct them during the meetings to reach a common agreement. At the same time we were all helping and contributing 
in the different parts of the project, contributing all the necessary knowledge to make it as complete as possible.

During the completion of the activities and at the end, member Diego Alberto Alamilla Osorio, was in charge of reviewing and correcting syntax, order and writing errors if necessary. 
syntax, order and wording if there were any. Thus ensuring to deliver a project as polished and meeting the required expectations.

<br>

### **TeamWork**
---
#### Repository: 

#### Metric of individual contribution: 

#### Verification of the contribution percentage: 

### **Subject proficiency**.

<br>

#### **General Proficiency** 
-------
* **Communicates orally and in writing in Spanish in professional and personal life, using the language correctly:** 
* **Communicates in Spanish in an orderly and clear manner to achieve greater effectiveness in the ideas to be conveyed.**
* **Communication in the sessions was done in an orderly and clear manner in order to achieve greater effectiveness in the ideas to be transmitted. In addition to this, several revisions were made in the wording of the whole project to achieve the same objective.**
* **Use ICTs in their professional interventions and in their personal lives in a relevant and responsible way:** 
* **A wide range of tools were used in the project.**
* **A wide range of digital tools, such as Meet for team meetings; Monday for activity tracking and Excel for charting, were used to maximize workflow efficiency.**
* **Manages knowledge in their professional interventions and in their personal lives, in a relevant way:** 
* **Knowledge and skills of the team are managed in a relevant way.**
* **The team's knowledge and skills were maximized in the development of the activities, the elaboration of files and the presentation of progress required skills and knowledge. Knowledge was shared in team sessions so that we all had an equal understanding of what we wanted to accomplish and how we planned to do it.**
* **Work with others in multi-, inter- and trans-disciplinary environments in a cooperative manner.Each team member took on activities that made the most of the skills and knowledge they possessed, and worked together so that the workload was distributed in an equitable and balanced manner.**

<br>

#### **Specific Proficiency** 
-----
* **Identifies the concepts linked to the phases of requirements, design, development, testing and maintenance, according to the recognized bodies in the discipline:**
* **Identifies the concepts linked to the phases of requirements, design, development, testing and maintenance, according to the recognized bodies in the discipline
 Information from the relevant phases at the current stage of the project was used to direct the development of the project. The progress of the project progressed as the classes helped us to understand the information and the research that the members did on their own.**
* **Identify the human factors involved in software development processes that affect the success of software projects. We took into account the strengths and weaknesses of the team members when assigning roles and tasks. We also organized meetings that were adjusted to the schedules of all team members, to present progress and complement the development of activities.**
* **The team members adequately used the terminology of Software Engineering in their professional interventions:**
* **With the research done by the members of the team. With the research done by the team members, we tried to use in the best way the terms relevant to the project. More advanced issues needed the support of the team tutor who guided us, recommended readings and paths we could take to have a better understanding of these concepts.**

<br>
