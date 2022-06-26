James O. Coplien
LeBlanc's Law: later equals never

As clean as possible at all times???
Clean code looks like somebody cares
Ward Cunningham
We don't know absolut right, you don't have to agree with us but you should know our opinion
Literate programming D. Knuth

Use good naming for search purposes
No I in interface?

Instead of many public constructors, make them private and create a static method to access them with meaningful name
var point = Complex. FromReal(23.0); vs
Var poitn = new Complex(23.0);
Consistent lexicon (get fetch retrieve)
Single level of abstraction for functions
Functions should do something or answer something
Instead of commenting, clean your mess
Communication is my first order of business
Dependent function should be close to each other

Rvalues
Different coding style in one project is introducing a complexity to the project

Data structure is opposite to object
Procedural code(using data structure) makes easy to add new functions without changing the data structure, object oriented code makes easy to add new classes without changing existing functions
Hybrids are both a data structure and an object - > try to avoid
Ask whether you need easy add new behavior or adding new data typee

Law of diameter = talk to friends not strangers
Try to write try catch finally blocks first

Checked vs unchecked exceptions? What is true
Provide context with exception as a message
Wrap 3patry API including thrown exceptions
Special Case pattern
Don't return null - > use special case pattern
Don't pass nulls??

Learning tests - > tests of 3party code
Seem?
Adapter VS facade?
Test code is not a second class citizen
Test single concept in one test
Tests should be first(fast independent repeatable self-validating timely
If your tests are not clean your code base will be soon

Many small classes?
Cohesion = maximal when all methods use all fields of the class, minimal when each method uses different fields

AspectJ
Software physics??
Psychological resistance to discard prior effort

Simple is (according to Beck) : runs all tests, no duplications, expresses the intent of the programmer, minimizes the number of classes and methods
Reuse in the small
Care about what you do

Keep your co currency code separate from other code
Learn problems: producer consumer, reader writer, philosopher dining problem
Get your no threaded code working first
Jiggling strategy - > putting some sleeps yields or waits to force concurrency errors

Negatives are slightly harder to understand than positives


Testing minimizes risk
Preemptive threading???
Contest app??

Base class should not know her derivatives
Final keyword is a clutter?? Why to use it?
Java enum jest jak klasa?
Feature envy??

Explaining temporary variables

Test coverage!
Smells an heuristics from clean code znalezc w internecie

Test and build should be done in one step
The principle of least astonishment

Template method vs strategy pattern??
Finite state implementation?? Base class depends on her derivatives??

No clutters (meaningless  artifacts)
Look at your code from reader perspective

Implementation patterns k. Beck
Feet per mile 5280 is absolutely obvious to know:D
Structure over conventions
Hither and yon???
Make a promise to yourself that you will write a clean code

IO bound problems vs processor (computation) bound problems
Use sever based locking instead of client based
Making all methods synchronized doesnt make an object thread safe

Deadlock : mutual exclusion lock and wait no preemption circular wait 