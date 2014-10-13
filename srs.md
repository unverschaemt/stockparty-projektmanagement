# Stock Party Software #
## Software Requirements Specification ##
### For node.JS / node-webkit / RFID ###
 
*Version 1.0*   
    
 

## Revision History ##
Check this file's history directly on Bitbucket.     
[SRS Revision History](https://bitbucket.org/stockings/projectmanagement/history-node/92b227729475/srs.md?at=master)



## Table of Contents ##
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
3.1 Use-Case Reports     
3.2 Supplementary Requirements      


# Software Requirements Specification #
## 1.  Introduction ##
This project should provide a tool to run a so called "Stock Party".      
On a "Stock Party" all the prices are calculated by demand and supply. To offer a easy and fast way to pay drinks we will realize a RFID cash system. It will be possible to charge these cards and to pay with them on the bar.      
This webapp will implement the whole cash system and also a stock monitor aswell as an admin panel. Furthermore there will be a alcohol sensor where the party guest can measure there alcohol level. To provide an interface for the RFID reader there will be a JS Driver developed which communicates with our node.js web client.      
There might be a feature to commuincate with other stock partys which happen at the same time and to concurrent with them. 

## 1.1  Purpose ##
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

### Smartphone-Application ###
• Show personal History (*shows a history of bought drinks, spend money*)    
    
• Show realtime graph (*shows current price/time graph to see current prices even where you are not at the bar*)    
    
• price notifications (*gives you push notifications when a drink drops under a certain price*)    

### Features that we would like to implement if we have enough time ###
• Open API    
Provide an API for other project to communicate with our software (*f.e schedule our party*)    
Only sell alcohol to persons that are over 16/18 (*detection via RFID card ID*)    
Communicate with other **Stock Party**'s that happen at the same time       

## 1.2 Scope ##
[Use Case Report](https://bitbucket.org/stockings/projectmanagement/src/master/useCaseReport.pdf)    
     
## 1.3  Definitions, Acronyms and Abbreviations ##
**RFID** = Radio Frequency Identification    
     
## 1.4  References ##
[Use Case Report](https://bitbucket.org/stockings/projectmanagement/src/master/useCaseReport.pdf)    
     
[Use Cases](https://bitbucket.org/stockings/projectmanagement/src/master/useCases.pdf)    
     
## 1.5 Overview ##
This SRS gives an overview of our project "**Stock-Party**" which includes goals, required features and technologies being used.     
     
## 2.  Overall Description ##
Here the Use-Case-Model is described and the requirements are specified.    
     
## 2.1 Use-Case Model Survey ##
The Use-Case-Model contains two systems: **See 1.1**!         
     
[Use Case Reort](https://bitbucket.org/stockings/projectmanagement/src/master/useCaseReport.pdf)    
     
[Use Cases](https://bitbucket.org/stockings/projectmanagement/src/master/useCases.pdf)    
     
## 2.2 Assumptions and Dependencies ##
• node.JS   
• JavaScript    
• C    
• RFID     
• Socket.IO    
     

## 3. Specific Requirements ##
[StockParty Network](http://s533994975.online.de/se-data/stockpartyNetwork.pdf)      
     
## 3.1 Use-Case Reports ##
[Use Case Reort](https://bitbucket.org/stockings/projectmanagement/src/master/useCaseReport.pdf)    
     
[Use Cases](https://bitbucket.org/stockings/projectmanagement/src/master/useCases.pdf)    
     

## 3.2 Supplementary Requirements ##
Modular-architecture    
API for everything     
Simplified design     
Gamification    
Using an optimized [database schema](https://bitbucket.org/stockings/projectmanagement/src/master/databaseSchema.pdf)     
