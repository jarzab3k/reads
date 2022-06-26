Carnegie, Dale. How to Win Friends and Influence People, Revised Edition. New York,
NY: Pocket Books, 1981.

For any project attribute, it’s possible to measure that attribute in a way that’s superior
to not measuring it at all

If there’s no heartbeat, the project is dead. (about building daily)

Gilb, Tom. Competitive Engineering. Boston, MA: Addison-Wesley, 2004. May be downloaded from website

Dale Carnegie’s How to Win
Friends and Influence People

Measure anything is better than do nothing

Against this backdrop, daily builds enforce discipline and keep pressure-cooker
projects on track

When you hear a tool vendor claim “This new tool will eliminate computer program-
ming,” run!

The smaller part of the job of programming is writing a program so that
the computer can read it; the larger part is writing it so that other humans can read it.

The bottom line
is that the details of a specific method of structuring a program are much less impor-
tant than the fact that the program is structured consistently.

until you’ve measured performance gains, you’re better off striving for
clarity and correctness first, performance second.

In well-written code, comments are the icing on the readability cake.

Performance is not a good reason to avoid commenting

The number of comments, however, will be a side
effect of the process itself. Rather than focusing on the number of comments, focus on
whether each comment is efficient.

Styles that are hard to maintain aren’t
maintained

