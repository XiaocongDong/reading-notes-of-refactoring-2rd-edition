# Principles in refactoring
## Definition of refactoring
Refactoring can be either a noun a verb.

noun: a change made to the internal structure of software to make it **easier to understand and cheaper to modify without changing its observable behavior**.

verb: to structure software by applying a series of refactorings **without changing its observable behavior**.

## Why do we need refactoring
* People can not come up with a comprehensive design of the system before building it, because the need of the system will likely change as you build the system.
* The internal architecture of the software tends to decay, as people change code to achieve short-term goals, often without a full comprehension of the architecture, the code loses its structure.
* Refactoring makes software easier to understand.
* Refactoring helps finding bugs.
* Refactoring helps programming faster.

## When should we refactor
* Preparatory refactoring - making it easier to add a feature.
* Comprehension refactoring - makeing code easier to understand.
* Litter-pickup refactoring - only refactor a small section of the code when you are doing your daily work.
* Planned and opportunistic refactoring
  * Good developers know that, often, the fastest way to add a new feature is to change the code to make it easy to add.

## Problems with refactoring
* Slowing down new features
  * The most dangerous way that people get trapped is when they try to justify refactoring in terms of "clean code", good engineering practice, or similar moral reasons. The point of refactoring isn't to show how sparky a code base is - it is purely economic. We refactor because it makes us faster - faster to add features, faster to fix bugs. It's important to keep that in front of your mind and in front of communication with others. The economic benefits of refactoring should always be the driving factor, and the more that is understood by developers, managers, and customers, the more of the "good design" curve we'll see.
  
