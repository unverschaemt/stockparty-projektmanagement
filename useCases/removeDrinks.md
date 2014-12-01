# Stock Party Software #
---
## Use Case Specification ##
#### Remove Drinks ####
 
*Version 1.0*   
    

## Table of Contents ##
---
1. **Use-Case Name**         
1.1 Brief Description     
1.2 MockUp       
2. **Flow of Events**    
2.1 Basic Flow     
2.2 Alternative Flows    
3. **Tests**    
4. **Special Requirements**    
4.1 Usability              
5. **Preconditions**       
6. **Postconditions**    
7. **Extension Points**


# Use Case Specification Remove Drinks #

## 1.  Use-Case Name ##
---
Remove Drinks

### 1.1  Brief Description ###
---
In the settings of the adminconsole drinks can be removed. Removed drinks are not longer available in cashpanels to be sold.
   
### 1.2  MockUp ###
---
![MockUp](https://bytebucket.org/stockings/projectmanagement/raw/master/useCases/manageDrinks.png)

## 2. Flow of Events Name ##
### 2.1 Basic Flow ###
---
![Add Drinks](https://bytebucket.org/stockings/projectmanagement/raw/90be2c8d8f7ec48bb99f141774a77c4ea28cd397/useCases/removeDrinkFlow.jpg)     

### 2.2 Alternative Flow ###
---
n/a

## 3. Tests ##
![Gherkin](https://bytebucket.org/stockings/projectmanagement/raw/master/useCases/removeDrinkNarrative.jpg)
    
## 4. Special Requirements ##
### 4.1 Usability ###
---
The user should add and remove drinks with as less clicks as possible.

## 5. Preconditions ##
There have to be drinks in the system, before you can remove any drinks.

## 6. Postconditions ##
After a drink is removed, it is no longer available in the system. That implies the cash register can't choose the drink and you can't see the drink in the graph.

## 7. Extension Points ##
---
n/a
    