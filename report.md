Experiences from Agile Web Development course, spring 2008
==========================================================

Antti Tarvainen, June 1, 2008


Abstract
--------

We organized a thirteen-day Agile Web Development course at Department of Software Systems at Tampere University of Technology in April 2008. The goal of the course was to teach students agile development and web programming in a fast-paced project with real customers. 

The daily sessions started at 9:00 each morning and lasted till 16:00, with a one-hour lunch break at the middle of the day. First three days were preparation for the project assignment. On the remaining ten days, lectures and exercises were intertwined with project work. 

Ten students enrolled to the course. Students were divided into five teams of two, with each team working on a separate project. By the end of the course, all teams delivered working software to their customers - albeit without deployment to production use. The customers in general were happy with the results.

We did not achieve all of the educational goals of the course. In particular, test-driven development was planned to be used in project work, but in the end was not. The technical difficulties in learning a new programming language and a new framework were higher than expected. We assessed that mandating test-driven development would cause confusion, frustrate students and interfere with learning.

Feedback from students was very positive.

![Feedback average 4.4 where 5 = very good and 1 = very bad](charts/overall2.png "Student feedback")

We propose that the same course be given next year with a few changes. Most notably, to ease wrestling with technical issues during the project work and to allow more focus on agile programming practices, the course preparation period should be lengthened from three days to five, bringing the total length of the course to fifteen days. We also propose creation of another course "Agile customership", 1 cp.


Introduction
------------

This report describes organizing Agile Web Development (AWD) course at Department of Software Systems at Tampere University of Technology in April 2008.

The course was organized for the first time this year. The purpose of this report is to document the experiences from the course and to help decide what to do with the course next year. Since the course was novel in many ways, perhaps this report can also benefit other courses.

In the rest of this report, we describe (a) the educational goals of the course, (b) how the course was structured to achieve those goals, (c) experiences from the actual course implementation, (d) the feedback from students and customers, and finally (e) conclusions and the changes we propose for the next year's course.


Educational Goals
-----------------

We had three educational goals.

1. To teach students agile values.
2. To teach students agile practices. 
3. To teach students programming with a modern web framework.


### Agile values

Agile software development is a fuzzy term that encompasses a lot of different methodologies. The different methodologies can differ a lot in practice. They do, however, share values: a core set of beliefs about what is important in software development. The difference between agile methodologies and traditional software development is the stress agile methodologies put on these values. The most widely cited description of agile values is [Agile Manifesto](TODO).

The first goal of the course was to teach the students agile values. We stressed the following three principles.

* **Minimality**: The price of a project as a function of its requirements grows faster than linearly. Besides requirements, the same holds true with the number of developers, the amount of documentation, and the size of the code base. The project should include just what is needed and nothing more. 
* **Change**: Customer's understanding of his own needs is always lacking, and thus requirements will always change. The project should prepare for this change. 
* **Understanding**: Work done without understanding it leads to trouble. Developer should always understand (a) what he is trying to achieve and (b) why is he trying to achieve it and (c) how he is trying to achieve it.

Combined, there are a few consequences from these values:

* **Minimality+Change**: Preparation for future enlarges the project. Often the plans end up outdated. It is very important that plans are lightweight and easily thrown away when outdated.
* **Minimality+Understanding**: It is important to understand e.g. the domain area and document that understanding somehow. On the other hand, the amount of documentation should be minimized. One document we cannot work without is the program code. Thus, whenever possible, we should store our understanding in the code, not in external documentation. A high priority should be given to keeping the code as readable and as descriptive as possible.
* **Change+Understanding**: The developers' and customer's understanding of the software should keep improving throughout the project. Much of this comes from the dialogue between them. Customer should have a concrete understanding of what is the status of the project, and where it is heading. Because the future is very uncertain, the basis for the feedback should be a working prototype of the system. Thus, project iterations should be short and result in a working software that the customer can evaluate.


### Agile practices

Agile practices are methods to achieve the agile values. There is a large number of them, which we pruned to a few. The priority of the course was to teach:

* **Test-driven Development** (more specifically behaviour-driven development), and
* **Scrum project management**.

In addition to these, the we planned to teach these, if the time would allow:

* **Continuous integration**,
* **Refactoring**,
* **Pair programming**, and
* **Retrospectives**.


### Web programming

...



Structure
---------

The course lasted 13 days, starting on Wednesday, April 9, 2008, and ending on Friday, April 25, 2008. Sessions started each day at 9:00 and lasted till 16:00. There was a lunch break from 12:00 to 13:00, and shorter breaks two times a day. This totaled to roughly 13*6 = 78 hours of work. No homework was given. Passing the course required continuous or nearly continuous attendance to sessions.

