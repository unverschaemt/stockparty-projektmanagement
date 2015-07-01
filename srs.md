# Stock Party Software #
---
## Software Requirements Specification ##
#### For node.JS / node-webkit / RFID ####

*Version 2.2*



## Revision History ##
----
Check this file's history directly on Github.
[SRS Revision History](https://github.com/unverschaemt/stockparty-projektmanagement/commits/master/srs.md)



## Table of Contents ##
---
1. **Introduction**   
1.1 Purpose   
1.2 Scope   
1.3 Definitions, Acronyms and Abbreviations   
1.4 References   
1.5 Overview   
2. **Overall Description**   
2.1 Use-Case Model Survey   
2.2 Assumptions and Dependencies   
3. **Specific Requirements**   
3.1 Functionality   
3.2 Usability   
3.3 Reliability   
3.4 Performance   
3.5 Supportability   
3.6 Design Constrains   
3.7 On-Line User Documentation and Help System Requirements   
3.8 Purchase Components   
3.9 **Interfaces**   
3.9.1 *User Interfaces*   
3.9.2 *Hardware*   
3.9.3 *Software*   
3.9.4 *Communication*   
3.10 Licensing Requirements   
3.11 Legal, Copyright and Other Notices   
3.11.1 *Dependencies*   
3.12 Applicable Standards   
3.2 Supplementary Requirements   
4. **Supporting Information**   


# Software Requirements Specification #

## 1.  Introduction ##
---
This project should provide a tool to run a so called "Stock Party".
On a "Stock Party" all the prices are calculated by demand and supply. To offer an easy and fast way to pay drinks we will realize a RFID cash system. It will be possible to charge these cards and to pay with them on the bar.
This webapp will implement the whole cash system and also a stock monitor as well as an admin panel. Furthermore there will be a alcohol sensor where the party guest can measure there alcohol level. To provide an interface for the RFID reader there will be a JS Driver developed which communicates with our node.js web client.

## 1.1  Purpose ##
---
### Desktop-Application ###
The desktop-application includes following sub-applications.

### Cash-Register ###
• Buy Drinks
People are able to choose drinks from a fixed drink-list and the specific amount they want, the software then calculates the price and handles the communication with the RFID card

• Charge Card
To pay a drink each customer needs to charge his card in order to pay for drinks

• Stockcrash
Should set all prices to minimum

### Admin-Panel ###
• Configuration/Installation
Setup settings, calibration of the alcohol sensor

• Manage Drinks
Interface to add or remove drinks, aswell as mark sold out drinks

• Settings
Basic settings just as the refresh intervall, options to change the algorithm and the stock behaviour, layout settings for font size, the graph and much more

• Statistics
Statistics for the party host, should show average prices of drinks, total amount of bought drinks and other useful statistics


### Graph/Price-Monitor ###
• Show Graphs
Time/Price Graph (*shows current price for each drink in a stock-like graph*)
Time/Alcohol-Level Graph (*shows average alcohol level in a graph*)

• Current Price-List (*shows current price for each drink in a list for the customer to better see the current price*)

### Alcohol-Tester ###
• Detects your Alcohol level (*connect sensor to web client, needs to implement an interface, most likely with a serial port adapter developed*)

• Optionally saves alcohol level to personal database record (*for a personal statistic each one can see on the associated smartphone app*)

### Features that we would like to implement if we have enough time ###
• Open API
Provide an API for other project to communicate with our software (*f.e schedule our party*)
Only sell alcohol to persons that are over 16/18 (*detection via RFID card ID*)
Communicate with other **Stock Party**'s that happen at the same time

## 1.2 Scope ##
---
[Use Case Report](https://github.com/unverschaemt/stockparty-projektmanagement/blob/master/useCaseReport.pdf)

## 1.3  Definitions, Acronyms and Abbreviations ##
---
**RFID** = Radio Frequency Identification   
**UX** = User Experience


## 1.4  References ##
---
[Use Case Report](https://github.com/unverschaemt/stockparty-projektmanagement/blob/master/useCaseReport.pdf)   
[Use Cases](https://github.com/unverschaemt/stockparty-projektmanagement/blob/master/useCases.pdf)   
[StockParty Network](http://s533994975.online.de/se-data/stockpartyNetwork.pdf)    
[database schema](https://github.com/unverschaemt/stockparty-projektmanagement/blob/master/databaseSchema.pdf)   
[Add Drinks](https://github.com/unverschaemt/stockparty-projektmanagement/blob/master/useCases/addDrinks.md)    
[Remove Drinks](https://github.com/unverschaemt/stockparty-projektmanagement/blob/master/useCases/removeDrinks.md)    
[Choose Client](https://github.com/unverschaemt/stockparty-projektmanagement/blob/master/useCases/chooseClient.md)    
[Pay Drinks](https://github.com/unverschaemt/stockparty-projektmanagement/blob/master/useCases/payDrinks.md)    
[Stock Crash](https://github.com/unverschaemt/stockparty-projektmanagement/blob/master/useCases/stockcrash.md)    
[Enable Party](https://github.com/unverschaemt/stockparty-projektmanagement/blob/master/useCases/enableParty.md)

[Loading Of Cards](https://github.com/unverschaemt/stockparty-projektmanagement/blob/master/useCases/loadingOfCards.md)    
[Manage Hardware Interfaces](https://github.com/unverschaemt/stockparty-projektmanagement/blob/master/useCases/manageHardwareInterfaces.md)    
[Show Graph](https://github.com/unverschaemt/stockparty-projektmanagement/blob/master/useCases/showGraph.md)      


## 1.5 Overview ##
---
This SRS gives an overview of our project "**Stock-Party**" which includes goals, required features and technologies being used.

## 2.  Overall Description ##
---
Here the Use-Case-Model is described and the requirements are specified.

## 2.1 Use-Case Model Survey ##
---
The Use-Case-Model contains two systems: **See 1.1**!

[Use Case Report](https://github.com/unverschaemt/stockparty-projektmanagement/blob/master/useCaseReport.pdf)    
[Use Cases](https://github.com/unverschaemt/stockparty-projektmanagement/blob/master/useCases.png)

## 2.2 Assumptions and Dependencies ##
---
• node.JS   
• JavaScript   
• C   
• RFID   
• Socket.IO   
• Mocha   
• JIRA   
• Bamboo   
• BitBucket   


## 3. Specific Requirements ##
---
[StockParty Network](http://s533994975.online.de/se-data/stockpartyNetwork.pdf)


## 3.1 Functionality ##
---

[UML Class Diagram Server](http://unverschaemt.net/stockparty/Class%20Diagram.html)   
[UML Class Diagram Client](http://unverschaemt.net/stockparty/Class%20Diagram%20Client.html)


[Use Case Report](https://github.com/unverschaemt/stockparty-projektmanagement/blob/master/useCaseReport.pdf)   
[Use Cases](https://github.com/unverschaemt/stockparty-projektmanagement/blob/master/useCases.png)   


**Use Case Specifications**   
[Add Drinks](https://github.com/unverschaemt/stockparty-projektmanagement/blob/master/useCases/addDrinks.md)   
[Remove Drinks](https://github.com/unverschaemt/stockparty-projektmanagement/blob/master/useCases/removeDrinks.md)   
[Pay Drinks](https://github.com/unverschaemt/stockparty-projektmanagement/blob/master/useCases/payDrinks.md)   
[Stock Crash](https://github.com/unverschaemt/stockparty-projektmanagement/blob/master/useCases/stockcrash.md)   
[Choose Client](https://github.com/unverschaemt/stockparty-projektmanagement/blob/master/useCases/chooseClient.md)   
[Enable Party](https://github.com/unverschaemt/stockparty-projektmanagement/blob/master/useCases/enableParty.md)   

[Loading Of Cards](https://github.com/unverschaemt/stockparty-projektmanagement/blob/master/useCases/loadingOfCards.md)   
[Manage Hardware Interfaces](https://github.com/unverschaemt/stockparty-projektmanagement/blob/master/useCases/manageHardwareInterfaces.md)   
[Show Graph](https://github.com/unverschaemt/stockparty-projektmanagement/blob/master/useCases/showGraph.md)   


## 3.2 Usability ##
---
**Browser**
The application runs in a browser which is common to nearly all users. We also try to provide a great UX so it will be easy for the users to use our software.

**Smartphone App**
As an addition we provide a smartphone application for the party guests. Most of the people today are used to work with smartphone applications.

**Internationalization**
The application will be both english and german which provides a great way for all users to understand the content of our software.

## 3.3 Reliability ##
---
The server is hosted by 1&1, one of the main companies in Germany when it comes to hosting. Therefore we expect a good uptime of our servers.

Thanks to the detailed documentation we also will provide high quality code which leads to a software with less bugs and therefore with a great reliability.
## 3.4 Performance ##
---
Our requirement concerning the performance of our application is that no user recognizes any latency of our application. That means we don't accept any latency longer than 100 Milliseconds. (Except Internet Connections)
## 3.5 Supportability ##
---
NodeJS and Javascript in general are standards in the web development. Because of that long term support is promised.
## 3.6 Design Constrains ##
---
**Technologies**   
JavaScript   
RFID   
Arduino   

**Frameworks & Compiler**   
Angular.js   
Node.js   
Socket.io   
node-webkit   
Mocha   

**Development Tools**   
Adobe Brackets / Edge Code CC   
Adobe Photoshop CC 2014   
Adobe Illustator CC 2014   
Adobe Inspect CC 2014   
JetBrains Webstorm   
Cyberduck   
Bitbucket   
Webbrowser (*Safari / Chrome*)   
JIRA   
Bamboo   




## 3.7 On-Line User Documentation and Help System Requirements ##
---
There will be a FAQ and a help section for users and a small guide for party administators.
## 3.8 Purchase Components ##
---
RFID-Reader - 13€ (2x)   
RFID-Cards - 0.62€ (10x)   
Shipping - 3€   

## 3.9 Interfaces ##
---
### 3.9.1 User Interfaces  ###

Coming soon
### 3.9.2 Hardware ###
Coming soon
### 3.9.3 Software ###
Coming soon
### 3.9.4 Communication ###
Coming soon
## 3.10 Licensing Requirements ##
Coming soon

## 3.11 Legal, Copyright and Other Notices ##
---
**Copyright 2014 Unverschämt.**
Our project is hosted by bitbucket.org.
It is licensed under the GNU Affero General Public License (AGPL) v3
*for more Information: (http://www.gnu.org/licenses/agpl-3.0.html)*

###3.11.1 Dependencies###

Our dependencies are free and allow commercial usage:

**Node.js**
https://raw.githubusercontent.com/joyent/node/v0.10.32/LICENSE
##3.12 Applicable Standards ##
---
The whole project will adhere stricty to HTML5 Standards.
Also it will be available on all operating systems due to browser compatibility and we plan to add a internationalization to support both a German and an English version.


## 3.2 Supplementary Requirements ##
---
Modular-architecture
API for everything
Simplified design
Gamification
Using an optimized [database schema](https://github.com/unverschaemt/stockparty-projektmanagement/blob/master/databaseSchema.pdf)



## 4. Supporting Information ##
---
Check our [Repository](https://github.com/unverschaemt/stockparty-projektmanagement) or our [Blog](http://blog.unverschaemt.net/) if you have more questions.


1. **Introduction**   
1.1 Purpose   
1.2 Scope   
1.3 Definitions, Acronyms and Abbreviations   
1.4 References   
1.5 Overview   
2. **Overall Description**   
2.1 Use-Case Model Survey   
2.2 Assumptions and Dependencies   
3. **Specific Requirements**   
3.1 Functionality   
3.2 Usability   
3.3 Reliability   
3.4 Performance   
3.5 Supportability   
3.6 Design Constrains   
3.7 On-Line User Documentation and Help System Requirements   
3.8 Purchase Components   
3.9 **Interfaces**   
3.9.1 *User Interfaces*   
3.9.2 *Hardware*   
3.9.3 *Software*   
3.9.4 *Communication*   
3.10 Licensing Requirements   
3.11 Legal, Copyright and Other Notices   
3.11.1 *Dependencies*   
3.12 Applicable Standards   
3.2 Supplementary Requirements   
4. **Supporting Information**   
