Knowledge crunching

As written, it is unlikely that any business expert could read this code to verify the rule, even
with the guidance of a developer.

Knowledge crunching is an exploration, and you can't know where you will end up.

The terminology of day-to-day discussions is disconnected from the terminology
embedded in the code (ultimately the most important product of a software project).
And even the same person uses different language in speech and in writing, so that the
most incisive expressions of the domain often emerge in a transient form that is never
captured in the code or even in writing.
Translation blunts communication and makes knowledge crunching anemic.

The Language Instinct, by Steven Pinker

Play with the model as you talk about the system. Describe scenarios out loud using the
elements and interactions of the model, combining concepts in ways allowed by the
model. Find easier ways to say what you need to say, and then take those new ideas
back down to the diagrams and code.

If sophisticated domain experts don't understand the model, there is
something wrong with the model.

It leads us toward simplified diagrams of conceptually important parts
of the object model that are essential to understanding the design. The diagrams in this book are
typical of those I use on projects. They simplify, they explain, and they even incorporate a bit of
nonstandard notation when it clarifies their point. They show design constraints, but they are not
design specifications in every detail. They represent the skeletons of ideas.

Always remember that the model is not the diagram.

It takes fastidiousness to write code that doesn't just do the right thing but also
says the right thing.

Tightly relating the code to an underlying model gives the code meaning and makes the model
relevant.

Development
becomes an iterative process of refining the model, the design, and the code as a single activity

Manufacturing is a popular metaphor for software development. One inference from this
metaphor: highly skilled engineers design; less skilled laborers assemble the products. This
metaphor has messed up a lot of projects for one simple reason—software development is all design. 

Programmers are modelers,
whether anyone likes it or not. So it is better to set up the project so that the programmers do
good modeling work.

This decoupling is important not because projects
frequently need to replace user interfaces with wire requests but because a clean separation of
concerns keeps the design of each layer easy to understand and maintain.

It is not practical to achieve that correspondence when the domain logic is mixed with other
concerns of the program. Isolating the domain implementation is a prerequisite for domain-driven
design.

Generating such an ID may require techniques that are beyond the scope of
this book. The goal here is to point out when the considerations arise, so that developers are
aware they have a problem to solve and know how to narrow down their concerns to the critical areas.

The goal of domain-driven design is to create better software by focusing on a model of the
domain rather than the technology. By the time a developer has constructed an SQL query,
passed it to a query service in the infrastructure layer, obtained a result set of table rows, pulled
the necessary information out, and passed it to a constructor or FACTORY, the model focus is gone.
It becomes natural to think of the objects as containers for the data that the queries provide, and
the whole design shifts toward a data-processing style. The details of the technology vary, but the
problem remains that the client is dealing with technology, rather than model concepts.
Infrastructure such as METADATA MAPPING LAYERS (Fowler 2002) help a great deal, by making easier
the conversion of the query result into objects, but the developer is still thinking about technical
mechanisms, not the domain. Worse, as client code uses the database directly, developers are
tempted to bypass model features such as AGGREGATES, or even object encapsulation, instead
directly taking and manipulating the data they need. More and more domain rules become
embedded in query code or simply lost. Object databases do eliminate the conversion problem, but
search mechanisms are usually still mechanistic, and developers are still tempted to grab whatever
objects they want.

The sheer
technical complexity of applying most database access infrastructure quickly swamps
the client code, which leads developers to dumb down the domain layer, which makes
the model irrelevant.

Client Code Ignores REPOSITORY Implementation; Developers Do Not!!!!

They [domain models] are seldom developed except through an iterative process of refactoring, including
close involvement of the domain experts with developers interested in learning about
the domain.

True, in a $100 million (MM) deal, no one cares about where
the extra pennies go, but bankers don't trust software that cannot meticulously account for those
pennies.

Read the book

Specification domain pattern

If a developer must consider the implementation of a component in order to use it, the
value of encapsulation is lost

INTENTION-
REVEALING INTERFACES.

With each decision, ask yourself, "Is this an expedient based on a particular set of
relationships in the current model and code, or does it echo some contour of the underlying
domain?"

It is more useful to make a big impact on one area, making a part of the design really supple, than
to spread your efforts thin

SIDE-EFFECT-FREE FUNCTIONS.

A design pattern should be applied
only when it is needed.

If you wait until you can make a complete justification for a change, you've waited too long. Your project is already incurring heavy costs, and the postponed changes will be harder to make
because the target code will have been more elaborated and more embedded in other code.
Continuous refactoring has come to be considered a "best practice," but most project teams are
still too cautious about it. 

Software development is not such a
predictable process that the benefits of a change or the costs of not making a change can be
accurately calculated.

Don't be absolute about things, but push
beyond the comfort zone in the direction of favoring refactoring.

Given that it isn't feasible to maintain a unified model for an entire enterprise, we don't have to
leave ourselves at the mercy of events

Bounded context!

Most Agile projects have at least daily merges of each developer's code changes.

"George's team's stuff is changing, so we're going to have to
change our stuff that talks to it." Say instead, "The Transport Network model is changing, so we're
going to have to change the translator for the Booking context."

If we are building a new system, we will
typically believe that our new model is the best available, and so we will think in terms of translating
directly into it. 

The harsh reality is that not all parts of the design are going to be equally refined.
Priorities must be set. To make the domain model an asset, the model's critical core has
to be sleek and fully leveraged to create application functionality. But scarce, highly
skilled developers tend to gravitate to technical infrastructure or neatly definable
domain problems that can be understood without specialized domain knowledge.

One of the most successful projects I've joined initially suffered from this syndrome. The goal was
to develop a very complex syndicated loan system. Most of the strong talent was happily working
on database mapping layers and messaging interfaces while the business model was in the hands
of developers new to object technology.

The planning process must drive resources to the most crucial points in the model and design. To
do that, those points must be identified and understood by everyone during planning and
development.

One way or another, creating distinctive software comes back to a stable team accumulating
specialized knowledge and crunching it into a rich model. No shortcuts. No magic bullets.

Write a short description (about one page) of the CORE DOMAIN and the value it will
bring, the "value proposition." Ignore those aspects that do not distinguish this domain
model from others.

This is a net gain, because the greatest value-added of
enterprise software comes from the enterprise-specific aspects of the model.

Each structural rule should make development
easier.

Are the developers knowledgeable about the domain? Are they interested in the domain?

nteresting" problems. And there is prestige attached to being a member of an elite team.
These forces often leave behind only the least technically sophisticated developers to actually build
applications. But building good applications takes design skill; this is a setup for failure. Even if a
strategy team creates a great strategic design, the application team won't have the design
sophistication to follow it.

A good project has lots of people sticking their
nose in other people's business. Developers play with frameworks. Architects write application
code. Everyone talks to everyone. It is efficiently chaotic. Make the objects into specialists; let the
developers be generalists.

. in practice master plans fail—because they create totalitarian order, not organic order.

Alexander and his colleagues advocated instead a set of principles for all community members to
apply to every act of piecemeal growth, so that "organic order" emerges, well adapted to
circumstances. 
