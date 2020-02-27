---
title: Learn to collaborate from the Batman
urls:
    - "collaborate-like-batman"
published: false
tags:
    - software
---

# Learn to collaborate from the batman
If developing software as a team is not something that awakens warm fuzzy feelings inside of you or your employees, then I'm going to venture to claim that you've been looking at software collaboration the wrong way.  Alternatively, if you're new to software development, here's your chance to learn how to not get bogged down by erroneous "teamwork" concepts that permeate so many workplaces.  You can easily lose _years_ of knowledge growth if you're not collaborating the right way.  So what's the right way?  To answer this question, we will take lessons from an extremely productive individual: the Batman.

Doesn't the batman work alone?  He certainly claims to have a clear policy regarding teamwork:

!["I work alone"](images/batman-works-alone.jpg "I work alone")

<!-- https://whatculture.com/comics/10-superheroes-who-broke-their-own-rules -->
Despite what the Dark Knight might pretend, he, more than any other superhero, is dependent on others.  He has no superpowers at all!  The Batman can only protect Gotham thanks to the support of other people.  First of all, there's of course Alfred Pennyworth, who acts as a moral anchor and source of wisdom and new perspectives.  There's also Commissioner Gordon who keeps our hero aware of the city's problems and more immediate needs.  Collaboration between him and the Batman is continuous.  And we certainly can't forget Lucius Fox, Bruce's business manager and critical provider of the technological toys and gadgets that allow the Batman to convince the bad guys to go away.

Just like the Batman, you don't need superhuman abilities to become a "rock star" developer.  Just like the Batman, getting anything done completely on your own is impossible.  Do you have the time and ability to write your own HTTP server?  How about a date-time library?  You might not realize [how complex this is](https://www.youtube.com/watch?v=-5wpm-gesOY).  Don't forget the leap seconds.  Would you build your own compiler?  Image, video, file compression algorithms?  How about an operating system?  Will you build a preemptive process scheduler or a cooperative one?  How about a microprocessor?  Will you go for a reduced or a complex instruction set architecture? Don't forget to consider the effects of quantum tunneling. The truth is that the first line of your own code that you ever executed was possible thanks to thousands of people who've worked millions of hours designing and building these things.  Perhaps more than in any other profession, we programmers "stand on the shoulder of giants". Or perhaps it's the shoulders of a few giants plus a huge amount of normal sized people.

Like Bruce, we inherited a _massive_ fortune from our engineering parents which gives us incredible creative freedom.  This is what drew me to programming as a teenager.  Even in the absence of a personal teacher, I was able to start creating programs on my dad's 286 IBM Compatible.  And that was without the internet. Today, even with the most budget friendly of computers and connections, you can start collaborating with millions of people who have collectively built, and continue to build,  myriads of amazing hardware and software systems.  In 2018, about 50% of the planet's inhabitants have access to this.

The reasons why this is possible are worth considering:
1. Building silicon based hardware is _cheap_.
2. Copying and distributing digital information is _extremely easy_.
3. The mathematical principles at the root of computer science make it possible to split big problems into many smaller problems.

Because of all this, software developers have many great ways to access other people's software. On linux we have a number of great package management tools and repositories (apt, dnf, snap, yum, pacman, dpkg, etc).  We have the quintessential collaboration tool, git, which has taken gargantuan scale via github.  Most programming environments even give us really smart ways to merge the various versions of this shared code into the various version of our own code without leaving the command line. JavaScript has npm, Python has pip, .Net has NuGet, Haskell has Hackage, and the list goes on.  We can package our apps using Docker images and easily deploy onto shared infrastructure in minutes or seconds.  All of these things are _free_.  We can even access other people's code while it _runs_ via web APIs!  This can be as simple as fetching a weather report or as advanced as creating very affordable virtual hardware resources in AWS.

So does this mean that being the Batman is easy?  No, having cool tools does not mean that you know how to use them.  

!["Batman reading"](images/batman-reading.png "Batman reading")
<!-- https://chasemagnett.wordpress.com/2015/07/06/comicbook-coms-san-diego-comic-con-survival-guide/ -->

The hardest part of software development is learning:

4. Copying and distributing human knowledge is _extremely difficult_.

The means to share human knowledge have not changed drastically.  Reading books, blogs, stackoverflow, emails, slack, source code or listening to lectures, videos or a personal teacher are really just different versions of the two basic tools that we've had for ages: written communication and verbal communication.  They simply vary in how interactive they are.  Interactive communication has the benefit that it can be tailored to the individual listener's needs but it comes at a high price time wise.  In my opinion, books and blog posts remain the most effective ways of acquiring the bulk of the advanced knowledge we need.  Authors can carefully craft them such that they pack a lot of knowledge in pages that are easily distributed to millions.  Each individual reader can consume them at the time, place and pace that's convenient for he or she.  When asked how he learned to build rockets, [Elon Musk reportedly answered](https://www.esquire.com/news-politics/a16681/elon-musk-interview-1212/) "I read books".  A lot of very accomplished people highlight the importance of reading books.

Reading nutritious things isn't easy.  I find that it's a skill I have to continuously maintain and improve.  If I stop reading even for a week, it's hard to get started again.  If I read regularly, I notice my ability to enjoy even challenging books starts to grow.

This contrast, the ease of sharing digital information vs the challenge of sharing knowledge, makes it tempting to try to use tools that we don't understand.  "Deploy Kubernetes in 10 minutes".  Copy-pasting makes it possible to use the latest tech without learning very much but the end result is guaranteed problems.  Problems which you're not equipped to handle and will kill productivity.

Another temptation might be to split the work up across groups of people with constrained knowledge. "How does your code get to production?  I don't know, the devops people just take care of it."  This is again a recipe for killing productivity.  The most productive teams are the ones who can act independently.  The same can be said for individual developers.



<!-- This leads me to the conclusion I'm hoping you'll take away from this post: being productive in software requires collaborating with hundreds of other people, even for lone wolf developers.  We do this by **learning** about what others have built and by **using** what others have built. 
 A significant portion of our time must go to this collaboration -->

Interestingly, we often need to learn about technology to gain access to more technology.  For example, you could read about and learn to use docker and this will allow you to easily leverage tools like Redis or Kafka.  But you should learn about Redis and Kafka before using them.  Often, it's more important to understand what distinguishes one tool from another than its actual implementation.  (Those who ignore history are bound to repeat it).

## Don't repeat the Batman's mistakes


<!-- These four facts needs to be at the bottom of our collaboration and team building strategy.-->



Points:
 - Feedback is key.  Just trying something is often better than speculation (small batch sizes).
 - We should aim to be as independent as possible
 - The more we know about all the different aspects of our software, the quicker we can iterate (devops, product knowledge, back end development, front end development, data persistence systems, algorithms).
 - Don't be afraid to work closely with others