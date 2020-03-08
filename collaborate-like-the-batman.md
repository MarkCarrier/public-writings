---
title: Learn to collaborate from the Batman
urls:
    - "collaborate-like-batman"
published: false
tags:
    - software
---

# Learn to collaborate from the batman
For some of us, "teamwork" has become an oxymoron.  We once believed that collaboration and productivity should go hand in hand but years spent within dysfunctional work environments has beaten our sense of purpose into submission.  Many companies unwittingly create a culture where trying too hard is foolishness and teamwork's reputation gets tainted in the process.   I'm hoping to clear teamwork's name and help you restart to use the words "productivity" and "collaboration" in the same sentence without laughing.  Being a productive software developer without collaborating with others is in fact impossible.  To illustrate, we're going to take a look at one supremely productive individual: the Batman.

## Team spirit lessons from the Batman
But wait, doesn't the batman work alone you say?  He certainly seems to try:

!["I work alone"](images/batman-works-alone.jpg "I work alone")

<!-- https://whatculture.com/comics/10-superheroes-who-broke-their-own-rules -->
Despite what the Dark Knight might pretend, he, more than any other superhero, is dependent on others.  He has no superpowers at all!  The Batman can only protect Gotham thanks to the support of other people.  First of all, there's of course Alfred Pennyworth, who acts as a moral anchor and source of wisdom and new perspectives.  There's also Commissioner Gordon who keeps our hero aware of the city's problems and more immediate needs.  And we certainly can't forget Lucius Fox, Bruce's business manager and critical provider of the technological toys and gadgets that allow the Batman to convince the bad guys to go away.

## We "stand on the shoulder of giants".
Just like the Batman, you don't need superhuman abilities to become a "rock star" developer.  Just like the Batman, a programmer could never get anything done on his or her own.  For example, would you have the time and ability to write your own HTTP server?  How about a date-time library?  You might not realize [how complex this is](https://www.youtube.com/watch?v=-5wpm-gesOY).  Don't forget the leap seconds.  Would you build your own compiler?  Image, video, file compression algorithms?  How about an operating system?  Will you build a preemptive process scheduler or a cooperative one?  Can you build a microprocessor?  Will you go for a reduced or a complex instruction set architecture? Don't forget to consider the effects of quantum tunneling.  The truth is that every software solution we've ever delivered was the result of combining a tiny speck of our own work with the product of millions of hours of work from other people. To be a software creator you must be a software (and hardware) consumer.  Like Bruce, we inherited a _massive_ fortune from our engineering parents which gives us incredible creative freedom.

The reasons why this is possible are worth considering:
> 1. Building silicon based hardware is _cheap_.
> 2. Copying and distributing digital information is _extremely easy_.
> 3. The mathematical principles at the root of computer science make it possible to split big problems into many smaller problems.

