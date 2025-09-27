# SW_NOTES
This repository gathers information regarding several SW design, principles and patterns.
Some ideas are compiled from distinguished authors as Donald Knuth, Niklaus Wirth, Kent Beck, Robert C Martin, David Thomas, Andrew Hunt... And some others are my humble opinion

## THINK TWICE BEFORE DOING ANYTHING
This is a premise for any engineer. It is the golden rule.

Before diving into code or desing, take time to consider several approaches to tackle the issue.

## LESS IS MORE


## SW AS A TOOL
Software is just another tool used by engineers to solve problems. A software program, ideally, is created to solve one problem. Therefore, do not create more problems in order to solve one.

As any tool, if it is not used properly the outcome won't be the expected. Always bear in mind what for the program was developed or what you want to achieved when writing it.

Several SW programs (tools) can be used to address a problem, although some fit better than others.

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
>- **Modularity:** A SW program should be composed of different blocks which are combined (think of it as Lego blocks).
>
>   Data, structures and procedures are grouped according to their affinity and purpose. They are almost isolated from each others. Thus, providing a mechanism to test and change them easyly.
>- **Flexibility:** SW should be easy to adapt for modifications and/or new features. This is what *The pragmatic programmer* (#books-of-reference) describes as the **ETC** principle.

In any case, a good design forces us to balance the features, not always is possible or desirable. As said previously, depending on the requirements and the context we should be flexible and take into account the trade-offs.

**When designing there are no  rules, only guidelines. Think twice before doing anything.**

### DIVIDE AND CONQUER
One commonn problem when tackling design is where to begin and the inability to see the whole picture.

It is always a good advice to see the problem as a puzzle. Decompose the problem into smaller pieces, therefore, you would have an easy way to start and a better understanding of the problem itself.

## MODULAR DESIGN

### ORTHOGONALITY

### GENERALIZATION

### INTERFACES


## DRY PRINCIPLE

## SHY CODE
Shy code doesn’t reveal too much of itself to anyone else and doesn’t talk to others any more than is necessary. Shy code keeps to itself. Command-query separation keeps code shy; the caller doesn’t know too much about how its command will be performed.

## REFACTORING
Most of the time it is spent reading code, from others, or even ours.

Refactoring is the natural order of nature in SW. It is essential, as programs grow and requirements change. Also, the fact that with time we gain more knowledge about the system should force us to improve it.
Refactoring is simply rephrasing your code/design to make it better.
It is a daily effort.

## OPTIMIZATION
Only in a few ocassions you should seek for optimization in your program.
Most of the time it is not necessary and any attempt to improve the performance will result in a nightmare. Because, your code will be difficult to maintain, harder to follow, less simple, and/or you will spend time trying to identify the point were a possible optimization could happen.

## FUNCTIONS
One of the basics elements in almost all programming languages. Thus, mastering creation of function is a requirement for any programmer.

Here are some keynotes:
- Functions must do one thing and only one thing. And must do it right! -> I usually consider the SRP principle of functions.
```
/*
 * THIS FUNCTION COMPLIES WITH SRP.
 */
int generateId(void)
{
    return generator->random();
}

/*
 * THIS FUNCTION DOES NOT COMPLY WITH SRP.
 * IT DOES NOT JUST GENERATE THE ID, IT ALSO ASSIGNS IT TO A USER.
 */
void generateId(UserType user)
{
    user.id = generator->random();
}
```
- Functions should keep always the same level of abstraction. This is the principle known as SLAP (SINGLE LAYER ABSTRACTION PRINCIPLE). In here, the idea is that the code is easier to read if the "instructions" are related and at the same level.

- Functions shouldn't be large. How many lines you may wonder, depends as always (there is no rule of thumb).

- In any function the number of parameters should be limited at four (readibility). Group data if necessary.

- Use a verb always to describe the, a descriptive one. Try to be as precise as possible.

## BOOKS OF REFERENCE
| Title | Author(s) |
| :---: |    :---:  |
| The Pragmatic Programmer: Your Journey to Mastery, 20th Anniversary Edition | Andy Hunt, Dave Thomas |
| Clean Architecture: A Craftsman's Guide to Software Structure and Design | Robert C. Martin |
| Structure and Interpretation of Computer Programs | Gerald Sussman, Hal Abelson |
| A Philosophy of Software Design | John Ousterhout |

