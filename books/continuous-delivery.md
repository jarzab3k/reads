In the late 90s, I paid a visit to Kent Beck, then working in Switzerland for an
insurance company. He showed me around his project, and one of the interesting
aspects of his highly disciplined team was the fact that they deployed their soft-
ware into production every night.

Software delivers no revenue until it is in the hands of its users. This is obvious,
but in most organizations the release of software into production is a manually
intensive, error-prone, and risky process.

Only when you have control over the progression of
every change from introduction to release can you begin to optimize and improve
the quality and speed of software delivery.

By this we mean that we aim to deliver valuable, working software
to users rapidly and iteratively, working continuously to remove waste from the
delivery process.

Releasing software is too often an art; it should be an engineering
discipline

However, implementing a deployment pipeline is resource-intensive, especially
once you have a comprehensive automated test suite. One of its key objectives
is to optimize for human resource usage: We want to free people to do the
interesting work and leave repetition to machines.

Lean manufacturing has resulted in huge cost and resource
savings, much higher-quality products, and faster time-to-market in several in-
dustries.

So we want to find and fix them at the earliest
possible opportunity, preferably before they are checked in to the code.

In software, when something is painful, the way to reduce the pain is to do it
more frequently, not less.

It should be possible for a new team member to sit down at a new workstation,
check out the project’s revision control repository, and run a single command to
build and deploy the application to any accessible environment, including the
local development workstation.
It should also be possible to see which build of your various applications is
deployed into each of your environments, and which versions in version control
these builds came from.

There is no prize for writing the shortest commit message

Keep binary files independent from configuration information, and keep all configuration information in one
place.

As one of our colleagues, Mike Roberts,
says, “Continuously is more often than you think”

Your build scripts should be treated like your codebase. They should be
tested and constantly refactored so that they are tidy and easy to understand.
It’s impossible to do this with an IDE-generated build process. This gets
more and more important the more complex the project becomes.

Continuous integration is a practice, not a tool

Steve Freeman and
Nat Pryce’s Growing Object-Oriented Software, Guided by Tests, and Gerard
Meszaros’ xUnit Test Patterns: Refactoring Test Code.

Lisa Crispin and Janet Gregory’s Agile
Testing (Addison-Wesley, 2009).

Brian Marick’s paper “When Should a Test Be
Automated?”

This really is
a virtuous circle: Testing at the right time leads to better code.

Mary and
Tom Poppendieck’s book Implementing Lean Software Development: From
Concept to Cash.

Afferent and efferent coupling

First of all, the whole pipeline does not need to be implemented at once. It
should be implemented incrementally.

Finally, your deployment pipeline is a living system. As you work continuously
to improve your delivery process, you should continue to take care of your de-
ployment pipeline, working to improve and refactor it the same way you work
on the applications you are using it to deliver.

Theory of Constraints !!!!

Domain-Specific Languages by Martin Fowler

Make sure you keep all your scripts in a version control repository, preferably the
same one that your source code lives in. It is essential for developers and operations
people to be able to collaborate on build and deployment scripts, and keeping them
in the same repository is what enables this.

It is essential that both build and deployment scripts work on developers’
machines as well as on production-like environments, and that they are used to
perform all build and deployment activities by developers.

When developers have to rely on shared resources in order to run the
application, it is necessarily run much less frequently, and the feedback loop is
much slower. This, in turn, leads to more defects and a slower pace of develop-
ment

“How can
we justify not investing in making the application run locally?”

Your default should be to use relative paths for everything.

Finally, it bears reiterating that scripts are first-class parts of your system. They
should live for its entire life.

Ideally, a commit stage should take less than five minutes to run, and
certainly no more than ten.

If you impose any barriers between the developers
and their ability to get changes made quickly and effectively, you will slow their
progress and store trouble for later

Developers and operations people must feel comfortable with, and responsible
for, the maintenance of their build system.

Use a Build Master for Very Large Teams

Programmers are fairly poor at predicting where the performance bottlenecks in
an application are

Don’t guess; measure.

Never
compromise readability for capacity without an explicit test that demonstrates
the value.

We have discussed
already why scenario-based capacity testing is of importance, but given the much
more common approach of benchmarking specific, technically focused inter-
actions, it is worth reiterating.

