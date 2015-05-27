---
title: Thanks Lenovo, for truly crappy software.
author: Andy Choens
layout: post
category: bitching
excerpt: I recently rebuilt a Lenovo laptop for my 10 year old nephew. Hilarity ensued thanks to some terrible software from Lenovo.

---

I would like to personally thank Lenovo for making my Memorial Day
Weekend just a little less pleasant. I was asked by my wife's brother
and his wife to clean-up an older Lenovo laptop and prep it for their
10 year old son. In truth, I was looking forward to it. I saw this as
an opportunity to do something nice for my nephew AND I saw it as an
opportunity to give him some FOSS title like Krita, Celestia, etc.

Fun!

The laptop in question is a G560, running Win7. If asked, I would have
gladly replaced Windows with Linux, but that was not the request. I
cleaned up the accumulated malware, replaced the anti-virus and
generally tidied things up. Matt had also asked that I strip the
system down to base-windows. I decided this request included the
Lenovo-branded software that had come with the laptop.

This was where I erred. I assumed the Lenovo-branded software was
properly written. It wasn't.

The app VeriFace was my nemesis. Everything else removed itself from
the computer without causing problems. But Veriface would not go
away. After removing it via the Windows Control Center, it still
started up, sorta, when the computer booted and provided users with
two apparently separate methods to log into the computer. But, because
only a few parts of Veriface were still there, the VeriFace log-in
functionality was not completely broken.

Lenovo's application incompletely removed itself from the system and
left the system broken as a result. This is not normal behavior and I
am not criticizing it because it isn't open source. I am criticizing
it because it does NOT follow the standard Windows process for
application removal. VeriFace 3.16, the version of the software which
came with the computer had not seen and update in YEARS, even though
the forums are full of people struggling with this software.

To be blunt. This is alpha quality software that is able to break the
Windows log-in screen. Considering other recent Lenovo software flaps,
I would have to think long and hard about running their computers with
anything other than a freshly installed OS by myself or some other
trusted IT professional.

At this point in time, I can no longer recommend anyone buy and use
Lenovo computers, unless they are prepared to perform a fresh install
of their software. In doing so, I recommend Linux, but at least pay
for an independent and clean version of Windows if that is your thing.

I attempted to ask Lenovo for customer service, but their server
refused to accept my request. I kept getting SQL errors.

I attempted to download the installation executable from the Lenovo
website, but was unable to find a version of the software that would
run on Windows 7. Microsoft continues to support Win7. Lenovo does
not.

In the end, I found a regedit hack on the Lenovo Forums. Fortunately,
it worked. To the LF, I say THANK YOU!

To everyone else, I'm going to start saying Dell.
