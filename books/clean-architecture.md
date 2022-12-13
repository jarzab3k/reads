Architecture =significant design decisions, significant is measured by cost of change

Architecture is more a journey as destination (like in lean)

The only way to go fast is to go well

Chris Guzikowski

The goal of architecture is to minimize the effort to build and maintain the system

Programowanie się nie zmieniło (metafora z przeniesieniem programisty 50 lat wstecz i odwrotnie)

Making mess is always slower!

Take responsibility for the mess that we made

Redesign (write whole thing again) won't help

Take software architecture quality seriously

If we had wanted the behavior of machines to be hard to change we would have called it hardware!

Programm =functionality +architecture

Importance of architecture over urgency of features

I need to safeguard the software!

True enough

Structure program = forbid the goto

Perfect Encapsulation was in C

Private members in header of c++ only because of the compiler implementation

Oo= any source code dependency can be inverted


Do us much as u can in Immutable components

After 50 years we know what not to do

Program = sequence iteration selection indirection

Single responsibility principle = common closure principle = axis of change

Open closed principle = the most important component should not be dependent on anything

Liskov substitute principles

Interface segregation principle

Dependency inversion principle = never mention the name of anything concrete or volatile

Linia między komponentami może być przecięta tylko w jednym kierunku

Reuse/release equivalence principle = classes that make a component should be cohesive group and together released

Common closure principle = gather into components classes that change for the same reason and at the same time

Common reuse principle = don't force users to depend on thing they don't need


Component Dependency diagram describes map to the build ability and maintainability

Acyclic Dependency principle

The stable Dependency principle

Something is stable when it is hard to change

Stable abstraction principle

Dependencies run in the direction of abstraction

Instability =fan out / (fan out +fan in) [0 1]

Abstractness = number of abstract classes / all classes




Distance from main sequence = |A+I-1|

Software architect is a programmer!

SA cannot do job properly when they don't know what problems they created for a rest of the team


A good SA maximizes the number of decisions not made

Disconnect policy from detail


Leave options open

Be awere of unifying false duplicatations

Decoupling mode = source level, deployment level (dll), service level - jak najdłużej w dll ale tak że zawsze można zrobić service

Draw lines between things that matter and things that dont

Plugin Architecture

Low level components should point to high level components low=blisko wejścia wyjścia high =daleko

Use cases depend on entities (business rule objects)

Frameworks are tools not way of life





Humble object pattern ?

To make boundaries use : skip the last step, strategy pattern, facade

Look for axis of change

Boundaries are important but watch for the cost of implementation

Main as Plugin component

Cucumber tests

Fragile tests Problem

Tests API

Learn what works then make a better solution

Processor abstraction layer

Hardware abstraction layer

Operating system abstraction layer


Letting all code be a firmware is not good long-term, testing only in the target hardware as well



Relationship with Framework is asymmetrical

Authors of framework make no commitment to you

Open arrow - using relationships

Closed arrow - Inheritance relationships

Different reasons corresponds to the actors

Different rates correspond to the levels of policy





The devil is in implementation details
Bob Martin's oo design principles paper?
Object oriented design with applications Grady booch
J. R. Bob dobbs
Architect ing for the enterprise when all you really need is a cute little desktop tool is a recipe for failure


There is nothing new under the sun. 