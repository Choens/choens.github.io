---

title: Version Control For Science Part 2
author: Andy Choens
layout: post
category: Git

excerpt: How it could have been different.

---

## A Different Version of Yesterday's Story

Yesterday's blog post introduced us to a group of intrepid social
scientists working for a nameless corporation somewhere on planet
earth. Today's blog post is equally hypothetical, because we will
retell the story, this time using the Git version control tool. As Git
commands and ideas are introduced, they will be explained. The goal is
to show how different things could have been.

**Example # 1 - Sarah and Bob = Clones!**

Tim, the company's lead analyst wrote some code that can be used to
run a report for two different clients. He put the code into a Git
repository on the shared drive. On Monday, he is at home with a head
cold so Sarah and Bob are asked to run his reports. Sarah will run the
report for one client and Bob will run the same report for another
client. There are only minor differences in the two reports. After the
meeting, Sarah and Bob both "clone" the repository to their respective
desktops. A cloned repository is a special way of copying the files
from the master repository, to your local computer. But, unlike a
normally copied file, Git remembers where the files came from and it
tracks the changes Bob and Sarah introduce into their individual
clones. Bob and Sarah both create local branches of the code. That is,
they create a new version of the code in the master branch of the
repository and work in their local changes. Any change introduced by
Bob and Sarah are only allowed into the master repository with Tim's
approval. 

Fifteen minutes into the week, and we already have two
clones and two branches. Fortunately, this isn't a zombie story.

**Example # 2 - Error in the Report!**

The following day, Tim is feeling better and comes back to work. He
realizes there is an error in his program. Tim immediately fixes the
error in his personal repository. He them "pushes" the changes back
to the master repository on the shared drive. By midday, Bob and Sarah
both notice that the master branch is "ahead" other them by two
steps. They know that Tim has altered the code in the master
repository. They both "pull" these changes into their local
repositories and "merge" these changes into their local branches. Git
tells them there that the master repository has changed and they then
integrate Tim's latest changes into their own work. Bob even manages
to offer Tim some suggestions on how to improve the efficiency of a
query.

Both submit their reports on time and, unlike yesterday's story. Both
Bob and Sarah submit reports that are error free.

**Example # 3 - Time Off**

Sam starts working on a new project Wednesday afternoon. He locates
the appropriate repository on the shared drive and clones it to his
desktop. On Thursday morning, the shared drive is mysteriously
offline. Some say it happens every Thursday, but that is just a
rumor. The shared drive is offline until lunch. Sam is a little
irritated that he can't push his changes back to the master
repository, but he spends the morning patching up the code and running
the report. When the shared drive come back on-line, he pushes all of
his changes to the server and turns in his report. Bob is left with no
one to talk to because Sam is busy.

**Example # 4 - Nobody Did It?**

Todd is in a hurry. Unlike Sarah and Bob, he is perpetually running
late. He needs to run an important report for his supervisor, NOW!
His current crisis, the dreaded TPS report, is a report he submits
weekly. As per company policy, he has an individual repository on his
local computer of the report.

He is about to run the report, but notices he needs to tweak the
code. His report is different this week. He makes his changes and runs
the report.

There are two possible endings for this last scenario. We'll take each
in turn.

_Version 1 - Todd's Branch Wins_

Todd saves his changes and runs his report. It is late, but only by a
couple of hours. He saves his work in his local branch and smiles,
knowing he has the changes for next week. Nobody else in the company
is affected by these changes.

_Version 1 - The Master Branch Loses_

Unfortunately, Todd was working in the Master branch of his local
repository. He save his changes and pushes them to the master
repository. These changes are buried half-way through the code and
they are wrong for everyone EXCEPT Todd. Several other people pull
down his changes and blindly merges them with their code. The
following week, while working on his own TPS report, Tim notices the
changes and realizes what Todd has done. Todd's carelessly pushed
edits have already been used by several other staff members.

Tim confronts Todd about his error. Todd denies that he made the
changes until Tim shows him the Git log showing exactly when he, Todd,
had introduced the changes to the master repository. Tim re-explains
company policy about pushing to the master repository. Because the Git
log shows exactly when Todd pushed the changes and other users are
able to see exactly when the pulled those changes into their local
repositories, the company is able to identify which TPS reports were
run using the faulty code. Several reports have to be called back from
clients, but most reports are shown to be fine. Todd is demoted to
scrubbing potatoes.

## Version Control - The Solution

Of course, none of this is real. Most social scientists are convinced
their current system works. And it does, to a degree, if you only have
one or two people in your office. Development work-flows that seemed
OK in grad school don't work well in an office with 20+ social
scientists working side-by-side, sharing code and occasionally
talking loudly on the phone.

Professional programmers use version control because it prevents
problems and when problems do occur, it helps untangle the mess. These
scenarios are all about disaster prevention. I could easily tell you
four stories where using version control doesn't save the day, but it
makes getting the work done a lot easier.

Science is complex. Programming is complex. We use tools to manage the
complexity of the science. We should also use tools to manage the
complexity of the source code. Most importantly, version control is
tool agnostic. In fact, this is so important, I'll say it again.

**Version control is tool agnostic**

You can use version control with SAS, SQL, R, Python, SPSS, C, Java,
Fortran, .Net, etc. If it is code, written in plain text, you can
track it and manage it in version control. Certain ecosystems have
preferences, based on the wide-spread acceptance of certain tools in
certain communities. For example, R users are often encouraged to
learn and use Git, simply because it is the dominant source control
tool among R programmers. You can use other version control systems,
such as Subversion, with R, but most R programmers use Git and Git
integration is built into some R tools. But it is not a requirement.

So there you have it. My pro version control diatribe, in two
parts. Have a great rest of your week.

--andy


