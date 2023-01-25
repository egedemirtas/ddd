# DDD

- Patterns on how to reduce and manage the complexity in the software when(or before) developing the system. These patterns are not all technical but also strategic. Some of these are: how to communicate with business analysts, how to cooperate and integrate with other development teams.

- Which methodology, architecture and technologies are the best for software dev? There is no universal "best", the "best" depends on the requirements of the software. The best methodology, achitecture, tech is the ones that can solve the business requirements the best.

- Design is all we need, to decide the best methodology, architecture and technologies in order to solve business requirements. All members (Analyst, developer, achitect, PO, domain expert, UX, test engineer) of the team must paticipate when designing the system. And the final design must be unanimously decided. Developer should know the design when coding so that he won't code with wrong design patterns.

- If an effective design is not made, business requirements won't be met fully.

## The Good Design vs. The Bad Design vs. No Design

- There isn't any "No design". If there is no design, then it is a bad design.

- But a bad design will create a solution that will create more problems in the lifecycle of the software, such as: DB locks, bad UX design, impacting other parts of the system when carrying the code to live.

- Design starts with knowledge acquisition, seeing the big picture will prevent future problems from occuring. methodology, architecture and technologies are just tools for the design, aka the solution, for business requirements. Analogy: business analysts require a road from A to B that will serve any transportaton vehicle. With bad design you can just build a dirt road. But when a customer tries to drive his/her ferrari, the car will get stuck on the road. Lets say you built an asphalt road by taking in the ferrari into consideration. You have even built a gas station just in case any car can get out of fuel. But in 20 years all the cars will be electric, and since you have not left any space for electric charge stations, your design will struggle to meet the requirements. A bad design can also occur from overkill: you might build a avenue, but your company will lose alot of money and resources to maintain this road.

- Good design vs. Effective design: it is much more important to achieve effective design since you want to meet all the present requirements of the business as a priority. You can create a very good design but it might have properties that is aimed to solve problems that will never be encountered.

## Effective Design

- Meets the needs of the business and distinguishes the business from its competition, thus earning a business value.

- What is business value and how to achieve it:

    1. What does the business tries to achieve with this requirement?
    2. What does the business want, what is it trying to solve?
    3. How does this requirement affects the team/company?

- Timelessness: designs should withstand from any changes made in methodology, architecture and technologies. Designs can change if business requirements change.

- Made for specific business domain and compatable with business strategy. Ex: a software you made now serves with certain channels, but strategically these channels will be increased to serve variety of customers in the coming years. If our design does not support these channels, the design will fail.

## DDD in Short

### DDD is About

- Discussion with the business
- Listening the business
- Understanding the business
- Discovering the business
- Generating value to the business

### DDD is Not About

- Software development methodology
- Software architecture
- Technology
- Hardware

## DDD Tools

DDD is a design process:
    - input: business requirements,
    - everyone works on it,
    - a model is created from business requirements by using DDD patterns/tools,
    - output: design/model.
    - The output lets developers to reflect design to the code.

### Strategic Design

- Contains tool sets to form solutions to business requirements. Thus must be done before tactical design.

- Bounded context
  - Explicit context boundry within in which a ubiquitous language is modeled. "Account" in banking context refers to bank account, but in literary context it can be a library account, email account etc.
  - Important because when swithing between different contexts.
  - Domain experts
- Ubiquotious language
  - language used in requirement document, scenarios, cases. Language shared by the team, developers, domain experts, and other participants so that there are no ambiguity. This ubiquotious language will be directly reflected to the code.
  - Every bounded context might have its own ubiquotious language.
  - Can contain: concepts, actions, constraints, personas.
- Context mapping
- Sub domains

### Tactical Design

- The part where developers reflect the model/design to the code. If the design is faulty, the code will be faulty.
- Aggregates
- Entities
- Value objects
- Domain events
