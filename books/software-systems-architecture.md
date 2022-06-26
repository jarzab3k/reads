
Www.viewpoints-and-perspectives.info
Stakeholder - people affected by system we need to meet their needs
Viewpoint - tool to structure the architecture
Perspective is for quality properties (performance, security)

What system does and how!
Systems and software engineering - architecture description ISO iec 42010
Define principles of the design and evolution
Every system has an architecture whether or not it is described or understood
Architectural element has responsibility and  boundary and interfaces
Stakeholder is a person that has an interest in the realization of the system
We don't have unlimited time to cover all wishes


4+1 view model
Viewpoints = classes, view = objects


Perspective helps to achieve the quality property

Perspective - safety?

Some stuff you can't avoid, you have to manage it
Architect focus the stakeholders' attention on the important questions and decisions
Identify and ENGAGE stakeholders
Capture and understand concerns
Take ownership of the architecture
Be a lead in the realization of architecture to the real system


Learn the (business) domain


Bashar nuseibeh's twin peaks model
Ta książka to nie jest opis tego co mamy w zaaf?

Architecture definition process stops when you covered the biggest risks which you can understand as no important comments from stakeholders, do it in 1~3 months
Stakeholder - driven process of course!
XP sprawdź
Lean Software programming sprawdź
Concern is problem what why or solution how with what focused

Don't forget business goals and drivers
Concern should be quantified measurable, testable, traceable


Good principle is constructive reasoned articulated testable significant (opposite test should be meaningful ), jargon free language


Stakeholder crieteria: informed committed authorized representative

Stakeholder groups: acquirer(money) , assessor (legal stuff), communicator (marketing), developer, maintainer(docu) , production engineer(devops?) , supplier, support, administrator, tester, user
Proxy Stakeholder
Martin Fowler : models are not right or wrong they are more or less useful
Porównanie modeli z ptolemeuszem kopernikiem newtonem i einsteinem
Model abstracts unnecessary detail
But ommiting details can hidden the problem
Qualitative model
Quantitative model
Skatches
Queueing theory??
Evangelizing or socializing the architecture
ADL
DSL
Abstraction is an act of taking away
Risk driven approach?
To support your decision you should mention the alternatives you've considered
Prioritize your work
Good architecture is correct, sufficient, timelined, concise, clear, current, precise
Introduction and management summary
Stakeholder map
Defining architecture is a continuous process
My language needs to be understandable by the stakeholders
Your model has to have purpose
Scenario based evaluation : architecture tradeoff analysis method by software engineering institute
Skeleton system
TARA tiny architectural review approach
Good recommendation is Clear concise and tact!





Context view!
Assume nothing
SysML
IDL
Interface definition is important!
Acid atomic consistent isolated durable
Eventual consistency
Integration hub open source?
Information quality
Reentrancy = thread safety?
Concurrency model trudno się czyta w książce
Activites vs states? State model VS activity diagram
Michael nygard book 2007
Headroom - dodatkowe możliwości sprzętu na wypadek pikow w użyciu sprzętu
ETL tools extract transform load
Think what could possibly go wrong
Monitor where your system spends time and resources
. Net counters
Back out plan vs backup
Alert starvation vs alert flooding
Do you know what it takes to install your system
DMZ? Network?
Principals use security mechanism that follow policies to access the resources
Security is a process of risk management
CIA concerns - confidentiality integrity availability
Accountability - tracking back to the principal thah did it
Security policy =trust model
Notional cost of risk
Keep security design simple
Fail securely
Information secrecy
Ensure integrity with cryptography?
Security should be in the underlying infrastructure, it should not be part of your application
Don't slow down your users
Throughput VS response time
Predictablity


Latency?
Don't oversimplificate the testing scenario for performance
Optimize where your system spends most of the time
Reduce contention via replication
You don't need do everything during peak hours
Relax transaction consistency
Continually question the validity of your analysis
Indirection (abstraction) vs performance
Measure how long it take to perform ping (nothing)
What would happen if it happened millions times
Mean time between (before) failures (fault)
Mean time to repair
Storage area network?
Log transactions?
Don't assume that something cannot fail in the future
Try to find out when your system is overloaded
Error handling strategy
When you pay for change? When you create a 100% flexible system then at the beginning of the project, but when system is difficult to change then later
How to preserve knowledge?

Estimate the priority of possible change: divide the work of to be done to change something by the estimated time when the change would be needed, eg. 60 - effort to implement, 12 months - when it will be needed, 5 is the piority

Variation points?

Focus on the right dimensions (of the problem)
Design for a change there where probability of a change is high

Confirm scope and external interfaces
Set of software development practices
Avodi refactoring spiral
What I do and how I reduce the risk for my stakeholders?
Documents need to have a customer 