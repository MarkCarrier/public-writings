---
title: Collaborate like the Batman
urls:
    - "collaborate-like-the-batman"
indexed: false
tags:
    - Software
---

# Learn to collaborate from the batman
For some, "teamwork" is an oxymoron. The belief that collaboration and productivity go hand in hand is eroded by years spent within dysfunctional work environments. Companies create boundaries that prevent individuals from acting independently and so teamwork's reputation is tainted. I'm hoping to clear teamwork's name so you can use the words "productivity" and "collaboration" in the same sentence unironically. Being a productive software developer without collaboration is impossible. To illustrate, let's take a look at one supremely productive individual: the Batman.

## Team spirit lessons from the Batman
Doesn't the batman work alone, you say?  He certainly seems to try:

!["I work alone"](images/batman-works-alone.jpg "I work alone")

<!-- https://whatculture.com/comics/10-superheroes-who-broke-their-own-rules -->
Despite what the Dark Knight might claim, he, more than any other superhero, is dependent on others. He has no superpowers! The Batman can only protect Gotham thanks to the support of others. Alfred Pennyworth acts as a moral anchor. He supplies wisdom and new perspectives. Commissioner Gordon keeps our hero aware of the city's problems and supports his plans from the outside. We certainly can't forget Lucius Fox, Bruce's business manager and critical provider of the technological toys that allow the Batman to deal with bad guys.

