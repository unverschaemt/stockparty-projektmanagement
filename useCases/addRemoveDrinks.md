# Stock Party Software #
---
## Use Case Specification ##
#### Add / Remove Drinks ####
 
*Version 1.0*   
    
 

## Revision History ##
----
Check this file's history directly on Bitbucket.     
[Add / Remove Drinks Revision History](https://bitbucket.org/stockings/projectmanagement/history-node/92b227729475/srs.md?at=master)



## Table of Contents ##
---
1. **Use-Case Name**         
1.1 Brief Description     
1.2 MockUp       
2. Flow of Events    
2.1 Basic Flow     
2.2 Alternative Flows    
3. **Special Requirements**    
3.1 Usability              
4. **Preconditions**        
4.1 Adding Drinks     
4.2 Removing Drinks     
5. **Postconditions**    
5.1 Adding Drinks    
5.2 Removing Drinks    
6. **Extension Points**


# Use Case Specification Add / Remove Drinks #

## 1.  Use-Case Name ##
---
Add / Remove Drinks

### 1.1  Brief Description ###
---
In the settings of the adminconsole drinks can be added and removed. The added drinks can be sold at the party.     
A drink has the following attributes:
    
• Name    
• Size    
• Minimum Price    
• Maximum Price    
• Start Price / Current Price    
### 1.2  MockUp ###
---
![MockUp](https://bytebucket.org/stockings/projectmanagement/raw/master/useCases/manageDrinks.png)

## 2. Flow of Events Name ##
### 2.1 Basic Flow ###
---
[Add Drinks](https://bytebucket.org/stockings/projectmanagement/raw/90be2c8d8f7ec48bb99f141774a77c4ea28cd397/useCases/addDrinkFlow.pdf)   
[Remove Drinks](https://bytebucket.org/stockings/projectmanagement/raw/90be2c8d8f7ec48bb99f141774a77c4ea28cd397/useCases/removeDrinkFlow.pdf)    

### 2.2 Alternative Flow ###
---
n/a    
    
## 3. Special Requirements ##
### 3.1 Usability ###
---
The user should add and remove drinks with as less clicks as possible.

## 4. Preconditions ##
---
The following conditions are splitted into two subgroups: for adding new drinks and for removing drinks

### 4.1 Adding Drinks ###
---
The drink the user wants to add, should not be in the list already.

### 4.2 Removing Drinks ###
---
There have to be drinks in the system, before you can remove any drinks.

## 5. Postconditions ##
### 5.1 Adding Drinks ###
---

A new drink is registered in the system. That implies, that the cashpanel can choose the new drink to sell. Also a new graph is created for the drink.

### 5.2 Removing Drinks ###
---
After a drink is removed, it is no longer available in the system. That implies the cash register can't choose the drink and you can't see the drink in the graph.

## 6. Extension Points ##
---
n/a
    