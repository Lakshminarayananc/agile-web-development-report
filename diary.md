Agile Web Development course diary, spring 2008
===============================================

Antti Tarvainen, antti.tarvainen@iki.fi

These are notes I wrote down (mostly) after each day's teaching.



Wed 2008-04-09
--------------

### Events:

9:00 People start arriving.

9:10 Nine out of ten present, starting the teaching. (The last one arrives 9:30.)

9:10-9:20 Everyone introduces themselves.

9:20-10:05 Lecture about Ruby.

10:05-10:20 Break.

10:20-10:50 Lecture about Ruby.

10:50-11:10 Setting up environment. Coding exercise (hello.rb).

11:10-12:00 Coding exercise (booklist.rb).

12:00-13:00 Break.

13:00-14:00 Coding exercise (booklist.rb).

14:00-14:15 Break.

14:15-14:40 Coding exercise (booklist.rb).

14:40-15:45 Enumerable exercise.


### Details:


#### hello.rb

Students were given a specification in an RSpec file and a solution template as a Ruby file. All they needed to solve it was to write a "puts 'Hello, World!'" in the Ruby file and run "spec spec" in the parent directory.

The primary goals of this exercise were

* to introduce Ruby to students
* to introduce coding tools to the students
* to make sure everyone's environment was set up properly

A secondary goal was 

* to gently introduce RSpec syntax so students get it more easily on the next day (when TDD with RSpec would be taught).

I asked students if they would like to have me do the example in AptanaStudio or in a plain text editor. The result was about 50-50. I chose AptanaStudio, because I believe it is the tool with more challenges. There were in fact quite a few of them but in about twenty minutes everyone had finished the exercise.


#### booklist.rb

This was a more complex Ruby programming exercise. 

The goals of this exercise were

* to introduce these concepts to students: classes, methods, instance variables, iterating arrays with Enumerable methods
* to teach students how to find information about Ruby libraries

Secondary goals were

* to find out about each students skills to better teach them
* to promote student cooperation

All students managed to finish or nearly finish this exercise. The students who finished it first helped their slower peers.


#### Enumerable exercise

Students were divided into pairs. Each pair got assigned a few methods from the  Enumerable module. Each pair's assignment was to demonstrate the methods via examples on the board. Afterwards, we went through all the examples and figured out together what each of them did.

The goals of this exercise were

* to make the ruby style enumeration code feel natural to students
* to have a non-coding task to finish the day

A secondary goal of the exercise was

* to promote student cooperation

This was a fun, lightish exercise for the end of a day.


### General notes:

I didn't know how much material I would need. In the end, seems like my material would have been enough for about three days. Perhaps we should cover some Ruby subjects on Friday as well.


Thu 2008-04-10
--------------

### Events:

9:15 Starting the teaching. Advice people to put ~seitti/railskurssi/bin/environment.sh in their .bashrc file.

9:20-9:45 Lecture about TDD.

9:45-10:15 TDD example (limited_stack.rb).

10:15-10:30 Break.

10:30-11:30 TDD coding exercise (limited_stack.rb).

11:30-12:00 Demoing ruby features (splatting, super) and tools (irb, rubygems, rake).

12:00-13:00 Lunch break.

13:00-13:30 Lecture about outside-in design.

13:30-13:50 Mock object example.

13:50-14:00 Preparation for the Coding Dojo: rules of ten-pin bowling.

14:00-14:15 Break.

14:15-15:45 Coding dojo.

15:45-15:55 Showing two alternative solutions to the ten-pin bowling exercise.


### Details:

#### limited_stack.rb

Students were asked to implement the same stack class as the teacher did on the demo. They were told to follow the TDD procedure (write tests, FAIL, write code, PASS, refactor, PASS). After they had implemented all that, they were asked to add new features to code using the TDD procedure.

The goals of this exercise were:

* to make the TDD process feel natural to the students.
* to learn the RSpec syntax.

There were a lot of variation among students on doing this exercise. Some immediately felt the process natural, some didn't seem to understand the point of it at all. The ease of understanding TDD probably correlated strongly with the amount of programming experience. A couple of students had some trouble with basic programming practices, a couple more with the syntax of Ruby.

Some students may have felt that it was boring to implement the same exercise I had already done on. I still believe this is a good way to teach the TDD process to the students. The alternative would require too much thinking about implementation and take the focus away from the real stuff.


#### Coding Dojo