Because of all this, developers have many great ways to access the software and hardware built by others:
* Linux allows us to install software in seconds using amazing package management tools and repositories (apt, dnf, snap, yum, pacman, dpkg, etc).  There's of course also Homebrew for the MacOS.  And I feel the need to specifically mention Arch Linux's fabulous [AUR (Arch User Repository)](https://aur.archlinux.org/).
* Git allows us to retrieve and share code in powerful way. It has taken gargantuan scale via github.  
* Most programming environments give us really smart ways to merge the various versions of other people's code into our own code without leaving the command line. JavaScript has npm, Python has pip, .Net has NuGet, Haskell has Hackage, and the list goes on.
* Docker allows us to package our solutions into images that can easily be shared and even securely deployed as containers in shared infrastructure in minutes.  

Can you believe that all these great things are _free_?  And it might seem obvious, but I want to highlight the amazing fact that we can now even easily access much of other people's code _while it runs_ (web APIs)!  Some of these APIs will give you access to free hardware.  Talk about an amazing Batcave.

## The hard part about being the Batman
So does this mean that being the Batman is easy?  The high costs of building software say otherwise.  Having access to cool tools and frameworks isn't enough.  Why not?  Because having fancy gadgets does not imply knowing how to use them.  To be the Batman, you have to learn to do your homework.

!["Batman reading"](images/batman-reading.png "Batman reading")
<!-- https://chasemagnett.wordpress.com/2015/07/06/comicbook-coms-san-diego-comic-con-survival-guide/ -->

The hardest part of software development is learning:

> 4. Copying and distributing human knowledge is _extremely difficult_.

Whatever level of knowledge you have today, you got there through a combination of direct and indirect collaboration.  Direct collaboration can take many forms. It might have started in an academic setting with lectures and team projects.  It also of course occurs on the job as whiteboard sessions, phone conversations or code reviews.  Indirect collaboration is more subtle.  It happens whenever you read something that another developer wrote, whether as code or documentation.  It also happens when you experiment with the tools directly.  The Batman is a good role model for the software developer because indirect collaboration is, in my opinion, much more important that direct learning.  Could you become a skilled programmer without ever directly collaborating with other developers?  It might not be common but it's definitely possible.  Could you make it without indirect collaboration?  No, of course not.  

What's the lesson?  Don't base your knowledge growth strategy on direct teamwork.  In software, most of the best available teachers are people you will never personally meet.  It's easy to just live in the local bubble of your direct teammates but you might be stunting the growth of your skill set.  Make sure you're learning to master the industry's well established collaboration tools.  Do you really know how to use Git or do you just re-use the same commands and hope someone else will do the merge?  Can you write a Dockerfile?  Learn it.

## How to learn
The means to share human knowledge have not changed drastically.  Reading books, blogs, stackoverflow, emails, slack, source code or listening to lectures, videos or a personal teacher are really just different versions of the two basic tools that we've had for ages: written communication and verbal communication.  They simply vary in quality and in how interactive they are.  Interactive communication has the benefit that it can be tailored to the individual listener's needs but it comes at a high price time wise.  In my opinion, books and blog posts remain the most effective ways of acquiring the bulk of the quality knowledge we need.  Authors can carefully craft them such that they pack a lot of information in pages that are easily distributed to millions.  Each individual reader can consume them at the time, place and pace that's convenient for he or she.  When asked how he learned to build rockets, [Elon Musk reportedly answered](https://www.esquire.com/news-politics/a16681/elon-musk-interview-1212/) "I read books".  A lot of very accomplished people highlight the importance of reading books.



Reading nutritious things isn't easy.  I find that it's a skill I have to continuously maintain and improve.  If I stop reading even for a week, it's hard to get started again.  If I read regularly, I notice my ability to enjoy even challenging books starts to grow.

This contrast, the ease of sharing digital information vs the challenge of sharing knowledge, makes it tempting to try to use tools that we don't understand.  "Deploy Kubernetes in 10 minutes".  Copy-pasting makes it possible to use the latest tech without learning very much but the end result is guaranteed problems.  Problems which you're not equipped to handle and will kill productivity.

Another temptation might be to split the work up across groups of people with constrained knowledge. "How does your code get to production?  I don't know, the devops people just take care of it."  This is again a recipe for killing productivity.  The most productive teams are the ones who can act independently.  The same can be said for individual developers.



<!-- This leads me to the conclusion I'm hoping you'll take away from this post: being productive in software requires collaborating with hundreds of other people, even for lone wolf developers.  We do this by **learning** about what others have built and by **using** what others have built. 
 A significant portion of our time must go to this collaboration -->

Interestingly, we often need to learn about technology to gain access to more technology.  For example, you could read about and learn to use docker and this will allow you to easily leverage tools like Redis or Kafka.  But you should learn about Redis and Kafka before using them.  Often, it's more important to understand what distinguishes one tool from another than its actual implementation.  (Those who ignore history are bound to repeat it).

## Don't repeat the Batman's mistakes


<!-- These four facts needs to be at the bottom of our collaboration and team building strategy.-->



Here's what I hope you'll remember from this article:

1. Building software isn't possible without the help of thousands of people.
2. Stay connected to these people. This requires being comfortable with the best collaboration tools.  Learn to use them.  Don't limit yourself to the tools used by your "local" team.
~~ 3. Become the Batman.  Being a specialist is okay, but since true black-boxes don't exist, it'll always be a handicap. Aim to become a expert-generalist.  ~~
4. Learning will be difficult if you don't cultivate a love for reading.
5. Understanding the reasons why a tool or technique is powerful is often more important than knowing how to use that tool or technique.
6. Learn to be the Batman but let a few people into the Bat-cave.