# DeGoogYourself
How did *you* end up here?

Not, [Here](github.com), but rather, to the conclusion that you were *too* dependendent on Google.

I came here in the aftermath of the 2016 US Presidential election, when I deleted my social media accounts.  All but one proved fairly simple.

Google.

Not through any dark patterns or for lack of customer service, rather, Google is *so* convenient it is nearly impossible to give up.

However, I've mostly migrated away.

I understand that I don't control the radio/modem in my device, and so, obviously, [NSA](https://github.com/nationalsecurityagency) has already pwned me.  Yeah. I know.  I'd just rather keep it to them.

By far the most difficult services (for me) to ditch have been Google Play Services, Google Maps, and Google Photos.

Google Play services is built into Android in a way that makes it *very* difficult to do without, despite not being part of the core OS.

Google Maps is *so* reliable, in such a profound way, it has put its competitors out of business one by one.  The fact that it is still free for the most part is mind-boggling.  *StreetView*. There is Apple maps, if you care for that flavor, but offline, in-dash navigation from the likes of TomTom and Garmin are completely gone.  This cannot be blamed on COVID; the most recent head unit with an offline navigation function was a 2014 Sony SKU.

(Yes there are little screens you can suction cup to your dash, but built in stuff has totally disappeared and been replaced with Android Auto and Apple CarPlay.

Google Photos is peerless.  I can browse my entire photo library on a phone I've just logged into without having to cache the entire library first.  I dunno how they do it.  Unbelievably local CDN's I imagine.  No other solution I've tried has come close to Google Photo's ability to offer frictionless backup, and seamless galleries. Ditching this app has put, not a *dent*, but a near ***total stop*** on my pocketcam photo output.  I don't take pictures any more in the same way, because I know it will be difficult to back them up, browse them, and share them.  I miss this on a visceral level.

In the secondary tier are GMail, Google Contacts, Google Calendar, Google Drive, YouTube, and Translate.

I was never really into the social aspects of the platform; I just appreciated the easy, frictionless backup and sync.

I recognize that this is not comprehensive. I'm not even sure if it's that useful.  But I'd rather do something than nothing, and I'm not willing to give up the connectivity.

I've been on a quest now for 7 years to rid myself of this dependency. This is my story:

# Get a cell phone that has official support from LineageOS

This is not as easy as it looks.  You need a Carrier Unlocked device. There are hacks to unlock locked devices - and they are cheaper - but it always complicates things.  In the interest of readability and brevity I'm writing about unlocked devices.

Devices from (ironically) Google, Sony, Samsung, Oneplus, and Motorola are decent bets but always check https://wiki.lineageos.org/devices/ first. LineageOS won't sort by "Last Added" which is very annoying.

Ideally, try the oldest supported version first, since it is usually the most stable. You might need to 'downgrade' your device if it has the 'wrong' updates that are incompatible with LineageOS.

I chose an unlocked OnePlus Nord N200.  I'm currently a version behind (19.1), since, although considered "stable", the current build (20.0) has problems with BlueTooth, phone calls, and reading from the sd card. It's a good idea to wait for that ".1" if you care about actually being able to use your phone vs. just-testing-things-out.

# Backup
If you're coming from a device that you're currently daily driving, here are some good things to backup.

Before you backup, disable Wifi and remove the simcard to avoid overlapping sync issues!

**remove the sim card!!**

Backup sms, mms, call log, 2FA, OPML, and NewPipe, along with anything else you keep locally on the device, like photos or downloads

Refresh login to nextcloud and bitwarden on separate machine for backup purposes

# Test

**This is nearly impossible to do without fucking up the backups you just made.  It at all posible, use a differnt sim.**

If a working build is found (There is no "Else" here, if there's no build, you fucked up the step where you acquire a compatible device):

Get the [MicroG for LineageOS](https://lineage.microg.org/) latest build of the one that worked

Use [payload-dumper-go](https://github.com/ssut/payload-dumper-go) to extract neccesary flash components

Follow [Lineage install instructions](https://wiki.lineageos.org/devices/dre/install) (**FOR Unlocked OnePlus Nord N200 ONLY!!  FOLLOW THE INSTRUCTIONS FOR YOUR DEVICE!!** )

## Test lineage

sms, wifi, phone calls, coverage, sdcard, crashes

# Minimal Setup

If LineageOS works, we will now modify it.  It will get erased a couple times, so do not restore/delete backups yet.

enable ADB

Install Magisk

Mod boot.img

move modded boot to host

Flash modded boot

Turn on Zygisk and Reboot

Setup MicroG

Allow display over other apps

Setup location providers

Give Mozilla location provider Special permissions

install Universal Safety net fix magisk mod

## Base System is Installed and will not be erased or reset again!!

install aurora services mod

install sms restore

restore sms and calls

install bitwarden

Install and restore aegis TractorFive$

install nextcloud

Install Dav5x client

install ical client

install fennec b4 Dav client and set as default!

Sync contacts and calender

## Personal Apps

install and setup protonmail

Install and setup K9

Install and setup phone track

Install and setup Nextcloud notes

Install and setup Discord

Feedly

Antennapod

AdAway

NewPipe

OSM And+
