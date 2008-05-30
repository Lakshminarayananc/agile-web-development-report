Agile Web Development course, spring 2008
=========================================


Abstract
--------

We organized a thirteen-day Agile Web Development course at Department of Software Systems at Tampere University of Technology in April 2008. The goal of the course was to teach students agile development practices and web programming in a fast-paced project with real customers. 

The daily sessions started at 9:00 each morning and lasted till 16:00, with a one-hour lunch break at the middle of the day. First three days were preparation for the project assignment. On the remaining ten days, lectures and exercises were intertwined with project work. 

Ten students enrolled to the course. Students were divided into five teams of two, with each team working on a separate project. By the end of the course, all teams delivered working software to their customers - albeit without deployment to production use. The customers in general were happy with the results.

We did not achieve all of the educational goals of the course. In particular, test-driven development was planned to be used in project work, but in the end was not. The technical difficulties in learning a new programming language and a new framework were higher than expected. We assessed that mandating test-driven development would cause confusion, frustrate students and interfere with learning.

Feedback from students was very positive.

![Feedback average 4.4 where 5 = very good and 1 = very bad](charts/overall2.png "Student feedback")

We propose that the same course be given next year with a few changes. Most notably, to ease wrestling with technical issues during the project work and to allow more focus on agile programming practices, the course preparation period should be lengthened from three days to five, bringing the total length of the course to fifteen days. We also propose creation of another course "Agile customership", 1 cu.


Introduction
------------

This report describes organizing an Agile Web Development (AWD) course at Department of Software Systems at Tampere University of Technology in April 2008.

In this report, we describe (a) the goals of the course, (b) how the course was structured to achieve those goals, (c) experiences from the actual course implementation, (d) the feedback from students and customers, and finally (e) the changes we propose for the next year's course.


Goals
-----

We had three educational goals.

1. To teach students agile principles.
2. To teach students agile methods in practice. 
3. To teach them programming with a modern web framework.


### Agile principles

Agile principles describe an understanding - or a widely shared opinion - of what is important in software development. They are not unique to agile methodologies. What differentiates agile from traditional software is the stress that agile puts on these principles.

The canonical source of agile principles is the [agile manifesto](TODO). As with any such document, the interpretation of agile manifesto differs from person to person. What follows, is our interpretation of these principles.

The principles we tried to teach students were the following:

* **Minimality**: The price of a project as a function of its requirements grows faster than linearly. Besides requirements, the same holds true with the number of developers, the amount of documentation, and the size of the code base. To maximize the impact we should minimize the size of the project to include just what is needed and nothing more.
* **Change**: Customer's understanding of his own needs are always lacking, and thus requirements will always change. The project should prepare for this change. 
* **Understanding**: Work done without understanding its need leads to trouble. Developer should always understand (a) what he is trying to achieve and (b) why is he trying to achieve it. We can find the root cause by following the chain of whys. The root cause should almost always be "because the customer wants it and we believe it's for the best of the customer". Also, a task done without understanding why it works leads to trouble. Code that "works" is not maintainable if we don't understand how it works.

Combined, there are a few consequences from these principles:

* **Minimality+Change**: Preparation for future grows the project, but may end up outdated. It is very important that plans are lightweight and easily thrown away when outdated.
* **Minimality+Understanding**: There is a need to understand e.g. the domain area, and document that understanding. On the other hand, we want to minimize the amount of documentation. Thus, we should document our understanding in code. The code should always represent our best understanding of the domain area. The code should be viewed as the most important design document for the project.
* **Change+Understanding**: The developers' and customer's understanding of the project area should keep improving throughout the project. Much of this comes from the dialogue between them. Customer should have a concrete understanding of what is the status of the project, and where it is heading. Because the future is very uncertain, the basis for the feedback should be a working prototype of the system. Project iterations should be very short and result in a working software that the customer can evaluate.


### Agile methods

Agile methods are ways to achieve the agile principles in practice. They are important but somewhat meaningless without the understanding of the principles. There is a very large number of different agile methods, which we pruned to a few. The priority of the course was to teach:

* test-driven development (or actually behaviour-driven development)
* scrum project management

In addition to these, the following were planned to be taught if the time would allow:

* continuous integration
* refactoring
* pair programming
* retrospectives

Web programming...


In addition to the educational goals, the course had two other goals: 

1. To test a new kind of a course in the university.
2. To bring experiences from the industry back to the university.




Planned structure
-----------------

* first week: three days preparation
  * first day: Ruby
  * second day: TDD, RSpec
  * third day: Ruby on Rails

* second week: sprint 1
  * first day of project work: planning
  * goals of sprint 1

* third week: sprint 2
  * goals of sprint 2

Implementation
--------------

* student enrollment

* deviance from the plan
  * teaching slower
  * agile part smaller: 1. no TDD 2. Scrum not really Scrum
  * less dialogue with customer

* impressions of student work
  * enthusiasm
  * focus on technical issues
  * two groups: those who were interested in agile and those who weren't. roughly corresponded to Finns-foreigners

* link to course diary

Feedback
--------

* student feedback
  * 

* customer feedback
  * generally satisfied
  * wished 

* feedback from prof Bormann
  * 


Summary
-------

* course was a partial success
  * was beneficial the way it was
  * didn't achieve all goals
  * can be much better

### Proposed changes for next year

* longer course
* course for customers



Appendix
--------

### Origins

The course was modeled after an Agile Web Entwicklung course held at the University of Bremen by prof. Carsten Bormann. In the end there were many differences between the courses. 

The Bremen course is a much more intensive period, consisting of 12 days of 12 hour work, including one weekend. There were two reasons why the intensity of the Bremen course was not emulated in the Tampere course.

* Firstly, such intensity is foreign to the culture at TUT. We feared it would be difficult to attract students to the course. This was later confirmed by student feedback. It could also be difficult to convince the university administration to approve such a course. 
* Secondly, working 12 hour days is opposed to ideals of agile development. Our goal was to teach students sustainable practices that they could later emulate later in their careers.

### Credit units and relation to OHJ-5100 Web programming course

The Agile Web Development course was offered in two ways: (a) as an independent course and (b) in conjunction with OHJ-5100 Web Programming course. The independent course was worth 3 credit points. Passing the independent course required attendance to teaching and finishing the assignment successfully.

In conjunction with OHJ-5100, the course replaced the normal J2EE assignment, two lectures and three weekly exercises of OHJ-5100. The total course credit was 6 credit points: 4 credit points from OHJ-5100 and 2 credit points from 2 credit points from AWD. Passing the two courses required attendance to AWD teaching, successfully finishing the AWD assignment, finishing at least four OHJ-5100 weekly exercises and passing the OHJ-5100 exam.

Of the ten students enrolled to the course, nine took the course in conjunction with OHJ-5100.

