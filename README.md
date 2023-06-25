# Elevator Low Level Design

## Concrete Classes

1. Building
2. Floor
3. Display
4. ElevatorCar
5. InternalButtons
6. ElevatorController
7. ExternalDispatcher
8. InternalDispatcher
9. ElevatorCreator - contains hardcoded data
10. Util - contains utility functions

## Enum Classes

1. Direction
2. Status

## Explanation

1. InternalDispatcher gets triggered by InternalButtons in ElevatorCar. 

2. ExternalDispatcher gets triggered by Floor `pressButton()` function

3. Elevator class contains a `move()` function which is triggered by dispatcher, and it runs a for-loop until it reaches the destination floor.



## Future Enhancement

ElevatorController must implement min. seek time algorithm to effectively co-ordinate with the two elevators.