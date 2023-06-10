# Lecture 6

# the agile manifesto

- individual and interactions over processes
- working software over documentation
- customer collaboration over contract negotiation
- responding to change over following plan

# 1. whole-team approache

- the whole team is responsible for quality in Agile projects.
- the team should be relatively small
- shares the same workspace
- Testers will work closely with both developers and business

# 2. early & frequent feedback

agile projects have short iteration to receive `early` and `continuous` feedback on product quality

> `benefits`
>
> - avoiding requirements misunderstandings
> - clarifing customer feature requests
> - discovering and resolving quality problems early
> - providing information to agle team regrading its productivity

# 3. agile approaches

## 3.1 Aspects of Agile Approaches

- collaborative user story creation
- retrospectives
- continuous integration
- release planning and iteration

> - `extreme programming`
>   - values
>     - communication
>     - simplicity
>     - feedback
>     - courage
>     - respect
>   - practices
>     - collective ownership
>     - continuous integration
>     - small releases
>     - refactoring
>     - test driven development
>     - planning game
>     - pair programming
>     - coding standard
>     - metaphor
>     - sustainable pace
> - scrum
> - kanban

# 4. extreme programming

## 4.1. planning game

- two levels

  1. release planning
     - the team and stakeholders decide what the requirements & features to be into production
  2. iteration planning
     - the team pick up the most valuable items from the list and break them down into tasks to finish at the end of the iteration

- three steps for every level
  1. exploration
  2. commitment
  3. stearing

## 4.2. simple design & refactoring

- code is frequently refactored
- make the 'definition of done' easier.
- conduct a small test or proof-of-concept workout called `Spike`

## 4.3 spike

> a small test or `proof-of-concept` workout that uses the simplest possible program to explore potential solutions

## 4.4. minimum viable product (**MVP**)

- advs
  1. help to breakdown complex modules in a small chunk of code
  2. help to demonstrate the production and focus only on the least amount of work with high priority

> `complete`
>
> cross-functional team in XP releases `Minimum Viable Product (MVP)` frequently.

## 4.5. system metaphor

naming conversion practice used in design and code to have a shared understaing beween teams

## 4.6. pair programming

consists of 2 pragrammers operating on the same code

- `pilot` programmer focuses on clean code, compiles and runs
- `navigator` programmer focuses on the big picture and review code for imporvements

## 4.7. collective code ownership

- no blame game
- no key player

## 4.8. continuous integration (**CI**)

integrate changes every fiew hours or on a daily basis

## 4.9. test driven development

tests are written before code

## 4.10. sustainable pace

it's a slack time (no development activities) during the iteration that acts as a buffer to deal with uncertainties

> `compelete`
>
> Teams can use the `slack time` to pay down `technical debt` by
> refactoring code or do research to keep up the pace.

# 5. scrum

unlike **XP**, does not follow specific techniques or how the testing to be done

# 6. kanban

- objective is to visualize & optimize the flow of work within a value-added chain
- used in
  1. situations where work arrivees in an unpredictable fashion
  2. when you want to deploy work as soon as it's ready
  3. with teams that have a lot of incoming requests

> - `kanban board`
>   - visualize the value chain that will be managed
> - `work in progress (WIP) limit`
>   - the maximum amount of tickets allow for a station or globally for the board
> - `kanban lead time`
>   - the time between a request being mad and a task being released (client wait time for a task to be done)
>   - used to evaluate customer satisfaction
> - `kanban cycle time` (actual work in progress time)
>   - tracks how long task stays in the different process stages
>   - used to measure team performance

# 7. scrum vs kanban

|                     | scrum                                 | kanban                     |
| ------------------- | ------------------------------------- | -------------------------- |
| cadence             | fixed length sprints (2 weeks)        | continuous flow            |
| release methodology | at the end of sprint                  | continuous delivery        |
| roles               | product owner, scrum master, dev team | no required                |
| key metrics         | velocity                              | lead time, cycle time, WIP |
| change philosophy   | no changes during the sprint          | can happen any time        |

# 8. user story

agile form for requirements specifications

- must address the functional and non-functional requirements
- includes acceptance criteria

- `epics`
  - larger collections of related features, or a collection of sub-features that make up a single complex feature
  - include user stories for different development teams

## 8.1 user stories creation techniques

written to capture requirements from the perspectives of developers, testers, and business representatives through `informal review`

### 8.1.1 invest technique

tester may use the invest technique to write effective user stories

- techniquess

  1.  brainstorming
  2.  mind mapping

- `I` => independient
- `N` => nogotiable
- `V` => add value
- `E` => estimatable in time
- `S` => short
- `T` => testable

### 8.1.2 3cs concept

1. `card`
   - phsical media describing a user story
2. `conversation`
   - explains how the software will be used
3. `confirmation`

- the acceptance criteria to confirm that the story is done

# 9 retrospectives

a meeting held at the end of each iteration to discuss what was successful, what can be imporved and how to incorporate it