(See http://wiki.agilefinland.com/?CodingDojo for an explanation of the concept.)

Students cooperated in writing a bowling game score calculator using the coding dojo method. This is the same TDD example that is used http://butunclebob.com/ArticleS.UncleBob.TheBowlingGameKata .

The goals of this exercise were:

* To make everyone think about the decisions and difficulties in TDD.
* To learn to read and communicate in and about code.

Secondary goals of this exercise were:

* To encourage student communication and participation.

I didn't spend much time prioritizing the features before we started coding. That lead to trouble focusing the development. Everyone seemed to be thinking differently on what and how we should design. After about half of the time was used, I stopped the coding, and we had a small communication break. I asked if anyone thought we knew what we were doing. No one thought so. I then gave four prioritized features and we started over. After that the coding started going better. The students finished a couple of simple cases, but the really hard cases were left unsolved.

In all, I think the exercise went pretty well. Students were excited about the task and discussed alternative design solutions in groups, sometimes visualizing their thoughts on the whiteboard. 

Finally I showed two alternative finished versions of the code they were writing. (I emphasized I had used many hours on writing those, and that the students should feel good about their achievement.)

Towards the end of the dojo most of the communication seemed to be among but not between two groups: Finnish students and foreign students. This was unfortunate and I think we should break this pattern somehow. Perhaps tomorrow I will pair the students myself so that each pair has one Finn and one foreigner.


Fri 2008-04-11
--------------

### Events:


9:15 Started the teaching.

9:15-10:10 Lecture about various Ruby features: case-expression, modules, mixins, public/protected/private.

10:10-10:25 Break.

10:25-11:30 Ruby libraries exercise, part 1: personal coding example.

11:30-11:50 Explaining the library example to partner.

11:50-13:00 Lunch break.

13:00-14:10 Ruby libraries explained to everyone.

14:10-14:25 Break.

14:25-15:10 Rails view+controller demo. 

15:10-15:55 Rails exercise.


### Details:

#### Ruby libraries exercise

Every student got one library/class/module that he needed to get familiar with. The student wrote an example code that used this library. He then explained it to his pair, and after that to the entire group. The modules in question were: Object, Module, Comparable, Enumerable, Dir, File, Time, String, OptionParser, ERB.

I chose pairs so that they were from opposite sides of the room, and with all pairs consisting of one Finn and one foreigner.

The goals were to:

* learn about different libraries.
* learn how to get information.
* get more used to writing Ruby.

A secondary goal was:

* to get more familiar with the students on the other side of the room.

This took much more time than I thought it would. The last part felt like it just repeated the middle part. I should have told the students that each would present their _partner's_ work in the end. That would have motivated the middle part more. Now I tried it in the end both ways: student introducing his partners work or his own work.

One problem with this was perhaps the different skill levels of different students.


#### Rails exercise

This was an ad hoc exercise. I didn't know what would be a good first exercise and decided to see how the teaching would go first.

After a quick Rails demo showing how to create a view and a controller in Rails, and showing how to use a link_to helper in the view, students were asked to get familiar with various view helpers and try them in their own code.

The themes were: forms with dates, forms without dates, link\_to+image\_tag, and small helpers.


The goals were to:
* Get familiar with working with Aptana Studio and Rails.
* To learn how to get information.
* For the teacher to learn about any problems with the environment or any large omissions in teaching.

A secondary goal was:

* To learn something about view helpers in Rails.

The biggest problem was that we didn't have much time and that I didn't have good reference books to give to students. (I had one up-to-date Rails Way and one nearly up-to-date (the newest edition) Agile Web Develoment with Rails, plus two outdated versions of AWDwR).


### General notes:

I wasn't prepared properly and some time was lost on thrashing. I changed my plans a couple of time during the day, which caused confusion.

All in all, it wasn't a terrible day but could have been better.


Mon 2008-04-14
--------------

### Events:

9:15-9:55 Lecture about working with a customer.

9:55-10:10 Break.

10:10-12:00 Work: Getting requirements from the customer, sketching UI.

12:00-13:00 Break.

13:00-14:00 Scrum lecture + demonstration.

14:00-15:15 Work: Finding user stories, guestimating user points, prioritizing.

15:15-15:50 ActiveRecord lecture. (Got through DB mapping and CRUD operations. Most of the slides are still ahead of us.)


### Details:


#### ActiveRecord lecture

This was a lot faster than my previous lectures, and I digressed from the slides much less. Perhaps there is less to talk about ActiveRecord, or perhaps my attitude was different. I don't think this was worse or better than the previous lectures, just different. (But we really needed a quick lecture at this point too. Tomorrow I plan to have only one hour lecture before the real work starts.)

### General notes:

An OK day. 


Tue 2008-04-15
--------------

### Events:

9:15-10:05 Demo to get things started.

10:05-12:00 Work. (Break whenever students wanted.)

12:00-13:00 Lunch break.

13:00-13:45 Advanced ActiveRecord lecture.

13:45-14:00 Break.

14:00-14:10 Demo: sharing project with SVN in AptanaStudio.

14:10-16:00 Work.


### Details:

#### Demo to get things started

1. Tiny lecture about ActiveRecord's foreign keys, belongs\_to, has\_many, and has\_one.
2. Installing Spec::Rails plugin.
3. Scaffolding.
4. (Would have shown how to share the project with SVN in AptanaStudio, but forgot to install the Subclipse plugin on student machines.)

#### Advanced ActiveRecord lecture

Not very useful information, but wanted to finish the ActiveRecord part.


### General notes:

I asked the students if we need more books and we decided we manage with the books we have now. (Before the course I accidentally ordered only one AWDwR book, when I meant to order three of them.)


Wed 2008-04-16
--------------

### Events:

9:15-9:55 Routes and ActionController lecture.

9:55-10:10 Break.

10:10-10:25 Daily scrum.

10:25-12:00 Work.

12:00-13:00 Lunch break.

13:00-13:25 Demos: root route, layouts.

13:25-16:00 Work. (Break whenever needed.)

### Details:

#### ActionController lecture

I presented this directly from the lecture notes and the lecture was quite  boring. It was just detail after detail, without context.

Couple of ideas to make this better:

* a controller example with more and more features. 
* more about typical uses for each feature.

#### Daily scrum

This went well. It didn't last too long and I believe it helped students to focus on their work and "get real".

#### Demos: root route, layouts

Just random things that I thought might be useful for the students. It should be noticed that I didn't talk about 

### General notes:

It seems that nobody is using TDD at the moment and I haven't demanded it. I will talk more about it tomorrow and we will see then.

Groups don't work in an iterative way. It seems that I find the concept so natural that I haven't explained it enough. It is too late now to make any big changes, but I will remind people tomorrow in the scrum meeting that it's easier for them if they take one feature at a time.

I will bring up these issues in the retrospective on Friday.

We don't have enough room at the back of the room for burndown charts for each project. I put a sheet there that contains a combined burndown chart (normalized so that each project has an equal weight.)


Thu 2008-04-17
--------------

### Events:

9:15-9:40 Work.

9:40-10:00 Daily Scrum.

10:00-12:00 Work.

12:00-13:00 Lunch break.

13:00-14:00 REST lecture.

14:00-14:15 Break.

14:15-16:00 Work.


### Details:

#### Daily Scrum

Started late, because I decided to wait until everyone was present.

#### REST lecture

I used creative-commons-licensed slides I found on the net. 

I started with a short general description of REST. The main part of the talk was about how to use RESTful routes in Rails.

REST is quite a multi-faceted concept. It is not easy to motivate the need for it clearly. Perhaps the motivation could start with a conversation about how web browsers work and how this should be taken into account when writing a web application.

The lecture went pretty well.

### General Notes:

The team that has best embraced agile method (YAGNI, KISS) is the one whose customer started with only one user story. They finished their user story quite quickly and were ready to start adding new features. The dialogue between the team and the customer is civilized and fruitful.

Also, this course might be a good learn experience for students as well. 

Thus, possible improvements for next year's course:

* Each customer presents only one user story at a time to the team. When the team finishes that story, the next one is presented, etc. (Or the teaching assistant may have the entire list, to act as a customer when the real one is not present.)

* Course called "acting as a agile customer", 1 cp.


Fri 2008-04-18
--------------

### Events:

9:15-9:40 Demo about using Rails::Spec to test models.

9:40-9:50 Daily Scrum.

9:50-12:00 Work.

12:00-13:00 Lunch break.

13:00-15:15 Work.

15:15-15:50 Retrospective. 


### Details:

#### Retrospective

I used a retrospective format that aimed to answer the following questions:

* What did we do well, that if we don’t discuss we might forget?
* What did we learn?
* What should we do differently next time?
* What still puzzles us?

I wrote the questions on the white board. We then answered the questions in three parts:

1. Students talked with their pair and tried to find answers that applied to them.
2. Every pair presented their answers. I wrote them on the board and commented on them. 
3. I presented answers to these questions from my perspective on my work.

Two groups found things they wanted to try to do differently next week. (Both of them decided to try to work on smaller chunks with clearer goals.) The others decided to continue the way they had worked so far.

### General Notes:

I had lunch with students for the first time. I thought about doing that already earlier. There is a small risk is that students find it uncomfortable. 


Mon 2008-04-21
--------------

### Events:

9:15-9:30 Daily Scrum.

9:30-10:50 Work.

10:50-11:05 Break.

11:05-12:05 Ajax lecture 1/3 (by prof. Bormann).

12:05-12:20 Prof. Bormann reviews students' work.

12:05-13:00 Lunch break.

13:00-13:30 Prof. Bormann reviews students' work.

13:30-14:50 Ajax lecture 2/3 (by prof. Bormann).

14:50-15:00 Break.

15:00-15:40 Work.

15:40-16:10 Ajax lecture 3/3 (by prof. Bormann).

16:10-18:20 Bonus work (assisted by prof. Bormann).

18:20-22:00 Dinner.


Tue 2008-04-22
--------------

### Events:

9:15-9:20 Demo: installing Firebug.

9:20-9:35 Daily scrum.

9:35-12:00 Work. (I was away 10:10-10:20 and 10:55-11:40.)

13:00-13:50 Deployment & scaling lecture.

14:05-16:00 Work.

16:00-17:00 Bonus work.

Wed 2008-04-23
--------------

### Events:

9:15-9:30 Daily Scrum.

9:30-12:00 Work.

12:00-13:00 Lunch break.

13:00-13:30 Lecture about maintainability and good style.

13:30-13:45 Exercise about maintainability and good style.

13:45-14:30 Demo about maintainability and good style.

14:30-16:00 Work.


### Details:

#### Maintainability and good style (lecture, exercise, demo)

##### Lecture

I introduced six concepts important to maintainability of code:

* DRY (Don't Repeat Yourself)
* YAGNI (You Ain't Gonna Need It)
* DDD (Domain-Driven Design)
* orthogonality
* state is evil
* KISS (Keep It Simple, Stupid)

I didn't have slides, but used whiteboard to give examples about some of these.

##### Exercise

I had prepared a simple Rails application that kept track of game scores in a sports league. I presented the code of the main controller to the students. The students then had ten minutes to find stylistic problems in the code and write them down.

##### Demo

I walked through the controller code, asking students to suggest improvements. 

The goals of this lecture/demo/exercise were:

* to introduce the six concepts to students
* to encourage the students think about maintainability and style as important issues
* to demonstrate the typical refactorings in Rails controller code

The students found a few of the small problems but missed the large DDD problem of the controller containing important domain logic.



Thu 2008-04-24
--------------

### Events:

9:15 - 9:30 Daily Scrum.

9:30 - 12:00 Work.

12:00 - 13:00 Lunch break.

13:00 - 13:55 Rails security lecture.

14:10 - 16:00 Work.

16:00 - 17:30 Bonus work.


### Details:

#### Rails security lecture

I used slides I found from the Internet and covered a few of the most important Rails security threats and how to prevent them. (Cookie-based session vulnerabilities, SQL injection, XSS, CSRF, Javascript attacks, DOS, etc.)

This was a typical boring lecture and not as good as the best ones found on the Internet. I believe a demo of the most important threats plus a pointer to a security checklist would have been better.

(A note added after the course: According to student feedback, the students liked this lecture very much. Very surprising. One of the reasons may be that the lecture is a set of individual topics. If you don't understand one of the topics, you can still follow and understand the rest of them.)

### General notes:

A lot of good software practices are ignored by students. Most notably TDD, but also proper naming, compact functions, etc. 

This probably has a lot to do with lack of skills to use proper tools. A few tools that should be introduced in an earlier stage of the course:

* FireBug
* HTML validator (e.g. Firefox plugin)
* RSpec StoryRunner (this demands (and supports) a proper process)
* a proper IDE (_and_ highlighting its features early in the course)

Professor Bormann commented on Tuesday that the students in Bremen have better tool skills than the students here.


Fri 2008-04-25
--------------

### Events:

9:15-9:25 Daily Scrum.

9:25-11:15 Work.

11:15-11:50 Finished assignments presentations. (2 out of 5 teams.)

11:50-13:00 Lunch break.

13:00-14:00 Finished assignments presentations. (The remaining 3 teams.)

14:00-14:45 Retrospective.

14:45-15:15 Filling course feedback forms.

15:15-15:50 People over processes lecture.

### Details:

#### Finished assignments presentations

Each of the teams had 20 minutes to present their finished assignment. 

Each team

* told what the customer's wanted
* demoed the application
* elaborated the important design decisions and told what were the hardest things to get right
* possibly presented interesting parts of the code 

At the end of each presentation we applauded the team for their good work.

The goals of this exercise were:

* to give students the good "finished!" feeling at the end of the project
* to let students compare their work
* to highlight the good solutions on each project

Students appeared to be interested in this. Some questions were asked about others' solutions.

It might be a good idea to have this at the end of each sprint. That would make other students problems more real, and it would provide a stronger incentive to get the project working at the end of the sprint.


### Retrospective

Each team discussed among themselves what problems they had, what they learned, and what did they do right. After a few minutes, I talked to teams one by one, semi-privately. I presented my views of the teams strengths and weaknesses and suggested ways to improve their performance after this course.  

This seemed to be a better way to do the retrospective than the one we used last week. The problem was that it took a lot of time to talk with each team while other teams had to wait. Perhaps this should be interleaved with other between-sprints activities, such as customer feedback and sprint planning?

### People over processes lecture.

This was my attempt to end the course with an upbeat "now go and change the world" note and it seemed to work quite nicely. 

(A month later:) I paraphrased the lecture from memory and saved it here: [People over processes speech](people_over_processes.html).

