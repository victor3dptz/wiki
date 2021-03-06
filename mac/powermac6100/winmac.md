---
layout: page
title: Windows Interoperability
---

![Logo](/mac/powermac6100/img/11winmac.gif)

### Introduction

Painful as it is to see, the computing world is dominated by Windows machines. Although we Mac users may choose not to work with these machines, we can't avoid working with their owners. On the plus side, developments over the past 5 years have made this easier than ever. We can share files, applications, peripherals, and even operating systems with PC owners.

Note that this section is titled "interoperability" rather than "compatibility." The distinction is subtle, but important. I'm less interested in running the Windows OS or Windows application on my Mac; what I'm really interested in is surviving amongst the Wintel herd. After all, if I can use the same files, same peripherals, and same websites, then I can co-exist despite having a superior machine :)

### Files

Many data files from PCs can be used just fine on a Macintosh. In most cases, data is data, and you need accomplish only two things in order to use a PC file &em; move the file and find a compatible application.

There are some technical differences between data file structures between Macs and PCs (primarily character set issues), but most modern applications are smart enough to handle the differences or make the appropriate conversions.

The three primary ways to share files with PCs are email, disks and networking.

Email is one of the easiest ways to share small files, especially if the machines are not physically proximate. Most common data files will survive transmission via email. Just use the Attachment feature of your email program (usually they have a paper clip button or icon) to attach the file to any email, and the recipient should be able to open the attachment with a compatible application.

### Disks

Of course email can be less practical if the files are larger than a megabyte or so. "Sneakernet" is a common term for the next most common way of sharing files &emdsh; putting files on a removable disk of some type and walking to the next room with it.

Sneakernet is most commonly used in reference to floppy disks, but CDs, Zip disks, Jaz disks, Syquest disks, etc. can be used cross-platform as well.

A file created on a Mac has invisible "TYPE" and "Creator" codes which tell the Finder which application to use if you double-click on it. A file created on a PC has a three letter extension (e.g. .txt, .xls, .doc) which allows Windows to figure things out.

Apple has bundled software called File Exchange (previously PC Exchange) with every version of the Mac OS since the early 7's. This software allows the Mac OS to recognize PC/DOS formatted media (disks) and also helps the OS determine which type of file is represented by which DOS extension(s). If, for some reason, File Exchange isn't doing it's job, and you get an error when you double-click a PC/DOS file, you can usually open it from within the application (using File:Open) or by dragging and dropping the file's icon onto the application's icon.

To use a Mac file on a PC, you can usually just add the appropriate extension onto the filename, and then copy the file onto a PC formatted disk.

Earlier versions of Iomega's free Zip Tools didn't allow a Mac user to reformated at Zip disk in DOS format, but the most current version has fixed this oversight.

### Networking

The easiest way to share files and services is over a network. Obviously, network administration is complicated enough to be the foundation of a job, career, company, or entire industry, so I can't cover more than a smidgen here. But I can at least go over the very basics as they relate to Mac and PC interoperability:

* **Wires** - Almost all networks require some sort of wire to connect the connected computers. The most common kind of network wiring is Ethernet. There are several types of Ethernet, but by far the most common is 10BaseT. See my basic Networking page for details on using or installing Ethernet on your computer. You can also connect Macs and PCs using TokenRing, serial cables, telephone cables, and wireless LANs (this is very cool).
* **Protocols** - After you have physically linked the machines over some sort of network medium (e.g. wires or wireless), the two machines have to "talk" the same protocol. There are three major protocols (or protocol sets) that PCs and Macs can use to talk to each other:
  * **AppleTalk** - A proprietary Apple protocol that comes preinstalled on every Mac. You can make your PC speak AppleTalk by installing Miramar System's PC MacLAN or Thursby System's TSSTalk (formerly COPSTalk). I use PC MacLAN on my IBM ThinkPad, and it works just fine.
  * **TCP/IP** - The lingua franca upon which the entire Internet runs, TCP/IP is preinstalled on every computer made in the last five years. Configuration is somewhat complicated, but I have a separate page devoted to that. TCP/IP isn't quite enough to enable full-fledged filesharing, though, so you probably will want to buy Thursby's DAVE. If you insist on doing this for free, you can mess around with FTP/HTTP as described on my networking page.
  * **IPX** - Novell's proprietary system for networks. IPX requires a server to manage the network, which means that you can't just set up two machines to talk to each other without spending some serious money. I won't go into how to set up IPX, since I don't know how, but I will tell you where you can download a free version of the Novell client for Mac OS.
  * **Other?** - There may be other protocols that you can use, but I don't know much about them, and they're not likely to be widely available or easy to use. 
