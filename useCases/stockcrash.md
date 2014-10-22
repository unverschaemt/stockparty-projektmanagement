# Stock Party Software #
---
## Use Case Specification ##
#### stockcrash ####
 
*Version 1.0*   
    


## Table of Contents ##
---
1. **stockcrash**         
1.1 Brief Description     
1.2 MockUp       
2. Flow of Events    
2.1 Basic Flow     
2.2 Alternative Flows    
3. **Special Requirements**    
3.1 Usability              
4. **Preconditions**        
4.1 active party     
5. **Postconditions**     
5.1 prices should change
6. **Extension Points**


# Use Case Specification stockcrash #

## 1.  stockcrash ##
---
stockcrash

### 1.1  Brief Description ###
---
A stock crash means the prices of all drinks reach the minimum price of the drink. A stock crash can be fired in the adminconsole.   
### 1.2  MockUp ###
---
![MockUp](BILDLINK)

## 2. Flow of Events Name ##
### 2.1 Basic Flow ###
---
[enable stock crash](https://bytebucket.org/stockings/projectmanagement/raw/master/useCases/enableStockcrashFlow.pdf)     

### 2.2 Alternative Flow ###
---
[disable stock crash](https://bytebucket.org/stockings/projectmanagement/raw/master/useCases/disableStockcrashFlow.pdf)     
    
## 3. Special Requirements ##
### 3.1 Usability ###
---
The user should enable and disable a stock crash easily.

## 4. Preconditions ##
---

### 4.1 active party ###
---
The party should run. Otherwise a stock crash makes no sense.

## 5. Postconditions ##
### 5.1 prices should change ###
---

If the stock crash is enabled by the user, all prices should fall to their lowest reachable price with the next refresh intervall. If the stock crash is disabled, the prices should fall and grow calculated by the specific algorithm.

## 6. Extension Points ##
---
n/a
    