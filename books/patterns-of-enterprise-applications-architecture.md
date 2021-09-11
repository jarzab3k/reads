First approximation around nouns in the domain

Where on x axe my app lies?

ISAM / VSAM files

Patterns are not mutually exclusive
Unit of work 184
Rule of thumb - zasada z palca
Finding object, lepiej obiekt niż statyczna klasa bo wtedy można zamienić zachowanie
W stihlu bardziej by mi się przydała :)
Mixing patterns adds complexity
Beware of a design that looks like a database design
Amount of annoyance is inversely proportional to the amount of the difference
Opisuje rzeczy które duże firmy sprzedają za ogromne pieniądze
Thread scoped registry
Precompiling queries in Influx?
Model view controller - controller = input-controller
Controller is an action
If you aren't familiar with source code control systems you really should not be developing enterprise applications
Two forms of concurrency control - optimistic and pessimistic
Optimistic - conflicts detection
Pessimistic - conflicts prevention
Belt and braces?
Lock escalation

Trade-off errors vs performance 

Applications developers should almost never have to deal with explicit concurrency mechanisms.
Concurrency avoid when possible? - dlaczego mamy osobny proces dla Influx?
Performance test for thread per request VS process per request?
Mała wiara w programistów :) trzymać ich z daleka od wielowątkowości
Singleton vs registry? 
Stateless server to implement stateful session
Distribution by class model does not work-because procedure call between two separate processes is order of magnitude slower 
First law of distributed object design - don't distribute your objects
Dlaczego w Cat całość to nie jedna usługa? 
Sell your favorite grandma first before you make objects distributed 
Distributed object - coarse grained interface local object - fine grained interface
Komunikacja przez pliki tekstowe (xml) tylko jeśli nie ma możliwości komunikacji bezpośrednio miedzyprocesowej
Frodo LOTR : go not to the Elves for counsel for they will say both yes and no
Use book to prod your thinking but don't use it as a replacement for your thinking
Beck extreme programming explained, fowler an essay on continuous integration na jego stronie, beck Test Driven Development by example, fowler refactoring
You match tools to architecture or architecture to tools
Compare layering schemas
Microsoft DNA? 
As few dependencies as possible between the domain model and other parts
Fix the bloating when and if it becomes a problem 
People forget about regular Java objects because they haven't got fancy name that's why POJO:) 
Larman applying UML and Patterns, Fowler Analysis Patterns, gang of four, 
Delegate handling to an object that is most qualified to handle it
Encapsulation is generally a good thing 
Business logic podzielona na dwie: domain logic (faktyczne operacje na danych, na domain model), application logic (workflow logic, informowanie innych bo jakiś stan osiągnięto w domain model) 
Choose your poison:) 
Dobieraj architekturę również do zespołu ludzi których masz dostępnych
Many who are comfortable with sql may not write it well


UML nauczyć się 
Cardinal sin of making fields public
Buy database mapping layer! 
Topological sort
Virtual proxy gang of four 
Remote calls are slow! 
Największy rozdział to object relational structural patterns 
So bear with me
Method object pattern - Beck
UML composition pełny rombik
Make occasional compromise 
Memento pattern
Switch of type to get concrete type - alternative? Dictionary? 
Inheritance mapper- other use cases? 
Interpreter pattern
Scriptlet-laden server? 
Salient point
I think that scriptletcode has the same relationship to well-designed software that professional wrestling has to sport
Template method pattern
Front Controller - nasz Webserver? 
Transform view - easy to test? Dla nas dobry? 
IS mainstream? XSLT
Wiele decyzji zostawił zespołowi, ale często inny zespół decyduje a inny implementuje? 
Hogwash 
Test load your system! 
In Object oriented model the best is to go with small object that have small methods
Interprocess communication Dlaczego to robimy? 
Remote facade-no domain logic i w ogóle fasada! 
Garrulous
Nie bać się podobnego kodu, jeśli tylko można go wygenerować 
Systems clocks are simply to unreliable 
Optimistic offline lock for inconsistent read 
Locking is not just a technical problem
Be sure to implement what suits your needs
Gateway as simple as possible 
Separated interface VS inversion of control
Interface and implementation should be different! 
Hide Singleton pattern Registry.getInstance.foo-registry.foo? 
Multithreading code can drive you to insane asylum 
Divide registers by usage not by implementation 
Any global data is always guilty until proven innocent 
Aliasing bug? 
Ward Cunningham idea of money bag
You should always question your use of accessors
Foemmels conundrum 
Flyweight pattern
Special case w cat? 
Development experience? 
Implicit interface course evil - passing data around in dictionaries 
