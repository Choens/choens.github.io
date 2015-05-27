---
title: Thanks Lenovo, for truly crappy software.
author: Andy Choens
layout: post
category: bitching
excerpt: Over the long weekend, I spent some time with a Lenovo laptop. I came
away from the experience with a bad taste in my mouth.

---

Over the long weekend, I spent some time with a Lenovo laptop. I came
away from the experience with a bad taste in my mouth. The hardware
was and is good stuff. Lenovo makes great hardware. But, their
software sucks a giant lemon. The following rant will explain.

Recently, my brother-in-law asked me to clean-up an older Lenovo
laptop and prep it for their 10 year old son. As a general rule, I
don't do Windows support on the weekend, but I am willing to make
exceptions. Although I prefer to keep my non-work IT time dedicated to
Linux; I saw this as an opportunity to do something nice for my nephew
AND I saw it as an opportunity to give him some FOSS titles like
Krita, Celestia, etc.

Fun! My first job was as a computer-tech in high-school. My primary
job was fixing software problems and virus infections in Windows 3.x
and Windows 95. This should have been another fun trip down memory
lane. Just clean up some malware and remember the good old days. I
expected the clean up to take a couple of hours and installation of
new software to take an hour or two.

I was wrong. Very wrong. It took me HOURS to complete this idiotically
simple task. In the end, it was more like Gilligans Island than a long
movie. My three to four hour project turned into a really bad comedy
with too many repeat jokes. I was the butt end of all the jokes and
the comdeian is an ass-hole names Lenovo.

The laptop in question is a G560, running Win7. An older but
respectable rig. In a nutshell, this is what I did:

- I cleaned up the accumulated malware.
- Replaced the anti-virus and
- Generally tidied things up.
- Removed any / all unnecessary software.

Matt (brother-in-law / client) asked me to strip the system down to
stock windows. The new owner, his son, is 10 years old. This kid
doesn't need duplicate software. He does not need additional chat
software, encryption software, etc. In other words, he has no use for
the Lenovo software stack. I decided my job included removing all of
the Lenovo-branded software that had come with the laptop. None of
this software is truly necessary and it just added extra features my
client would see as liabilities in the hands of a 10 year old. does
not want on the system. I assumed the Lenovo-branded software was
properly written. It isn't.

*Note: I only removed end-user apps. I did not remove any Lenovo
drivers. Obviously, the system needs those.*

The app VeriFace was my nemesis. Everything else removed itself from
the computer without causing problems. But Veriface would not go away
without a fight. After removing it via the Windows Control Center, it
still started up, sorta, when the computer booted. I was not able to
prevent this behavior via msconfig, even though I deactivated all
VeriFace systems in the boot menu. Worse, VeriFace continued to
provide users with two apparently separate methods to log into the
computer.

In truth, my first reaction to a fully functional VeriFace was bad. It
is a dumb idea. Logging into a computer via a software hack that
"recognizes" the user may or may not be a good idea. I won't comment
on that. But hacking the Windows log-in screen with some half-baked
crap that has NEVER seen an update is a decidedly BAD idea. It is bad
op-sec and it is bad customer service.

Adding insult to injury, after "removal" the Veriface software would
present an alternative log-in method which no longer worked. As
purchased, VeriFace is merely confusing and an example of
middle-school grade op-sec. After "removing" VeriFace, I was left with
a computer with a broken log-in screen.

Awesome. Truly fucking awesome.

Let me be painfully clear here. I used the Windows Control Center to
remove VeriFace.  I had full admin rights to the system. VeriFace is
fundamentally broken because it is impossible to cleanly remove the
software via the Windows Control Panel which is the platform-defined
method for software removal. This software was not properly QA'd or it
was released before it was ready by a mid-level manager with an itchy
shipper finger.

Considering the other recent Lenovo software flaps, I will no longer
use a Lenovo computer unless I know for a fact the computer has been
wiped and rebuilt AFTER purchase. If you want to use a ThinkPad (many
do), be prepared to reinstall the OS yourself or hire someone you
trust to do it for you. DO NOT TRUST LENOVO. They are going to put
some shit in there. I recommend you replace Windows with Linux, but
that is another screed. A clean Windows installation is superior to
ANYTHING shipped by Lenovo.

Note: The G-series laptop is not a ThinkPad, but I have loved
ThinkPads for a long time. One of the best computers I ever owned was
a ThinkPad and my wife uses a Lenovo U310 as her daily driver. But it
is running Kubuntu. Not the broken version of Windows distributed by
Lenovo. If you love somebody, replace their Lenovo OS with something
clean.

I did ask Lenovo for customer service, but the server refused to
accept my request. I received several SQL errors for my effort. All I
wanted to know was where I needed to go to download an executable to
re-install VeriFace. I never found it.

In fact, I wasted hours of my weekend looking for the software. I was
unable to find a version of Veriface that would run on Win7. Microsoft
continues to support Win7. Lenovo no longer supports VeriFace on
Win7. Unsupported software tied to something as critical as the log-in
screen is unacceptable. If Lenovo is unwilling to provide ongoing
support and updates to such critical software, it should NEVER
distribute it in the first place. I continue to suspect someone has an
itchy shipper finger.

In the end, I found a regedit hack on the Lenovo Forums. Fortunately,
it worked. To the fine people in the Lenovo Forums, I say THANK YOU!
To everyone else, I'm going to start saying Dell. Dell doesn't build
anything as awesome as a ThinkPad but it doesn't force any software
down my throat as bad as VeriFace. Thank you Michael. Thank you. I
promise to replace the U310 with a Laptop, especially if you expand
the selection of Dells that ship with Linux pre-installed.
