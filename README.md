# MenusAndEvents

## Delegate Declarations

- DelegateDeclarations.h
- Declare Delegates
  - multicast delegate one param FPointsAddedEvent
  - multicast delegate FGameOverEvent

## EventManager
- EventManager.h
- Declare invokers and listeners for each event
  - Declare an array of the actors of the type that adds points
  - Map each of this actor to its delegate
  - Declare an array of the actors of the type that calls game over
  - Map each of these actors to their delegates
  - Declare functions to add and remove points added event invoker and listener, game over event invoker and listener.
- EventManager.cpp.
  - Implement functions like on teddy bear destruction
 
## FrenchFries Actor
- Actor that Adds points to the game
- FrenchFries.h
  - Declare an instance variable of FPointsAddedEvent delegate type
  - Declare a configuration data actor variable
  - Declare a function to get points added event.
  - Remove invoker when game is finished
 
- FrenchFries.cpp
  - On BEginPlay, add this actor as the invoker of the event in the event manager
    - find all acteors with tag event manager
    - save it to and event manager actor variable
    - Add points added invoker function to this event manager variable
    - save the confifuration data
