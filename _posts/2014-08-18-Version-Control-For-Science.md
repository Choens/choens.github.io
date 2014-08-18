---

title: Version Control For Science
author: Andy Choens
layout: post
category: Git

excerpt: One skill the social sciences should adopt from computer science.

---

# First, A Story . . . Or Seven

I am going to use the term "social scientist" to broadly apply to
everyone from economists to political scientists. I am explicitly
including disciplines such as epidemiology, criminal justice, social
work, etc. 

Social scientists write an amazing amount of code. The tools vary by
discipline, but everyone writes code. Epidemiologists often use tools
such as SAS, SQL and R. Social Workers tend to use SPSS. Based on what
I have seen in the journals economists will use anything that holds
still. The tools vary, but all of these disciplines write code (Excel
is the primary exception to this rule). Often, this code is stored in
files on a shared drive.

End users either copy the code / syntax to their computer OR they open
and use the files on the shared drive. This is inefficient for a
number of reasons. The goal of this entry is to demonstrate the
problems and inefficiencies this work flow creates. I do NOT intend
this to be an introduction to Version Control although I will provide
a link or two at the bottom. My goal is to create a compelling picture
of why business as usual MUST change for social scientists.

The following scenarios are works of fiction. Any resemblance to
anyone I work with / for is entirely coincidental. That being said,
most of us have been in at least a few of these situations or were
very nearly in one of these situations, so hopefully these stories DO
feel familiar.

## Example # 1 - Sarah and Bob - CONFLICT!

Sarah and Bob both need to run the same report, for different
clients. Sarah gets to work early and decides to work with the files
directly on the shared drive. Bob knows he has to alter the report for
his client, so he copies the code to his computer.

Tim, the company's lead analyst wrote the code used by both Sarah and
Bob. But, he is at home with a head cold so Sarah and Bob are asked to
run the reports. The actual differences between Sarah's code and Bob's
is minimal. But because there are differences, and only one person can
work on a file at a time, there are now two different versions of the
code. One on the network and one on Bob's computer.

Two copies is minimal, but in this case it leads to . . . . 

## Example # 2 - Error in the Report!

After Bob copies the super-important code from the network to his
computer, he starts to run his report. He might not be the early-bird
that Sarah is, but he is a good analyst.

Two days later, Tim realizes there is a error in the program. Tim
immediately fixes the error in the code files on the shared
drive. Tim sits next to Sarah and he knows she is working on a report,
but because Tim missed the Monday morning staff meeting, he does not
know Bob is working on the code too. The following day, Sarah and Bob
turn in their reports. Unfortunately, Bob's is wrong. Sarah's report
is correct because she ran the code on the shared drive, which
included Tim's changes. Bob got left out. 

## Example # 3 - Time Off

Sam starts working with some files stored on the shared drive on
Wednesday afternoon. On Thursday morning, this shared drive is
mysteriously offline. It stays offline until lunch. Sam is frustrated
that he wastes the morning waiting for access to his code to come
back. 

## Example # 4 - Who Did It?

Todd is in a hurry. Unlike Sarah and Bob, he is perpetually running
late. He needs to run an important report for his supervisor, NOW!  He
opens the necessary files on the shared drive.

He is about to run the report, but notices he needs to tweak the
report. He makes his changes and runs the report. Unfortunately, Todd
also saves his changes to the network drive. These changes are buried
half-way through the code and they are wrong for everyone EXCEPT
Todd. His careless edits become part of the official program and
nobody even realizes it for several months. When the mistake is
finally discovered, nobody is able to figure out when the errors were
introduced or by who. The company knows it has run several incorrect
reports, but nobody knows how many . . . or who to hold accountable
for the errors. 

## Version Control - The Solution

Version Control can help you with ALL of these problems and
more. Without version control, it is impossible to track changes to
code over time. It is impossible to remember why changes were made and
it is often impossible to know who made those changes. This is why all
code should be stored in a repository controlled by a version control
tool. I personally recommend Git because it does not require a
centralized server. But ANY version control is better than no version
control.

The crux to this entire argument is the following fact: All social
scientists **who write code** are programmers. Unfortunately, many
such social scientists do not see themselves as programmers. I have
never met a social scientist who thought they could be effective without
knowing statistics, but I have met MANY social scientists who felt they could
be effective without learning basic computer science skills.

This is an attitude that I believe needs to change, now. Right
now. Computer science skills are more important **now** to the
effective implementation of social science research than at any prior
moment in human history.

## Links!

- For a more detailed introduction to:
  [A Visual Guide to Version Control](http://betterexplained.com/articles/a-visual-guide-to-version-control/)
- For an introductory primer in Git, see this
  article. [Getting Started - Git Basics](http://git-scm.com/book/en/Getting-Started-Git-Basics)
- For another perspective on this, see the Git section of the Software
  Carpentry website here:
  [Version Control with Git](http://www.software-carpentry.org/v5/novice/git/index.html)

    This is a terrific website. The authors of Software Carpentry
    provide introductory computer science courses for scientists all
    over the world. They are very cool people.


--andy

