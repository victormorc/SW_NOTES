# SW_NOTES
This repository gathers information regarding several SW design, principles and patterns.
Some ideas are compiled from distinguished authors as Donald Knuth, Niklaus Wirth, Kent Beck, Robert C Martin, David Thomas, Andrew Hunt...

## SW AS A TOOL

## GOOD DESIGN
***A good design could be achieved as a combination of applying several ideas/principles. It always depends on the context, not always the same approach can be used.*** 

In almost all good designs the following features can be identified in them:

> - **Simplicity:** Possibly the hardest thing to achieve in any SW project. It requires a lot of practice and thinking (usually it is not the first idea). Simplicity is avoiding overengineering (less is more). In return it favors changes in the future. It may not sound fancy, but a simple design always pays off.
>
>   [Simple is often erroneously mistaken for easy](https://www.infoq.com/presentations/Simple-Made-Easy/). "Easy" means "to be at hand", "to be approachable". "Simple" is the opposite of "complex" which means "being intertwined", "being tied together". Simple != easy.
>
>- **Clarity:** The following quote is from Donald Knuth "When you write a program, think of it primarily as a work of literature.
>
>   You're trying to write something that human beings are going to read.
>
>   Don't think of it primarily as something a computer is going to follow.
>
>   The more effective you are at making your program readable, the more effective it's going to be: You'll understand it today, you'll understand it next week, and your successors who are going to maintain and modify it will understand it."
>    - **Consistency/Uniformity:** Using the same style helps to favor collaboration. Define processes and standards, thus everybody is aligned and any new member can contribute earlier.
>- **Modularity:** Data, structures and procedures are isolated. 

In any case, a good design forces us to balance the features, not always is possible or desirable. As said previously, depending on the requirements and the context we should be flexible and take into account the trade-offs.

**When designing there are no  rules, only guidelines. Think twice before doing anything.**

## SOLID (OOT - OBJECT ORIENTED TECHNIQUES)

### S - SRP (SINGLE RESPONSABILITY PRINCIPLE)
##### SLAP - SINGLE LAYER ABSTRACTION PRINCIPLE
### O - OCP (OPEN CLOSE PRINCIPLE)
### L - LSP (LISKOV SUBSTITUTION PRINCIPLE)
### I - ISP (INTERFACE SEGREGATION PRINCIPLE)
### D - DIP (DEPENDENCY INVERSION PRINCIPLE)

## DRY PRINCIPLE

## ORTHOGONALITY

## SHY CODE
Shy code doesn’t reveal too much of itself to anyone else and doesn’t talk to others any more than is necessary. Shy code keeps to itself. Command-query separation keeps code shy; the caller doesn’t know too much about how its command will be performed.

## REFACTORING