* **File Sharing Systems** - I'm probably not using the correct technical term here, but there's more to filesharing than just the protocol. Once you have the machines speaking to each other, they still have to share information about what files are stored where, what permissions each user has, etc. Windows and Mac OS each have their own systems, and they are not compatible out of the box. If you have one Mac and many PCs, you probably want to use DAVE. If you have one PC and many Macs, you probably want to install TSSTalk or PC MacLAN. If you have Windows NT Server, it comes bundled with Services For Macintosh, but you have to install it manually. 

### Applications

Most comparisons/holy-wars about Macs vs. PCs include some mention of the vast differential in the number of applications available for each platform. The truth is, for most users, you can obtain most of the same functionality on a Mac as you can on a PC:

* **Office suites** - Microsoft Office is the de facto standard in the American corporate world, and Microsoft has committed to publishing a Mac version for at least the next 3 years. Their current version is quite good on balance. It lacks some Windows features, and definitely runs slower, but it also has some neat Mac-only features such as auto-repair and drag-and-drop installation. There is some competition for productivity apps, such as the beta WordPerfect from Corel, and the upcoming (free!!) Star Office from Sun
* **2D graphics** - I'm no expert here, but industry is ruled by Adobe, and Adobe loves the Mac. PhotoShop, Illustrator, Acrobat, and all of Adobe's major apps will run on the Mac for the foreseeable future. Adobe CEO Bruce Chizen has gone on record to say that Adobe is "absolutely committed to OS X."
* **3D graphics** - I know very little about this space, but Apple's adoption of OpenGL and AGP have done wonders to garnering OEM support for 3D hardware on the Mac. The recent decision by Maya to offer ???? for the Mac may be a bellwether for the rest of the 3D industry, inciting other software companies and high-end graphics card manufacturers to start supporting the Mac. The introduction of ATI's Radeon and the recent noise by 3dfx and Nvidia are encouraging signs that we are second-class citizens no longer!
* **Games** - What's good for 3D graphics is obviously good for gaming, especially in conjunction with Apple's adoption of USB for game controllers. Although the Mac historically has lagged severely in the game space, we're catching up fast. Quake 3 Arena was released simultaneously for Windows, Mac OS and Linux, and more and more companies are jumping on the Mac bandwagon. We'll see about former Mac stalwart Bungie, but the future of Mac gaming looks better now than it ever has.
* **Internet tools** - The Mac OS has pretty darn good parity here. Mac users can get browsers, FTP tools, network analysis tools, email apps, videoconferencing, etc. that are feature competitive with just about anything on the Windows side. With the exception of Microsoft NetMeeting, the Internet is pretty much platform- and application-agnostic.
* **CAD/Engineering** - The Mac platform has some serious catch-up to do here. AutoCAD will probably never make it to the Mac, which makes it difficult to work in a PC-dominated environment. There are CAD apps for the Mac, and most of them can be made to work with AutoCAD files, but the Mac is still at a disadvantage here. Advances in Mac 3D may help drive some CAD and engineering software development but there have been few significant announcements in this area.
* **Databases** - Another major weak point. Microsoft Access will never be ported to the Mac. FileMaker is a pretty good little database, but it won't do what Access does, and there are lots of small- and mid-size business tools that are built on top of Access.
* **SOHO accounting** - There's a mixed bag here. There are few options, but there is still an imbalance that is serious enough to be worrisome. QuickBooks hasn't been updated in ages, despite that Intuit CEO Bill Campbell is on Apple's Board of Directors, and the current version can't even share files with the Windows version. There are other alternatives such as MYOB listed on Apple's website, but precious few of them are truly cross-platform.
* **Enterprise accounting** - A sorry state, but with a promising future. Although most ERP systems aren't very Mac friendly (if not downright hostile), there is also a burgeoning movement towards running ERP systems over browsers. Once that happens, the Mac should be at parity almost instantly. Lots of other major enterprise apps are Unix-based, and should port to Mac OS X fairly easily. 