Release strategy, release plan

The Unity 3D web player software publishes statistics on its site

Google framework called Protocol Buffers

Even if you have good reasons for not releasing
every change you make—and there are less such reasons than you might
think—you should behave as if you were going to do so.

It is axiomatic that most projects fail due to people problems rather than technical
problems

The deployment system forms an integral part of the application—it should
be tested and refactored with the same care and attention as the rest of the appli-
cation, and kept in version control. When this is not the case (and we have seen
many projects where it is not), the result is always a set of poorly tested, brittle,
and badly understood scripts that make change management risky and painful

In our view, no technology can be considered genuinely enterprise-ready unless
it is capable of being deployed and configured in an automated way. If you can’t
keep vital configuration information in versioned storage and thus manage changes
to in a controlled manner, the technology will become an obstacle to delivering
high-quality results. We have been burnt by this many times in the past.

On one of our projects, we kept a “pain-register,” a diary of time
lost on inefficient technology, which after a month easily demonstrated the cost
of struggling with technology that slowed down delivery.

We recommend Scott Ambler and Pramod Sadalage’s excellent book Refactor-
ing Databases, and the accompanying minibook Recipes for Continuous Database
Integration, for more detail on managing incremental changes to databases.

Dividing an application into a collection of loosely coupled, well-encapsulated,
collaborating components is not only good design. It allows for more effi-
cient collaboration and faster feedback when working on large systems

If different members of the team are working on separate
branches or streams, then by definition they’re not continuously integrating

Indeed, there is a school of
thought that any work on a branch is, in the lean sense, waste—inventory that
is not being pulled into the finished product.

The incremental approach certainly requires more discipline and care—and
indeed more creativity—than creating a branch and diving gung-ho into re-
architecting and developing new functionality. But it significantly reduces the
risk of your changes breaking the application, and will save you and your team
a great deal of time merging, fixing breakages, and getting your application into a
deployable state.

How do you manage large teams of developers
working on multiple releases if you check every change in to mainline? The answer
to this is good componentization of your software, incremental development,
and feature hiding.

If this seems incompatible with making far-
reaching changes to your code, then we humbly submit that perhaps you haven’t
tried hard enough. In our experience, although it may sometimes take longer to
implement a feature as a series of small, incremental steps that keep the code in
a working state, the benefits are immense. Having code that is always working
is fundamental—we can’t emphasize enough how important this practice is in
enabling continuous delivery of valuable, working software.

We have seen even small, experienced,
ninja-level agile teams mess this[branching by feature] pattern up, so there is little hope for the rest of
us.


This last point was so troubling to Nokia that they created a test to evaluate
whether their teams were really doing Scrum. It is divided into two parts.
Are you doing iterative development?
• Iterations must be time-boxed to less than four weeks.2
• Software features must be tested and working at the end of each iteration.
• The iteration must start before the specification is complete.
Are you doing Scrum?
• Do you know who the product owner is?
• Is the product backlog prioritized by business value?
• Does the product backlog have estimates created by the team?
• Are there project managers (or others) disrupting the work of the team?


Dancing with Bears by
Tom DeMarco and Timothy Lister

RELEASE STRATEGY
TESTING STRATEGY

A good starting point to analyze any project is to pose these questions (this
list has worked well for us on several projects):
• How are you tracking progress?
• How are you preventing defects?
• How are you discovering defects?
• How are you tracking defects?
• How do you know a story is finished?
• How are you managing your environments?
• How are you managing configuration, such as test cases, deployment scripts,
environment and application configuration, database scripts, and external
libraries?
• How often do you showcase working features?
• How often do you do retrospectives?
• How often do you run your automated tests?
• How are you deploying your software?
• How are you building your software?
• How are you ensuring that your release plan is workable and acceptable
to the operations team?
• How are you ensuring that your risk-and-issue log is up-to-date?

When confronted with a set of symptoms,
simply behave like a small child and repeatedly ask the team, “Why?” It is rec-
ommended that you ask “Why?” at least five times.

The most common failure mode, by far, is that there is too little
automated testing, not too much.

The commit stage takes too long to run (less than five minutes is ideal, more
than ten minutes is unacceptable).

This is an application of
the principle: “If it hurts, do it more frequently.” We can’t stress enough how important this practice is.