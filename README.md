# Eriantys Board Game - 2021/2022

**The project received the maximum score (30L)**

**The application contains Graphical Assets owned by Cranio Creations, if you want to check the repository which contains all the source code ask the project owners**

This project is the final test of **"Software Engineering"** course and it consists in the implementation of the  **[Eriantys]**  board game made by **Cranio Creations**.

<img src="ImagesREADME/Eriantys.png" width=250px height=250 px align="right" />


**Table of contents:**

- [Group Members](#group-members)
- [Implemented Functionalities](#implemented-functionalities)
- [Documentation](#documentation)
	- [UML](#uml)
	- [Communication Protocol](#communication-protocol)
- [Compiling and Packaging](#compiling-and-packaging)
- [Execution Instructions](#execution-instructions)
	- [Server](#server)
	- [Client](#client)

<br/>

---
<br/>

## Group Members 

 - [**Gregorini** Michela](https://github.com/MichelaGregorini) 
 - [**Fiore** Jonathan](https://github.com/JonathanFiore)
 - [**Gallicola** Renato](https://github.com/RenatoGallicola)

<br/>

## Implemented Functionalities
<br/>

| Functionality | Status|
|:---------------:|:----------:|
|Simplified Rules|:white_check_mark:|
|Complete Rules|:white_check_mark:|
|Socket|:white_check_mark:|
|CLI|:white_check_mark:| 
|GUI|:white_check_mark:|
|All Character Cards|:white_check_mark:|
|4 Players Game|:white_check_mark:|
|Multiple Games|:white_check_mark:|
|Persistence|🔴|
|Disconnection Resilience|🔴|

<br/>

The implemented extra functionalities are:
- **All Character Cards**: in the expert mode, all the 12 Character are available.
- **4 Players Game**: the first player can choose to start a game between four players, divided into two teams.
- **Multiple Games**: the Serves can manage multiple games at the same time. This funcionality is implemented as follows:
  - once the client sends a join request to the server, if there's no game created yet, a new one is created and the player is added to that game.
  - if there's a game whose number of players have not been decided yet, the player is added to that game only if they were the second one to join it.
  -  if there's a game whose number of players have already been decided, the player is added only if there is an available slot for that game.
  - in any other case, a new game is created and the player is added to it.

<br/>

## Documentation

In  the  folder  **[deliveries]** there's the project's documentation, complete with: initial and final **class diagrams**, **communication protocol**, sent and received **peer reviews**.

  
### UML

The project's class  diagrams  in  the  Unified  Modelling  Language can be found in the following folders:


-  **[Initial  UML]**

-  **[Final  UML]**



### Communication Protocol

To check the communication protocol ask the project owners.

<br/>

## Compiling and Packaging
The jars are built with Maven Shade Plugin.
To compile the jars, use this command in the project root folder:
```
mvn package
```
The jars will be placed into the folder ```target``` and named ```Client.jar``` and ```Server.jar```.

<br/>

## Execution Instructions

  To get The jars ask the project owners.

  

  ### Server
  To execute the Server, use the following command:
  ```
  java -jar Server.jar
  ```
  
_NB. the Server will open automatically on port number: **12345**_



  ### Client
  To execute the Client, use the following command:
  ```
  java -jar Client.jar
  ```
 
 Then, once the following line is shown: 
 
```
Choose CLI[0] or GUI[1]
```

press ```0``` to play using the CLI or press ```1``` to play using the GUI.

_NB: to properly play using the CLI on Windows, it is necessary to install **[Windows Terminal](https://apps.microsoft.com/store/detail/windows-terminal/9N0DX20HK701?hl=it-it&gl=IT)** , because Windows CMD doesn't support special Unicode characters._

### Pictures:

<img src="ImagesREADME/Img1.JPG" />
<img src="ImagesREADME/Img2.JPG" />
<img src="ImagesREADME/Img4.JPG" />
<img src="ImagesREADME/Img5.JPG" />

  

