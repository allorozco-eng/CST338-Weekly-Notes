# Week 3 Notes #
<b> Assignments this week: </b>
<br>
• Project 1 Solitaire: Part 2  • Week 3 Learning Journal  • Midterm Prep: Super Maker <br>
• WK03D01: UML and java in general  • WK03D02: Inheritance, statics, and general java

## Design Patterns ##
<b>Topics covered:</b> <br>
• Intro and overview  • Design patterns as reusable  • Focus on the Command Pattern <br>
• Interfaces, inheritance, and abstract classes  • Game programming examples and practical implementation

## What are design patterns? ##
- They are like data structures
- A set of ideas for solving certain problems (Ex. Creational, Behavioral, Structural)
- A simple structure used cleverly is better than a clever structure used simply (Nystrom)
- In other word: A design pattern is a codified mental model

## Command Pattern ##
- The Command pattern turns a method into an object
- The method can then be dynamically changed and shared
### Checklist on implementing Command ###
- Define a command interface with a method signature like execute(), Do(), Activate(), Etc..
- Create one or more derived classes that encapsulates some subset of the following: a "reveiver" obeject, the method to invoke, the arguments to pass.
- Instantiate a Command object for each deferred execution request.
- Pass the Command object from the creator (aka sender) to the invoker(receiver)
- The invoker decides when to execute()