Actually that last point is critical for several classes of apps beyond accounting. Many analysts see the "hosted" application model as the future of desktop computing, and many companies are betting their futures on it. If it becomes reality, then Mac application parity will take a large step forward indeed.

Of course processor-intensive apps (e.g. graphics, games and CAD) will remain local for a good long time (possibly forever), but the Mac is already at parity or making great strides in some of these areas already.

### The Web

The beauty of the Internet is that it's supposed to be platform agnostic. Most of the browsers in the world run on Windows 95 or 98, but most of the servers in the world do not. This is usually invisible to the user, since all modern computers speak the same TCP/IP, HTTP and HTML. With a few exceptions, what you can view on your PC I can view on my Mac.

Of course nothing ever really achieves the ideal, and there are some plugins and browser features that don't correspond exactly across the two major desktop platforms.

### Peripherals

By peripherals, I generally mean anything and everything external that gets plugged into your computer:

* **Diplays** - There has been 99% parity here for quite some time. With very rare exceptions (such as the Apple Portrait Display and some modern digital flat-panel displays), any Mac and any PC can use just about any monitor
* **Input devices** - With Apple's universal adoption of USB, compatibility for mice, trackballs, keyboards, game controllers and webcams has never been better. The only requirement for cross-platform compatibility is that the manufacturer write a Mac OS driver. Even for devices that don't have a manufacturer's driver, shareware drivers such as USB Overdrive can enable them to work on the Mac. This is no good for 6100 owners like us, but at least we can look forward to our next Mac :). Even before that, there are some decent options. For keyboards and mice, GeeThree makes an ADB-PS2 adapter. Several decent webcams like the QuickCam were once offered in ADB versions, and these can still be found on ebay and in Mac catalogs. For game controllers, the JoyPort allows many PC game controllers to be used with an older Mac.
* **External storage** - See the Disks section.
* **Printers** - Most network printers have Mac drivers available for them, and most of the newer local (i.e. non-networked) printers have USB and Mac drivers. For older printers and (more importantly, for 6100 owners), Infowave's PowerPrint is a Mac serial-PC parallel adapter with bundled drivers for thousands of printers.
* **Scanners** - Most older scanners were offered in a SCSI version with Mac drivers. Newer scanners are USB or FireWire, which puts them out of reach for 6100 owners but makes them perfect for owners of modern Macs. 

### Upgrade cards

There's no good news here for 6100 owners. Nubus and PDS are, for all practical purposes, Mac-only, and there's no crossover or compatibility.

But for modern Mac owners (PCI or newer), many of the upgrade cards for PCs can also be used on your Mac. PCI is PCI and AGP is AGP, so all they require are software drivers and sometimes (for video cards), a flashable BIOS. Many VooDoo cards can be flashed with a Mac BIOS and used with public beta drivers from 3DFX. Likewise, many Fast Ethernet and Gigabit Ethernet cards are available with Mac drivers.

Apple's recent success and their continued adoption of key standards like 2x AGP and 4x AGP will make card compatibility better and better. There are persistent rumors of high-end 3D card manufacturers coming to the Mac very soon.


