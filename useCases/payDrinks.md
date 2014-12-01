# Stock Party Software #
---
## Use Case Specification ##
#### Pay Drinks ####
 
*Version 1.0*   
    


## Table of Contents ##
---
1. **Pay Drinks**         
1.1 Brief Description     
1.2 MockUp       
2. Flow of Events    
2.1 Basic Flow     
2.2 Alternative Flows   
3. Tests
4. **Special Requirements**    
4.1 Usability              
5. **Preconditions**        
5.1 RFID card is recognized     
5.2 There are drinks in the system     
5.3 "shopping basket" shouldn't be empty     
6. **Postconditions**     
6.1 Drink is bought
7. **Extension Points**


# Use Case Specification Pay Drinks #

## 1.  Pay Drinks ##
---
Pay Drinks    

### 1.1  Brief Description ###
---
Drinks can be bought at a cash panel. At a party there can be several cash panels. Each drink which is bought has to be recognized in the system. When an RFID reader is connected to the cash panel a dialogue pops up, when the RFID reader recognizes an RFID card. At this point the current stock prices of the drinks will be paid. In the dialogue drinks can be selected. The customer does not pay at the cash panel. The drinks he buys are saved to the database.  
### 1.2  MockUp ###
---
![MockUp](https://bytebucket.org/stockings/projectmanagement/raw/master/useCases/cashregister.png)

## 2. Flow of Events Name ##
### 2.1 Basic Flow ###
---
![Pay Drinks](https://bytebucket.org/stockings/projectmanagement/raw/master/useCases/payDrinksFlow.jpg)  

### 2.2 Alternative Flow ###
---
n/a    

## 3. Tests
![Pay Drinks](https://bytebucket.org/stockings/projectmanagement/raw/master/useCases/payDrinksNarrative.jpg)
    
## 4. Special Requirements ##
### 4.1 Usability ###
---
The cashier should add and remove drinks easily to the "shopping basket". He or she should do that with as less clicks as possible.

## 5. Preconditions ##
---

### 5.1 RFID card is recognized ###
---
An RFID card of a party member should be recognized from the RFID reader, which is connected to the cash register.

### 5.2 There are drinks in the system ###
There should be drinks in the system, so the cashier can select any.

### 5.3 "shopping basket" shouldn't be empty ###
The cashier should have added at least one drink to the "shopping basket".

## 6. Postconditions ##
### 6.1 Drink is bought ###
---
After the cashier bought drinks, there should be a connection between the party member, who ordered the drinks and the drinks with a timestamp on the database.

## 7. Extension Points ##
---
n/a
    