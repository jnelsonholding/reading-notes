### Class 04 Reading Notes

## Objects

Objects all have state and behavior. State is like stats in a game. A character might have speed, agility, and perception. Behavior is the action. A character's action would be to run or look around.

In Java, an object's state is contained in fields and its behavior is handled through methods. Methods interact with the objects fields and provide a way to communicate with other objects. Data encapsulation is the act of forcing all interaction with an object's fields to go through its methods.

## Classes

A class provides a way to create an object type. It can be used to make an instance, or many instances, of that object type.

Classes can also be extended for use in multiple subclasses. For instance, the Cat class might have a subclass of LazyCat that can use all of the Cat methods, but also has its own sleepsALot() method. Cat might also have another subclass of HyperCat that does not have the sleepsALot() method but does have makeWideEyesAndRunAround() available.

## Binary and Hexadecimal

Our typical number representation system is Decimal, base 10. It means we have 10 symbols (0,1,2,3,4,5,6,7,8,9) that can be used in one digit position before we need to start using a second digit (10-99).

Binary works the same way, except it's base 2. So we only get to use 2 symbols (0,1) in a digit position before moving to the next digit (10-11). Binary is annoying to write. But it's super handy for computers because the tiny transistors can only be turned on (1) or off (0).

Another handy system for representing numbers is Hexadecimal, base 16. In hexadecimal, we have access to 16 symbols (0,1,2,3,4,5,6,7,8,9,A,B,C,D,E,F) for use in one digit before we need to use a second digit (10-FF). In programming, this is often used to represent numbers that relate to chunks of memory.

[Return to table of contents](../README.md)