s Kernighan and Plauger emphasize, “Don’t document bad code—
rewrite it” (1978

Coding conventions should
encourage good practices; heavy routine headers do the opposite.

follow the Principle of Proximity and put comments as close as possible to
the code they describe. They’re more likely to be maintained, and they’ll continue to
be worthwhile.

Personal character has received a rare degree of attention in software development.
Ever since Edsger Dijkstra’s landmark 1965 article, “Programming Considered as a
Human Activity,”

Your employer can’t force you to be a good programmer; a lot of times your employer
isn’t even in a position to judge whether you’re good. If you want to be great, you’re
responsible for making yourself great.

The purpose of many good programming practices is to reduce the load on your gray
cells

Conceptual Blockbusting
(2001).

: “Look. This is how much it’s
going to cost. I can’t say whether it’s worth this price to the company—that’s your job.
But I can tell you how long it takes to develop a piece of software—that’s my job. I can’t
‘negotiate’ how long it will take; that’s like negotiating how many feet are in a mile.
You can’t negotiate laws of nature. We can, however, negotiate other aspects of the
project that affect the schedule and then reestimate the schedule. We can eliminate
features, reduce performance, develop the project in increments, or use fewer people
and a longer schedule or more people and a shorter schedule.”

keep the person who has to modify your code in mind.
Programming is communicating with another programmer first and communicating
with the computer second.

Don’t waste your creativity on things that don’t matter. Establish conventions in non-
critical areas so that you can focus your creative energies in the places that count.

Dijkstra, Edsger. “The Humble Programmer.” Turing Award Lecture. Communications
of the ACM 15, no. 10 (October 1972): 859–66

In general, attacking what Chapter 5 describes as “accidental difficulties” wher-
ever possible.

Dogmatic methodologies and high-quality software development don’t mix. Fill
your intellectual toolbox with programming alternatives, and improve your skill
at choosing the right tool for the job.

35.4 A Software Developer’s Reading Plan

35.5 Joining a Professional Organization 

Construction is the only activity that is guaranteed to be done

Never think that one technology or methodology would solve 100% of your problems

Measure twice, cut once

This phenomenon is known as the WISCA or WIMP syndrome: Why Isn’t Sam Cod-
ing Anything? or Why Isn’t Mary Programming

Part of your job as a technical employee is to educate the nontechnical people around
you about the development process.

Architektur vs Design

Stable requirements are holy grail of software development

If you're not heading right direction then stop and check

Evolutionary delivery?

If you can't explain something to six year old you really don't understand it yourself -> A. Einstein

Threat model

The architecture should say whether we implement simplest possible solution or should tend to be overengineered

Most likely changes should be the easiest to implement

Essential problem with large systems is maintaining their conceptual integrity (brooks 1995)

Boehm Barry Richard Turner balancing agility and discipline a guide for the perplexed


Avoid variations in code so you can concentrate on a problem

Wave of technology has influence in your time doing stuff

Brooks no Silver bullets essence and accidents os software engineering 

Managing complexity!!! - reduce load on your brain, you should have small independent parts of the system so you think only about that part not the whole system

Encapsulation picks up where abstraction leaves off. Abstraction says, “You’re allowed
to look at an object at a high level of detail.” Encapsulation says, “Furthermore, you
aren’t allowed to look at an object at any other level of detail.”
encapsulation helps to manage complexity by forbidding you
to look at the complexity

David Par-
nas in 1972 called “On the Criteria to Be Used in Decomposing Systems Into Mod-
ules.

Information hiding emphasizes hiding complexity.

Hiding complexity so that your brain doesn’t have to deal with it unless you’re
specifically concerned with it

What should I hide

Connection between modules as simple as possible! 

Classes and routines are first and foremost intellectual tools for reducing complexity.
If they’re not making your job simpler, they’re not doing their jobs.

Draw a diagram

Prototype with discipline = it is a throwaway code, don't forget that 

Class responsibility collaborator cards (crc cards) is it worth anything? 

The art of unix programming, Raymond Eric s 2004

Is relation test for inheritance = is my class a base class, eg. Is an EmployeeCensus a ListContainer (when EmployeeCensus :ListContainer) 

Complexity is how much code you have to think about at one single moment 

Very important!!!:

If you can’t figure out how to use a class based solely on its interface documentation,
the right response is not to pull up the source code and look at the implementation.
That’s good initiative but bad judgment. The right response is to contact the author of
the class and say “I can’t figure out how to use this class.” The right response on the
class-author’s part is not to answer your question face to face. The right response for
the class author is to check out the class-interface file, modify the class-interface doc-
umentation, check the file back in, and then say “See if you can understand how it
works now.” You want this dialog to occur in the interface code itself so that it will be
preserved for future programmers. You don’t want the dialog to occur solely in your
own mind, which will bake subtle semantic dependencies into the client code that
uses the class. And you don’t want the dialog to occur interpersonally so that it bene-
fits only your code but no one else’s. 

Be critical about classes that contain more than 7 data members (7 +-2 rule)

Functional cohesion 

C is weak typed?? 

The most important reason for creating a routine is to improve the intellectual
manageability of a program, and you can create a routine for many other good
reasons. Saving space is a minor reason; improved readability, reliability, and
modifiability are better reasons.

Use error-handling code for conditions you expect to occur; use assertions for
conditions that should never occur

Robustness VS correctness 

Consider building a centralized exception reporter 

We forget that coding is not trivial task! 

95 % of errors are coused by the programmers themself 5 % by operating system, hardware, compilers etc.. 

Hacking compiling and fixing is not a way to programm a working software 

High quality programming is an iterative process 

Hybrid coupling 

You should not need to figure out code, you should be able to read it! 

Avoid numerals in names, use arrays instead

Count or index instead of num

Code is read much more times than written 

Internationalization and localization as soon as possible 

Truly soft= easy to work with and change

Dog tag for pointers a

Code should be read not figured out

Tramp data

Loop with exit! 

If Statement always first with the main workflow 

Break in the if statement??! 

The language you use to solve the problem substantially affects your solution 

Computer science books aren't doing the world any favors with their examples of recursion 

Dijkstra goto statement considered harmful 1968

D. Knuth structured programming with goto statements 1974

If you have your rain boots on, it’s not worth walking around the block to avoid a mud puddle.

Table driven methods!!!!!!! - > instead of complicated logic or complicated inheritance, see also stair step access table

As Butler Lampson, a distinguished engineer at Microsoft, says, it’s better
to strive for a good solution and avoid disaster rather than trying to find the best solu-
tion (Lampson 1984).

More generally, complicated code is a sign that you don’t understand your program
well enough to make it simple

Decisions point-one per if while for and or
10+ is a warning sign

 The organization must show programmers that quality is a priority. Making
the quality-assurance activity explicit makes the priority clear, and programmers will
respond accordingly.

Different people find different errors

General principle of software quality = proving quality reduces development costs

Software standards can be written and distributed but if no one talks about them, they won't be followed. 

Try to hope that you find an error in your code, it's better than somebody else would find it. 

Mature testing organizations tend to have five dirty tests for every clean test

Measure where the errors occur measure your test results! 

Kaner testing computer software 1999

Extreme programming and flexible process software engineering xp2000 conference, endo testing unit testing with mock objects, Steve freeman 

Tramp data

Programmers are notoriously bad at guessing what functionality might be needed some day

Before you invest time solving a performance problem make sure that you're solving a problem that needs to be solved

The part that needs to be perfect is usually small

Sedgewick algorithms in....

Jam loops