## We "stand on the shoulders of giants".
Just like the Batman, you don't need superhuman abilities to become a "rock star" developer. Just like the Batman, a programmer could never get anything done alone. For example, do you have the time and ability to write your own HTTP server? How about a date-time library? You might not realize [how complex this is](https://www.youtube.com/watch?v=-5wpm-gesOY). Don't forget leap seconds! Would you build your own compiler? Image, video, file compression algorithms? How about an operating system? Will you build a [preemptive process scheduler or a cooperative one](https://en.wikipedia.org/wiki/Scheduling_(computing)#Types_of_operating_system_schedulers)? Can you build a microprocessor? Will you start with a [reduced or a complex instruction set](https://www.geeksforgeeks.org/computer-organization-risc-and-cisc/) architecture? Don't forget to consider the effects of [quantum tunneling](https://hackaday.com/2015/07/31/quantum-mechanics-in-your-processor-tunneling-and-transistors/). The truth is that every software solution we've ever delivered, including our first "Hello World", was the result of combining a tiny speck of our own work with the massive combined results of millions of hours of labour from thousands of smart people. To be a software creator you must be a software (and hardware) consumer. Like Bruce, we inherited a _massive_ fortune from our engineering parents which gives us incredible creative freedom.

The reasons why this is possible are worth considering:
> 1. Building silicon based hardware is _cheap_.
> 2. Copying and distributing zeroes and ones is _extremely easy_.
> 3. The mathematical principles at the root of computer science make it possible to split big problems into many smaller problems.

Developers have many great ways to access software and hardware built by others:
* Linux allows us to install software in seconds using amazing package management tools and repositories (apt, dnf, snap, yum, pacman, dpkg, etc). There's also [Homebrew](https://brew.sh) for the MacOS. I feel the need to specifically mention Arch Linux's fabulous [AUR (Arch User Repository)](https://aur.archlinux.org/).
* Git allows us to retrieve and share code in powerful and flexible ways. It has taken gargantuan scale via github. 
* Programming environments give us ways to merge other people's code into our own without leaving the command line. JavaScript has [npm](https://www.npmjs.com/), Python has [pip](https://pip.pypa.io/en/stable/), .Net has [NuGet](https://www.nuget.org), Haskell has [Hackage](https://hackage.haskell.org), and the list goes on.
* Docker allows us to package our solutions into images that can be shared and deployed as containers in shared infrastructure in minutes. 

Can you believe that all these great things are _free_?  It might seem obvious, but I want to highlight the amazing fact that we can now access much of other people's code _while it runs_ (web APIs)!  Some of these APIs will give you access to free hardware. Talk about an amazing Batcave.

## The hard part about being the Batman
So does this mean that being the Batman is easy? The high costs of building software say otherwise. Having access to cool tools and frameworks isn't enough. Why not? Because having fancy gadgets does not imply knowing how to use them. To be the Batman, you have to learn to do your homework.

!["Batman reading"](images/batman-reading.png "Batman reading")
<!-- https://chasemagnett.wordpress.com/2015/07/06/comicbook-coms-san-diego-comic-con-survival-guide/ -->

The hardest part of software development is learning:

> 4. Copying and distributing human knowledge is _extremely difficult_.

Whatever knowledge you have, you acquired it through a combination of direct and indirect collaboration. Direct collaboration can take many forms. It might have started in an academic setting with lectures and team projects. It also occurs on the job as whiteboard sessions, phone conversations or code reviews. Indirect collaboration is more subtle. It happens whenever you read something that another developer wrote, whether as code or documentation. It happens when you experiment with tools directly. The Batman is a good role model for the software developer because indirect collaboration is much more important than direct learning. Could you become a skilled programmer without ever directly collaborating with other humans? Perhaps uncommon, but possible. Could you make it without indirect collaboration? No, of course not. 

What's the lesson? Don't count on direct teamwork for knowledge growth. In software, most of the best available teachers are people you will never meet. It's easy to just live in your team bubble but you'd be stunting your growth. Make sure you're learning to master the industry's well established collaboration tools. Do you really know how to use Git or do you just re-use the same commands and hope someone else will do the merge? Can you write a Dockerfile? Learn to.

## How to learn
Despite the IT revolution, the means to sharing human knowledge have not changed significantly. Reading books, blogs, StackOverflow, emails, slack, source code or listening to lectures, videos or a personal teacher are just different versions of the two basic tools that we've had for ages: written communication and verbal communication. They simply vary in quality and in how interactive they are. Interactive communication has the benefit that it can be tailored to the individual listener's needs but it comes at a high price time wise. Books and blog posts remain the most effective ways of acquiring the bulk of the _quality_ knowledge that we need. Authors carefully craft them such that they pack a lot of information in pages that are easily distributed to millions. Each individual reader consume them at the time, place and pace that's convenient for them. When asked how he learned to build rockets, [Elon Musk reportedly answered](https://www.esquire.com/news-politics/a16681/elon-musk-interview-1212/) "I read books". Many accomplished people highlight the importance of reading books. YouTube can't compete.

Reading in-depth articles and books isn't easy. I find that it's a skill I have to continuously maintain and improve. If I stop reading even for a week, it's hard to get started again. If I read regularly, I notice my ability to both understand and even enjoy challenging books grows. I read every day. I usually have at least two on-going books, one more technical and one less demanding such as a work of fiction. If I'm too tired to read about the Fourier Series, I'll read the Foundation Series.


## What to read
Because sharing software is easier than sharing knowledge, it's often tempting to try to use tools that we don't understand. Some articles are geared towards this: "Deploy Kubernetes in 10 minutes!". Copy-pasting makes it possible to use the latest tech without learning very much about it. The end result is guaranteed problems you're not equipped to deal with. This kills productivity.

Many of the tools that are being created today solve old problems in new ways. For example, much of what we do with Docker could already be accomplished using zip files and virtual machines. But Docker came into existence because people who used these old methods gradually realized the existence of serious limitations and sought to improve the situation. It's therefore better to start by trying to understand how a given tool is conceptually different from others than to know how to use it. Articles such as [Docker vs Virtual Machine – Understanding the Differences](https://geekflare.com/docker-vs-virtual-machine/) may be more challenging but the knowledge you acquire will last for decades, even after Docker gets replaced. It also puts you in a position to suggest significant changes in your workplace since you can explain the advantages and limitations of a new approach even if you've hardly used it yourself.

Don't limit yourself in the things you read about. It's more appealing to read about things we can use right away. For example, a front-end developer might be more motivated to read about WebGL than about B-Tree indexing used in databases. Fully giving in to this desire will lead to being overspecialized. The Batman is a jack of all trades. His accomplishments require the help of other people but in the heat of the action he's able to act alone regardless of the type of problem he's facing. Specializing in a narrow area of software is _OK_ but if you're unable to build solutions end-to-end then your skill can become a handicap. The modern development team is small yet still able to quickly get things into the Done column. The more knowledge you have about the entire process, the more useful you'll be to your team (devops, security, algorithms, data persistence, etc). You should go beyond technical topics. If you were a manager, what books would you read? Aim to become an [expert-generalist](https://www.forbes.com/sites/michaelsimmons/2015/03/23/how-one-life-hack-from-a-self-made-billionaire-leads-to-exceptional-success/#67e48b87543d)


## Don't repeat the Batman's mistakes
Being the Batman is pretty great. It makes you more useful to your team today and more prepared for changes tomorrow. You won't struggle to find work and will experience the delight of true productivity at work (aka [Flow](https://www.bbc.com/worklife/article/20190204-how-to-find-your-flow-state-to-be-peak-creative)). There's a danger however. The trauma of past experiences can lead us to over isolate ourselves. Bruce won't let anyone get close to him because his past relationships caused him pain. We can do the same thing at work by literally avoiding people or by showing contempt for their questions or contributions thereby discouraging collaboration. Just because we've worked on bad teams before doesn't mean that the solution is to reject teamwork. Learn to be independent but let people into the Batcave and share your knowledge.


Here's what I hope you'll remember from this article:

1. Building software isn't possible without the help of thousands of people who you will never meet.
2. Stay connected to these people. This requires being comfortable with the current collaboration tools. Don't limit yourself to the tools used by your "local" team.
3. Learning will be difficult if you don't cultivate a love for reading.
4. Become the Batman. Being a specialist is OK but make sure it's not a handicap. Aim to become an expert-generalist.
5. Understanding the reasons why a tool or technique is powerful is often more important than knowing how to use that tool or technique.
6. Being independent doesn't mean being a loner. The more Batmans the better.