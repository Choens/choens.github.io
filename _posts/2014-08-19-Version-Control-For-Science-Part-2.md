---

title: Version Control For Science Part 2
author: Andy Choens
layout: post
category: git

excerpt: How it could have been different.

---

## A Different Version of Yesterday's Story

[Yesterday's discussion](http://choens.github.io/git/2014/08/18/Version-Control-For-Science/)
introduced a group of intrepid social scientists working for a
nameless corporation somewhere on planet earth. Today's discussion
retells their story, but today our team is using the Git version
control system. The goal is to show how the story changes, because of
the advantages introduced when the team uses version control.

All Git commands and ideas are explained as they are introduced. You
do not need to be a Git expert to follow this, but I do recommend
reading the yesterday's discussion before reading today's discussion.

**Example # 1 - Sarah and Bob = Clones!**

Tim, the company's lead analyst wrote some code that can be used to
run a report for two different clients. He put the code into a central
Git repository on the shared drive. On Monday, he is at home with a
head cold. Sarah and Bob, two junior analysts with the company, are
asked to run his reports. Sarah will run the report for one client and
Bob will run the same report for another client. There are only minor
differences in the two reports. After the meeting, Sarah and Bob both
"clone" Tim's central repository to their respective desktops. A
cloned repository is a special way of copying the files from the
central repository, to the user's local computer. Unlike a normally
copied file, Git remembers where the files come from and it tracks the
changes Bob and Sarah introduce into their cloned repositories. All
repositories contain branches of code, which are parallel development
tracks of the code. Bob and Sarah both create local branches of the
code in their local repositories. This enables Git to track the
differences between the master branch and their individual
changes. As per company policy, changes introduced by Bob and Sarah are only allowed into
the master branch with Tim's approval.

Fifteen minutes into the week, and we already have two
clones and two new branches. Fortunately, this is not a Star Wars film
and this story includes no further references to the Clone Wars or Jar
Jar Binks. I apologize for making you think about Jar Jar Binks.

**Example # 2 - Error in the Report!**

The following day, Tim is feeling better and comes back to work. He
realizes there is an error in his code. Tim immediately fixes the
error in his personal repository. He them "pushes" the changes back to
the central repository on the shared drive. By midday, Bob and Sarah
both notice that the master branch on the shared drive is "ahead" of
their local branches by two changes. They know Tim has altered the
code in the central repository. Bob and Sarah "pull" these changes
into their local repositories and "merge" these changes into their
personal development branches. Git is able to warn both scientists
about the changes made to the central repository and it provides tools
to integrate (merge) Tim's changes into their own work. Git is able to
tell them, down to the letter, how Tim's master branch differs from
their local development branches. In fact, assuming that Tim's changes
do not overlap with their own changes, the merge can be done in a
matter of seconds.

Both submit their reports on time and both reports are error free.

**Example # 3 - No More Time Off**

This story is arguable one that not all staff will prefer. I apologize
in advance. It will however, win the acclaim of supervisors everywhere.

Sam starts working on a new project Wednesday afternoon. He locates
the appropriate central repository on the shared drive and clones it
to his desktop. On Thursday morning, the shared drive is mysteriously
offline. Some say it happens every Thursday, but that is just a
rumor. The shared drive is offline until lunch. Sam is a little
irritated that he can't push his changes back to the central
repository, but he spends the morning patching up the code and running
the report. When the shared drive come back on-line, he pushes all of
his changes to the central repository and submits his report.

Bob is left with no one to talk to because Sam is busy. Sorry Bob.

**Example # 4 - Who Did It?**

Todd is in a hurry. Unlike Sarah and Bob, he is perpetually running
late. He needs to run an important report for his supervisor, NOW!
His current crisis, the dreaded TPS report, is a report he submits
weekly. As per company policy, he has an individual repository on his
local computer of the report.

He is about to run the report when notices he needs to tweak the
code. His report requirements changed this week. He makes his changes
and runs the report.

There are two possible endings for this last scenario. We'll take each
in turn.

_Version 1 - Nobody Did It_

Todd saves his changes and runs his report. It is late, but only by a
couple of hours. He saves his work in his local branch and smiles,
knowing he has the changes he needs for next week. Nobody else in the
company is affected by his changes and Todd is still able to track and
merge approved changes that fall intot he master development branch.

_Version 1 - Todd Did It, And We Know When_

Unfortunately, Todd was working in the Master branch of his local
repository. He save his changes and pushes them to the central
repository. He did not follow company policy and go through the
appropriate code review process. These changes are buried deep in the
code and they are wrong for everyone, except Todd. Several other
people pull down his changes and blindly merge them with their
code. The following week, while working on his own TPS report, Tim
notices the changes and realizes what Todd has done. In the meantime,
Todd's changes have been used by several other staff members.

Tim confronts Todd about his error. Todd denies that he made the
changes until Tim shows him the Git log showing exactly when he, Todd,
introduced the changes to the master branch of the central
repository. Tim reiterates company policy about code review before
pushing changes to the master branch. Because the Git log shows
exactly when Todd pushed the changes and other users are able to see
exactly when they pulled those changes into their local repositories,
the company is able to identify which TPS reports were run using the
faulty code. Several reports have to be recalled, but most reports are
shown to be clear of the error. Todd is demoted to scrubbing potatoes.

Obviously, anyone reading this named Todd will prefer the first
scenario. But it is important to understand the utility and
accountability introduced when all programming changes are logged and
accounted for.

## Version Control - The Solution

Of course, none of this is real. Most social scientists are convinced
their current system works. And it does, to a degree. When there are
one or two people working on a code base, issues of accountability and
tracking appear to be less important. Unfortunately, this development
structure also leads to bad habits that are ineffective in an office
with 20+ social scientists working side-by-side, sharing code and
occasionally talking loudly on the phone.

Professional programmers use version control because it prevents
problems and when problems do occur, it helps untangle the mess. The
scenarios presented here all focus on disaster prevention. It would be
equally easy to write four stories demonstrating how the power and
logging capabilities make it easy to maintain multiple branches of a
code base, in a single repository or how changes can be easily merged
across multiple developers.

Science is complex. Programming is complex. We use tools to manage
this complexity such as statistics and models that simplify complex
interactions. It is equally logical to use tools to manage the
complexity of the source code that is driving the science. In the days
of Newton and Darwin, mathematics was the lingua franca of
science. Today, the lingua franca of science is the source code.

And I mean it. Show me the code. No code = No science. I belong to a
generation of analysts who believe the source code is arguably more
important than the fancy verbiage published in a journal. And that
source code, which drives our understanding of the science, should be
auditable.

Fortuantely, you can use version control with SAS, SQL, R, Python,
SPSS, C, Java, Fortran, .Net, etc. If it is code, written in plain
text, you can track it and manage it in version control. Any
discussion of version control is separate from ongoing discussions
about using SAS, R, SQL, Vertica, SPSS, etc. The language used is an
implementation detail. It is an important detail, but version control
is applicable regardless of which tool is used. The only real
exception to this is Excel and Word. These are not plain text and they
are not easily or effectively tracked via version control.

So there you have it. My pro version control diatribe, in two
parts. Later in the week, I will discuss installation and how to use
it with your own work. The scenarios here involve central
repositories, but Git can be useful to a social scientist even if it
is only used locally. More to come . . . . 

--andy


