## SOLID: The First 5 Principles of Object Oriented Design

### Single-Responsibility Principle
- A class should have one and only one reason to change, meaning that a class should have only one job.

### Open-Closed Principle
- Objects or entities should be open for extension but closed for modification.
- You should write a class that does what it needs to flawlessly and not assuming that people should come in and change it later.
- It's closed for modification, but it can be extended by, for instance, inheriting from it and overriding or extending certain behaviors. 
- This means that a class should be extendable without modifying the class itself.

### Liskov Substitution Principle
- The liskov substitution principle (lsp) is the one here that is most unique to object-oriented programming. the lsp says, basically, that any child type of a parent type should be able to stand in for that parent without things blowing up.
- This means that every subclass or derived class should be substitutable for their base or parent class.

### Interface Segregation Principle
- The interface segregation principle (isp) says that you should favor many, smaller, client-specific interfaces over one larger, more monolithic interface
- A client should never be forced to implement an interface that it doesn’t use, or clients shouldn’t be forced to depend on methods they do not use.

### Dependency Inversion Principle
- The dependency inversion principle (dip) encourages you to write code that depends upon abstractions rather than upon concrete details
- Entities must depend on abstractions, not on concretions. It states that the high-level module must not depend on the low-level module, but they should depend on abstractions.
- Projects that adhere to SOLID principles can be shared with collaborators, extended, modified, tested, and refactored with fewer complications.


