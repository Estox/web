# Google Summer of Code 2019 Ideas

02 Feb 2019

Here we have a list of the final ideas and students selected for GSOC' 2019:  


# Google Summer of Code 2019 Ideas

02 Feb 2019

## General information on applications

This is the list of ideas for the Google Summer of Code 2019, if you are interested in any of the ideas listed below we encourage you to apply.

* It is important to first familiarize with the software ([https://github.com/robocomp/robocomp](https://github.com/robocomp/robocomp)).
* Please, go through the available tutorials and direct your questions to the gitter chat (links available in contact section).
* Please read all the information posted in this page before applying.
* Make sure you are familiar with the required skills for the idea.
* Since several of the mentioned RoboComp tools and components are not explained here to keep this list short, we encourage everyone to check the RoboComp documentation linked below.
* Mentors and backup mentors are listed right after the idea explanation. All mentors contact info is at the end of the page. Contact them directly for specific questions on the idea.


Robocomp installation and tutorials: [https://github.com/robocomp/robocomp/tree/stable/doc#tutorials](https://github.com/robocomp/robocomp/tree/stable/doc#tutorials)

**Where can I start and what to include on my application?**

You are encouraged to go through these steps for a better understanding and follow-up of your application:

1.  Download and install RoboComp: [https://github.com/robocomp/robocomp/blob/stable/README.md](https://github.com/robocomp/robocomp/blob/stable/README.md).
2.  Follow the tutorials: [https://github.com/robocomp/robocomp/tree/stable/doc#tutorials](https://github.com/robocomp/robocomp/tree/stable/doc#tutorials).
3.  Once you are familiar with RoboComp and the components and tools involved in the particular idea you want to contribute to, try to understand how these components/tools work and, if possible, their design.
4.  Participate in gsoc [gitter](https://gitter.im/robocomp/robocomp/robocomp-gsoc) asking any question you might have.
5.  Create a schedule with the milestones you plan to follow during the GSoC 2019 program.
6.  **Send the schedule and any code you might have written along with your CV and other application materials to the mentor of your idea and the backup mentor.**

For general questions about RoboComp please use: The [gitter chat](https://gitter.im/robocomp/robocomp).


## IDEAS LIST for GSoC 2019

### 1\. Implementation of a distributed graph-based world representation for robots
**Mentors**  
Pablo Bustos, Cristian Vázquez
 
**Brief description**  
As the tasks that autonomous robots perform become complex, the need to explicitly represent the world surrounding autonomous robots becomes clearer. The presence of humans and the need to manipulate multiple objects make these representations complex, comprising hundreds of data elements combining geometric and symbolic information. On the other hand, advanced autonomous robots are not designed as monolithic programs but as networks of software components whose interaction defines robots’ behaviour. Sharing these complex world representations in a centralised fashion raises efficiency concerns that can be overcome distributing the world representation. The goal of this GSoC slot is to contribute to the implementation of the distributed technology that the RoboComp team is currently working on.

**Needed skills**  
c++11

### 2\. Learning acceptable social behaviour using machine learning techniques 
**Mentors**
Luis J. Manso, Pedro Nuñez

**Brief description**  
The detection and implementation of social skills is usually handcrafted by developers writing hardcoded if-then-else constructs in the robots’ code. This code usually consists of a series of queries to the robots’ world representations (e.g., if the robot is closer than 400mm to a human the person might consider the behaviour inappropriate, if two humans are interacting the robot should not interrupt their visual contact). The aim of this slot is to include in RoboComp a feature to learn to classify social behaviours as desirable or undesirable. The input information to do such classifications would be the robot’s world representation (a graph), and the dataset will be generated by the student and the mentors, using the simulation tool and the camera system available at the University of Extremadura.

**Needed skills**  
python, basic machine learning

### 3\. Human-robot dialogue and collaboration for social navigation   
**Mentors**  
Araceli Vega, Pedro Núñez

**Brief description**  
The navigation of a robot in an environment with humans is a subject with enormous interest in the last years. To be accepted in these types of scenarios, it is important that the robot navigate respecting social norms, for example, avoiding getting too close to humans, avoiding interrupting a conversation or asking permission to pass through a blocked path. The aim to this slot is to describe the dialog manager, besides of the corpus that allows to establish dialogues between the robot and the human in real situations in order to improve the behavior of the robot navigation system, making  it more socially accepted. The dialog manager should be a RoboComp agent, which read information from the robot’s world representation (a graph) and adapt the conversation to the current situation (e.g, according to the age of people, genre, etc). The idea of this slot is of integrating the tool pyText, an open-source Natural Language Processing tool recently developed by facebook:AI team.  

**Needed skills**  
...

### 4\. Development of a human activity recognition component
**Mentors**  
Diego Faria, Luis J. Manso

**Brief description**  
Nowadays with the advances of robotics research worldwide, a cognitive robot can act as human assistant in the context of assisted living, and also with the potential to offer social and entertaining interaction experiences through human-robot interaction. For that, in order to enable this natural and social human-robot interaction, a robot needs to infer human intentions, their daily routine and potential risk situations (e.g. fall detection) by observing them. Human behaviour recognition has been a very active topic of research in different fields, such as computer vision, robotics, machine learning & pattern recognition. It is still a very challenging research topic, due to the inherently complex temporal and spatial patterns that characterise most human body motions.  The aim of this slot is to include in RoboComp a feature for human daily activity recognition using data from an RGB-D sensor. Essentially, we will develop approaches for activity recognition relying on 3D spatio-temporal features from skeleton data (joint position/motion data).  Different classical machine learning techniques will be used to verify their performance on a public available dataset, e.g. CAD-60 (Cornell Daily Activities Dataset). Our final goal is to develop a competitive framework (features extraction+classifier(s)) of daily activity recognition as a RoboComp recognition component to attain high accuracy comparable with the state-of-the-art on CAD-60 ranking table.

**Needed skills**  
python

### 5\. Interactive robotic simulator
**Mentors**  
Pilar Bachiller, Sparsh Garg


**Brief description**  
RCIS is the robotic simulator of the RoboComp framework. This simulator is very useful for multiple purposes. It can simulate complex worlds and provides a hardware abstraction layer for simulated robots that facilitates testing robot behaviors without modifying any line of code of the high-level components. Thus, the simulated robot can perceive the environment through its sensors and act upon the environment through its actuator as the physical robot does. Nevertheless the simulated worlds are static. The user can not change the position of an object or add new elements during the simulation. The aim of this project is to improve RCIS, adding options that make modifications of the environment possible during a simulation. This new feature will allow the user for interacting with the simulated robot to test more complex situations.

**Needed skills**  
...

### 6\. People identification component for the EBO educational robot
**Mentors**  
Pilar Bachiller, Nicolás González

**Brief description**  
EBO is an educational robot created by RoboLab to help children to learn programming concepts. EBO can exhibit not only motor behaviors, but also emotional ones, which makes it an interesting tool for the design of activities related to emotional management. The programming tool of EBO includes a wide range of functionality, such as color detection, face detection, emotion recognition and mark identification. Despite the combinations of these skills give rise to a great variety of interactive behaviors between the robot and a human, we want to go a step further, endowing EBO with the ability to identify a known person and “meet” new people. To this end, this project aims to create a people identification component for our educational robot. The component should provide two operation modes: “classify a new person” and “identify known people”. In the first mode, the component will receive a set of images and a name identifying the person. In addition, images of previously classified persons can be sent to the component. Thus, incremental learning techniques should be applied for the implementation of this new component. In the second mode, the component will receive an image and, after classifying all the faces on it, will return a list of identified persons.

**Needed skills**  
...


### 7\. Bluetooth extension for RoboComp
**Mentors**  
Iván Barbecho, Marco A. Gutiérrez


**Brief description**  
Components currently generated with RoboComp use Ethernet networks to communicate but these type of networks are not always available. This idea proposes to add another communication technology to RoboComp that can connect components in Ethernet deprived areas. This technology would be Bluetooth and it will be incorporated using the ZeroC IceBT plugin to the Ice middleware. It will be tested first and then integrated into the RoboComp’s source code generator, so it becomes available as an option to anyone creating a new component.  This technology will provide some additional advantages such as low power consumption and wireless communication over devices 10 meters apart.

**Needed skills**  
...

### 8\. New examples and scenarios for swarm robotics in RoboComp
**Mentors**  
Francisco Andrés, Pilar Bachiller

**Brief description**  
Nowadays technology is constantly changing, a great example is RoboComp. Thus, the creation of new context scenarios is constantly needed to test the devices with which we work. We must consider that the level of distributed communication in educational robotics scenarios is very complex. It is proposed to create examples of robots’ swarms that help deepen more effective communication mechanisms. The swarm intelligence is an approach to optimal solutions taking its inspiration from social living beings. Thanks to the data collected by the different individuals we will be able to achieve a great possibility of objectives. We believe that through this project we can find  examples that help improving the quality of our robots to achieve better results.

**Needed skills**  
...


### 9\. Neural Compute Stick 2 as a RoboComp hybrid component 
**Mentors**  
Francisco Andrés, Cristian Vázquez


**Brief description**  
Frequently, the construction and training of a neural network can be a very complex task when it comes to maintain it. The information that neural networks give us is very important when it has to getting better technology for human beings, for this reason we believe that a good assistant to maintain a neural network will be a Neural Compute Stick 2 to understand the reality that surrounds us. This device acts as a discrete accelerator of neural networks by adding in-deep learning inference capability to current computing platforms to improve performance and efficiency. Robots can readily benefit of this modules by lessening the computational requirements required by DNN. This task will create a RoboComp module that initializes, execute, monitor and publish the results of the USB stick NN hardware module. Examples will include real time object detection and labeling with YOLO and text analysis with PyText.

**Needed skills**  
Python, C++, Qt5, Robocomp

### 10\. Creative new examples to show RoboComp’s core functionality
**Mentors**  
Esteban Martinena, Marco A. Gutiérrez

**Brief description**  
As the community of developers grows, we have detected some problems related to how beginners understand the architecture of Robocomp. Although significant progress has been made in the documentation of all the tools and in the components involved in the development process of Robocomp, the absence of examples that integrate all this knowledge and that allow them to be put into practice makes it difficult to incorporate new collaborators into the community. The aim of this proposal is to design and develop a series of examples of increasing difficulty that integrate the different components, tools and libraries that make Robocomp powerful. This series of examples should guide the beginner in her initiation to Robotics and creation of networks of components. As a consequence of this work, anyone who wants to start contributing to Robocomp will have a quick, global vision of the whole architecture.

**Needed skills**  
Python, C++, Qt5, Robocomp

### 11\. Development of a graphic interface for RoboComp’s code generator: robocompdsl  
**Mentors**  
Esteban Martinena, Ramón Cintas

**Brief description**  
Robocomp is a Robotics framework based on software components. The framework provide the tools to create and modify software components that communicate through public interfaces. Components may require, subscribe, implement or publish interfaces in a seamless way. Building new components is done using a domain specific language CDSL. Robocomp currently have the rocobocompdsl tool to generate and modify components based on this language and files. This slot is aimed to create a GUI for the robocompdsl terminal tool to be able to generate and modify the .cdsl files. It’s a concept similar to the cmake-gui tool. With this new GUI the user will have a visual reference of the options available when generating componentes (interfaces, gui, agm, etc). This also will avoid common mistakes while manual creating or modifying cdsl files. This tool will be a great add to the current tools of Robocomp framework.

**Needed skills**  
Python, Qt5

### 12\. RCManager 2.0: a tool to deploy and monitor large sets of RoboComp components
**Mentors**  
Esteban Martirena, Pablo Bustos

**Brief description**  
Currently RoboComp has a tool to deploy components that is being improved through several GSoC editions. It’s name is RCManager and is used on a daily basis by all the people that use RoboComp to program robots. Since this tool is crucial to the software development process and since robot software is all the time increasing its complexity as a large-scale distributed system, we need to improve this tool as much as we can. 
The first extension is to make the tool access remote RoboComp installations to create a list of potential components to be added to the deployment set.
The second extension tackles the need to group sets of components into higher order entities, so visualization is simplified.
A third extension is to include the capability to probe the edges in the graph of components so a pop-up window would show in real time the traffic moving through it. When connections between components use publish/subscribe modality the probing is easy, but when communication is done using the pull/request modality things get more complicated.

Where to start and what to include in my application?

Run a test with the RCManager tool and understand how it works
Have a look at the tool’s code and check for how to make modifications so a deployment file can be automatically generated in a painless way through the tool
Provide some example of a small modification or improvement in the tool.

**Needed skills**  
Python, Qt5, NetworkX

### 13\. A Natural Language Understanding (NLU) component for RoboComp
**Mentors**  
Pablo Bustos, Pedro Núñez


**Brief description**  
Significant efforts have been carried out in the Human Robot Interaction (MHRI) research field to provide multimodal and user-friendly interactive experiences between users and robots. As between humans, speech is the most natural, simplest and ideal modality to interact with robots using natural language processing technique, in particular when interacting with social robots.

Different Semantic Role Labelling (SRL) systems have developed for their use in different   NLU-based applications. The main purpose of this project is the study of different SRL systems freely available, mainly those based in Deep Learning techniques. The libraries and APIs provided by these systems will be used and will have to be adapted for their use in the RoboComp cognitive robotic architecture.

As a result of the project, a component capable of understanding the natural language of speech input sentences will be developed. The student will also have to evaluate the quality of the semantic representation of knowledge, for the development of future dialogue systems between humans and robots.  

**Needed skills**  
Python, Qt5, RoboComp
 
### 14\. An Automatic Speech Recognition (ASR) component for RoboComp
**Mentors**  
Luis V. Calderita, Pedro Núñez


**Brief description**  
Significant efforts have been carried out in the Human Robot Interaction (MHRI) research field to provide multimodal and user-friendly interactive experiences between users and robots. As between humans, speech is the most natural, simplest and ideal modality to interact with robots using natural language processing technique, in particular when interacting with social robots.  

Different ASR modules have been developed so far for their use in different speech-input based applications. The main purpose of this project is the study of different ASR systems freely available (offline and online). The libraries and APIs provided by these systems will be used and will have to be adapted for their use in the RoboComp cognitive robotic architecture.
  
As a result of the project, a component capable of recognizing the speech of different users will be developed. The student will also have to evaluate the quality of the captured signal and the transcriptions obtained, for the development of future dialogue systems between humans and robots.  

**Needed skills**  
C++, Python, Qt5

### 15\. Storage of the graph-based world representation used in RoboComp

**Mentors**  
Luis V. Calderita, Ramón Cintas

**Brief description**  
Currently RoboComp keeps in real time the state of the robot and the world around it. For this, it uses a graph-based world representation that evolves over time. The aim of this slot is to include a new component that can store the evolution of the robot's world representation. This would allow to keep the history of the actions carried out by the robot with the consequent benefits for analysis, learning and decision making.
In our opinion, the most promising technology to achieve the long-term storage of the robot's world is to use graph databases. Specifically we want to explore the viability of Neo4J for this propose, due to it is one of the best candidates under open source license.

**Needed skills**  
Js, NodeJS, Neo4J, Ice JavaScript, XML, C++

### 16\. Development of a Text To Speech component that operates offline for the EBO educational robot.
**Mentors**  
Iván Barbecho, Marco A. Gutiérrez

**Brief description**  

Our educational robot, EBO, has been endowed with a wide variety of skills related to the perception of its environment. Nevertheless, currently EBO has a limited way to communicate with the outside world. It can express emotions, but it can not verbally interact with a human. This idea aims to endow EBO with the ability to speak. With this objective, a robocomp component will be developed implementing a TTS that works offline and has a beautiful voice. The new component will receive a string and must return or reproduce the generated audio data, depending on the configuration of the component. 
The EBO project is developed in Python, thus knowledge of this programming language is necessary to implement this idea. This way the new component can be easily added to the python package.

**Needed skills**  
Python, Qt5 

### 17\. Design of a Qt3D based simulator for RoboComp:
**Mentors**  
Pablo Bustos, Sparsh Garg

**Brief description**  
Currently Robocomp uses OpenSceneGraph as its scene graph for visual simulations. With this project we want to test Qt3D as an alternative scenegraph for improving 3D robot simulation. Qt 3D has a robust and very flexible material system that allows multiple levels of customization. Also it has modular architecture that’ll help break large software into flexible collaborating modules. And because Qt3D uses ECS rather than inheritance, it is possible to dynamically change how an object behaves at runtime simply by adding or removing components.
Currently, RoboComp’s simulator RCIS is written using the InnerModel kinematic tree representation in connection with OpenSceneGraph, so one of the main goals will be to connect InnerModel to Qt3D bidirectionally such that they have minimum dependency. Testing of the prototype will include the load and simulation of the frequently used worlds and robots in RoboComp.

**Needed skills**  
Qt3D, Qt5, Openscenegraph, C++  
 
### 18\. Text detection, recognition and interpretation using DNNs 
**Mentors**  
Pilar Bachiller, Pablo Bustos

**Brief description**  
Social robots need to be understand their environments and the written text that humans write in them. With the recent release of DNN tools, such as PyText and Senna,  that can analyze the semantic structure of sentences signalling the role of the different elements, the robots can read and access information in the environment that was elusive before. This proposal aims at creating a RoboComp set of components that enable the robots for text reading in real time and during the execution of their daily tasks. Recognition of objects by reading labels and other kind of text annotations will be integrated with other visual recognition modalities such as YOLO object detection to increase the reliability of the process. Several experiments will be run in our ALab facility with our robot Shelly to test the results of the work.

**Needed skills**  
Python, RoboComp, Qt, DNNs
### 19\. Testing and comparison of alternative robotic simulators for RoboComp: Dartsim, V-REP, OpenGym
**Mentors**  
Sparsh Garg, Pablo Bustos

**Brief description**  
RoboComp’s current simulator, RCIS, is based on OpenSceneGraph technology and custom made sensor rendering and actuator simulation. Since its conception in 2005 many other projects have appeared that provide interesting and advanced solutions to the robot simulation problem. In this task we want to to build several prototypes of robotics simulator using open source existing technologies and use their APIs and SDKs to connect them to RoboComp ecosystem. The proposal consist on analyzing several available technologies and code the necessary connectors to RoboComp. Each prototype will be evaluated against the world models and robots currently used in RoboLab.

**Needed skills**  
C++, Python, RoboComp, 3D graphics



## Complete list of Mentors:

### Luis J. Manso

>**l.manso**AT**aston**DOT**ac**DOT**uk**  
Lecturer in Computer Science,  
School of Engineering & Applied Science, Aston University, UK  
[http://ljmanso.com](http://ljmanso.com) __

### Pilar Bachiller

>**pilarb**AT**unex**DOT**es**  
Professor, RoboLab,  
University of Extremadura  

### Ivan Barbecho

>**ibarbech**AT**alumnos**DOT**unex**DOT**es**   
Researcher, Robolab,  
University of Extremadura  

### Pablo Bustos

>**pbustos**AT**unex**DOT**es**  
Professor, RoboLab,  
University of Extremadura  

### Marco A. Gutiérrez

>**marcog**AT**unex**DOT**es**  
Robocomp Developer
  
### Esteban Martinena

>**emartinena**AT**unex**DOT**es**  
Researcher, Robolab,  

### Cristian Vázquez

### Ramon Cintas

>**rcintas**AT**unex**DOT**es**  
Researcher, Robolab,  
University of Extremadura  

### Pedro Núñez

>**pnuntru**AT**unex**DOT**es**  
Professor, RoboLab,  
University of Extremadura  

### Luis V. Calderita

### Araceli Vega

### Francisco Andrés

### Diego R. Faria

>**d.faria**AT**aston**DOT**ac**DOT**uk**  
Lecturer in Computer Science,  
School of Engineering & Applied Science, Aston University, UK  

### Sparsh Garg















