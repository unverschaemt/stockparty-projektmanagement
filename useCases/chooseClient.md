# Stock Party Software #
---
## Use Case Specification ##
#### Choose Client ####
 
*Version 1.0*   
    


## Table of Contents ##
---
1. **Pay Drinks**         
1.1 Brief Description     
1.2 MockUp       
2. **Flow of Events**    
2.1 Basic Flow     
2.2 Alternative Flows   
3. **Tests**
4. **Special Requirements**    
4.1 Usability              
5. **Preconditions**        
5.1 Connection was successful    
5.2 Login was successful     
5.3 There are clients configured in config  
6. **Postconditions**     
6.1 Client is chosen
7. **Extension Points**


# Use Case Specification Pay Drinks #

## 1.  Pay Drinks ##
---
Pay Drinks    

### 1.1  Brief Description ###
---
After establishing a connection and entering the correct user login the user needs to choose which client he wants to use. A 'client' is in our case a user interface controller which can have differnt grafical or non-grafical (console) user interfaces. The different clients need to be registered before in our config.json file. In this Use-Case the user should get a list of clients which can be chosen and should be able to choose one of them.
### 1.2  MockUp ###
---
![MockUp](https://github.com/unverschaemt/stockparty-projektmanagement/blob/master/useCases/chooseClientMockUp.png)

## 2. Flow of Events Name ##
### 2.1 Basic Flow ###
---
![Choose Client](https://github.com/unverschaemt/stockparty-projektmanagement/blob/master/useCases/chooseClientFlow.jpg)  

### 2.2 Alternative Flow ###
---
n/a    

## 3. Tests
![Choose Client](https://github.com/unverschaemt/stockparty-projektmanagement/blob/master/useCases/chooseClientNarrative.png)
    
## 4. Special Requirements ##
### 4.1 Usability ###
---
The user should be able to choose a client (Cashpanel/Connector/Monitor/Adminpanel) after a successful connection and login. After a client is chosen the according client should be displayed. He or she should do that with as less clicks as possible.

## 5. Preconditions ##
---

### 5.1 Connection was successful ###
The client-side script has successful created a socket.io (WebSocket or XHR-Polling) connection.

### 5.2 Login was successful ###
The user has entered a valid username and password.

### 5.3 There are clients configured in config ###
There is a valid client which can be chosen by the user configured.

## 6. Postconditions ##
### 6.1 Client is chosen ###
---
After the user has chosen a client he should see the chosen client UI (User-Interface).

## 7. Extension Points ##
---
n/a
    