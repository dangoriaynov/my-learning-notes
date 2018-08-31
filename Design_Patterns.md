# Creational
Name | Description | Use case
--- | --- | ---
Simple Factory | Creates an instance of object w/o exposing its instantiation logic | Simplify new object creation
Factory Method | Delegate some method's logic to the child classes | Client choose which log's reporter implementation to use
Abstract Factory | Factory of factories to add some specific logic to the initial factory object | When there are relations between different factories
Builder | Create different flavors of an object w/o constructor's pollution | SQL queries etc.
Prototype | Clonning of the object | When create new is more expensive that to clone
Singleton | Ensures that only 1 object of particular class is ever created |

# Structural
Name | Description | Use case
--- | --- | ---
Adapter | Wrap an otherwise incompatible object to make it compatible | For edge cases and hot-fixes (not good)
Bridge | Prefer composition over inheritance | Each webpage is having a theme, but they are separated as objects and have a separate hierarchy
Composite | Group the same objects in tree structures to treat them at once in the same manner | Calculate salary of all Emp in Org
Decorator | Dynamically change the obj behavior in the runtime by wrapping it in another class | Web auth access restriction
Facade | Simplified interface to a complex system | Hide actions needed to power on the PC when you press only 1 button
Flyweight | Minimize resource usage by sharing to the maximum | Page and resource sharing etc.
Proxy | Wrap object and use its functionality while also provising extra features | Caching or simply a better abstraction from inner logic

# Behavioral
Name | Description | Use case
--- | --- | ---
Chain of Responsibility | Get a chain of objects to get the one suitable for handling | Set of payment methods to use in a shop
Command | Encapsulate actions in objects - decouple client from receiver | Useful when a change history is needed
Iterator | Iterate through elements of the object w/o exposing underlying impl |
Mediator | Decouple objects by introducing thrird-party which is used for their relations | People chat through the ChatRoom
Memento | Store current state of object so that it could be restored later on | Workspace backup in Notepad++ on close
Observer | When object changes the state all its dependencies are notified | Daily email subscriptions (I am the observer in this case)
Visitor | Alter object's actions without re-writing its implementation | Different handlers, anything where commands are supplied as params
Strategy | Control method' behaviour by having logic placed in different classes instead of using if-else | Sorting depending on the set size - strategy is chosen at a runtime
State | Like strategy, but the implementation not the subject itself is supplied as parameter | Caps Lock is changing what each keyboard button is producing
Template Method | Logic is defined in ancestors, but sequence in superclass | Define actions() in sub-class, invoke execute() from super-class

* cudos to https://github.com/kamranahmedse/design-patterns-for-humans