The setting of the course was decided to resemble real-life project work in a fast-paced project. The first three days were preparation. After that, students worked in pairs. Each pair had their own project with a real customer.

The original plan 


### Original lecture plan

* first week: three days preparation
  * first day: Ruby
  * second day: TDD, RSpec
  * third day: Ruby on Rails, Agile

* second week: sprint 1
  * first day of project work: planning
  * goals of sprint 1

* third week: sprint 2
  * goals of sprint 2

### Actual lecture plan


Experiences
-----------

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

### Things that worked well




Feedback
--------

* student feedback
  * 

* customer feedback
  * generally satisfied
  * wished 

* feedback from prof Bormann
  * 


Conclusions
-----------

The course was a partial success. Three goals were set for the course: to teach agile values, agile practices and web programming. Out of these only the last one was realized with satisfactorily. However, the student feedback from the course was very positive.

We believe that the course - implemented even as it was this year - would be a valuable addition to the department's course palette. The course can be made still much better. Therefore, we propose that the course be given next year, but with a few changes.

### Planned changes for the next year

We plan to make the following changes for the next year's course.

* **The course will be lengthened from 13 days to 15 days.** This will allow for more preparation before the actual assignment work begins. The focus of the preparation will be teaching technical details. This way the work on the assignment should feel less painful and more agile. 
  
  Our plan for the structure of the first week looks like this:
  
  1. Monday: Introduction to the course. Learning to use the programming tools. Learning Ruby.
  2. Tuesday: Learning more Ruby.
  3. Wednesday: Learning Rails and the tool support for it.
  4. Thursday: Learning more Rails.
  5. Friday: Learning TDD with Spec:Rails.

  This should also give students a better chance to estimate how much they can achieve during the project, and the Scrum sprint goals will be more meaningful. 

  The two weeks of project work will be much like they were this year, only more structured, and possibly with additional lectures about agile topics.

* **The use of test-driven development will be mandated.** With all the other things they need to learn, this may feel painful to students at first. This is exactly the reason why students are unlikely to adopt it by themselves, and why it should be mandated.

* **The preparation of the Scrum sprints will be guided more carefully. Explicit sprint goals will be set.** This will give students a better understanding of Scrum.

* **Specific times will be set aside for customer interaction.**


### Proposal for another course: Working as an agile customer, 1 cp. 

The project customers wished for more guidance in preparing, monitoring and steering the project. This is a reasonable request, and we therefore propose a creation of another course. The students of this course would work as customers on the Agile Web Development course. The name of the course would be "Working as an agile customer" and its size one credit point.

The course would consist of lectures, a workshop, and the project work. We would prepare The workshop would 

Another reason why this course is needed comes from our experience in the software industry. The weakest link of a software project is often the customer. Many a project would benefit from having a customer who knows how to monitor progress and how he can (and cannot) help the project.

The department should recognize the importance of training software project customers. First step towards this would be creation of a course, even a small one, for this purpose.


Appendix
--------

### Origins

The course was modeled after an Agile Web Entwicklung course held at the University of Bremen by prof. Carsten Bormann. In the end there were many differences between the courses. 

The Bremen course is a much more intensive period, consisting of 12 days of 12 hour work, including one weekend. There were two reasons why the intensity of the Bremen course was not emulated in the Tampere course.

* Firstly, such intensity is foreign to the culture at TUT. We feared it would be difficult to attract students to the course. This was later confirmed by student feedback. It could also be difficult to convince the university administration to approve such a course. 
* Secondly, working 12 hour days is opposed to ideals of agile development. Our goal was to teach students sustainable practices that they could later emulate later in their careers.


### Credit points and relation to OHJ-5100 Web programming course

The Agile Web Development course was offered in two ways: (a) as an independent course and (b) in conjunction with OHJ-5100 Web Programming course. The independent course was worth 3 credit points. Passing the independent course required attendance to teaching and finishing the assignment successfully.

In conjunction with OHJ-5100, the course replaced the normal J2EE assignment, two lectures and three weekly exercises of OHJ-5100. The total course credit was 6 credit points: 4 credit points from OHJ-5100 and 2 credit points from 2 credit points from AWD. Passing the two courses required attendance to AWD teaching, successfully finishing the AWD assignment, finishing at least four OHJ-5100 weekly exercises and passing the OHJ-5100 exam.

Of the ten students enrolled to the course, nine took the course in conjunction with OHJ-5100.

