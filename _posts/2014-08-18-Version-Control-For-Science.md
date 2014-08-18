---

title: Version Control For Science
author: Andy Choens
layout: post
category: Git

excerpt: One skill the social sciences should adopt from computer science.

---

## First, A Story . . . Or Four

I am going to use the term "social scientist" to broadly apply to
everyone from economists to political scientists. I am explicitly
including disciplines such as epidemiology, criminal justice, social
work, etc. Social scientists write an amazing amount of code. The
tools vary by discipline, but everyone writes code. Epidemiologists
often use tools such as SAS, SQL and R. Social Workers tend to use
SPSS. Based on what I have seen in the journals, economists will use
anything that holds still. The tools vary, but all of these
disciplines write code. Often, this code is stored in files on a
shared drive.

Sharing is good, but work-flows that are acceptable for sharing
archived Word documents do not always scale up to the complexity and
requirements of formal programming. When sharing via a LAN, end users
either copy the code / syntax to their computer or they open and use
the files on the shared drive. The goal of this entry is to
demonstrate the problems and inefficiencies this work-flow
creates. This is not going to be an introduction to version control
although I will provide a link or two at the bottom. My goal is to
create a compelling picture of why business as usual MUST change for
social scientists.

The following scenarios are works of fiction. Any resemblance to
anyone I work with / for is entirely coincidental. That being said,
most of us have been in at least a few of these situations, so
hopefully these stories do feel familiar.

**Example # 1 - Sarah and Bob = Copies!**

Tim, the company's lead analyst wrote some code that can be used to
run a report for two different clients. On Monday, he is at home with
a head cold so Sarah and Bob are asked to run his reports. Sarah will
run the report for one client and Bob will run the same report for
another client. There are only minor differences in the two
reports. After the meeting, Sarah decides to work with the files
directly on the shared drive. Bob gets back to his desk a few minutes
later. Knowing he has to alter the report for his client, he copies
the code to his computer. Fifteen minutes into the work week, and we
already have two copies of the code base.

**Example # 2 - Error in the Report!**

After Bob copies the report code from the network to his computer, he
starts making his edits. Sarah does the same with the copy on the
shared drive.

The following day, Tim is feeling better and comes in to work. He
realizes there is an error in his program. Tim immediately fixes the
error in the code files on the shared drive. Tim sits next to Sarah
and he knows she is working with the code, but because Tim missed the
Monday morning staff meeting, he doesn't know Bob is working on the
code too. The following day, Sarah and Bob turn in their
reports. Unfortunately, Bob's report is wrong. Sarah's report is
correct because she ran the code on the shared drive, which included
Tim's changes.

**Example # 3 - Time Off**

Sam starts working with some files stored on the shared drive on
Wednesday afternoon. On Thursday morning (yes, Thursday), theshared
drive is mysteriously offline. Some say it happens every Thursday, but
it is just a rumor. It stays offline until lunch. Sam is frustrated
that he wastes the morning waiting for access to his code to come
back. He spends his morning talking to Bob who still needs to vent
about the errors in his report.

**Example # 4 - Who Did It?**

Todd is in a hurry. Unlike Sarah and Bob, he is perpetually running
late. He needs to run an important report for his supervisor, NOW!  He
opens the necessary files on the shared drive.

He is about to run the report, but notices he needs to tweak the
code. He makes his changes and runs the report. Unfortunately, Todd
also saves his changes to the network drive. These changes are buried
half-way through the code and they are wrong for everyone EXCEPT
Todd. His careless edits become part of the official program and
nobody even realizes it for several months. When the edits are
finally discovered, nobody is able to figure out when the errors were
introduced or by who. The company knows it has run several incorrect
reports, but nobody knows how many . . . or who to hold accountable
for the errors. 

## Version Control - The Solution

Version Control can help you with ALL of these problems and
more. Without version control, it is impossible to track changes to
code over time. It is impossible to remember why changes were made and
it is often impossible to know who made those changes. Programming is
complicated work. Let the computer do some of it! I recommend Git
because it does not require a centralized server and it is a commonly
used version control system. But ANY version control is better than
what most social scientists do. If you have files / folders with dates
or numbers in the name to help you remember which version is older, **I
AM TALKING TO YOU!** Start using version control TODAY.

The crux to this entire argument is the following fact: All social
scientists **who write code** are programmers. Unfortunately, many
such social scientists do not see themselves as programmers. I have
never met a social scientist who thought they could be effective without
knowing statistics, but I have met MANY social scientists who felt they could
be effective without learning basic computer science skills.

This is an attitude that I believe needs to change, now. Computer
science skills are more important **now** to the effective
implementation of social science research than at any prior moment in
human history.

Version control tracks changes made to code. It creates an auditable
log of change made to the code. It enables multiple programmers to
work on the same code at the same time. When appropriate, these
changes can be synced. When it isn't appropriate, the changes can be
left separate. Either way, the changes are tracked. It enables
scientists to know WHO edited the code, when it was edited and it even
includes a system to document WHY code changes were made.

This isn't just good computer programming. It is good science.

## Links!

I promised some links. So here are some links.

- For another perspective on this, see the Git section of the Software
  Carpentry website here:
  [Version Control with Git](http://www.software-carpentry.org/v5/novice/git/index.html)
    This is a terrific website. The authors of Software Carpentry
    provide introductory computer science courses for scientists all
    over the world. They are very cool people.
- For a more visial introduction:
  [A Visual Guide to Version Control](http://betterexplained.com/articles/a-visual-guide-to-version-control/)
- For an introductory primer in Git, see this
  article. [Getting Started - Git Basics](http://git-scm.com/book/en/Getting-Started-Git-Basics)

## In Closing

Download Git and install it today. It will pay for itself (it is free).

--andy

