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
