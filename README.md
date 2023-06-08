# DeGoogYourself
Delete Google from your life


how to degoog your life as much as possible

How did *you* end up here?

I came here in the aftermath of the 2016 US Presidential election, when I deleted my social media accounts.  All but one proved fairly simple.

Google.

Not through any dark patterns or for lack of customer service, rather, Google is *so* convenient it is nearly impossible to give up.

However, I've mostly migrated away.

I understand that I don't control the radio/modem and so, obviously, NSA has already pwned me.  Yeah. I know.  I'd just rather keep it to them.

By far the most difficult services (for me) to ditch have been Google Play Services, Google Maps, and Google Photos.

Google Play services is built into Android in a way that makes it *very* difficult to do without, despite not being part of the core OS.

Google Maps is so reliable, in such a profound way, it has put its competitors out of business one by one.  There is Apple maps, if you care for that flavor, but offline, in-dash navigation from the likes of TomTom and Garmin are completely gone.  This cannot be blamed on COVID; the most recent head unit with an offline navigation function was a 2014 Sony SKU.

Google Photos is peerless.  I can browse my entire photo library on a phone I've just logged into without having to cache the entire library first.  I dunno how they do it.  Unbelievably local CDN's I imagine.  No other solution I've tried has come close to Google Photo's ability to offer frictionless backup, and seamless galleries. Ditching this app has put, not a dent, but a near stop on my pocketcam photo output.  I don't take pictures any more in the same way, because I know it will be difficult to back them up, browse them, and share them.

In the secondary tier are GMail, Google Contacts, Google Calendar, Google Drive, YouTube, and Translate.

I've been on a quest now for 7 years to rid myself of this dependency.

Here is my story:

Get a cell phone that has official support from LineageOS

Devices from Google (ironically), Sony, Samsung, Oneplus, and Motorola are decent bets but check https://wiki.lineageos.org/devices/ first.

Ideally, try the oldest initial version first, since it is usually the most stable.

I chose a OnePlus Nord N200.  I'm currently a version behind (19.1), since, although considered "stable", the current build (20.0) has problems with BlueTooth, phone calls, and reading from the sd card. It's a good idea to wait for that ".1" if you care about actually being able to use your phone vs. just-testing-things-out.

If you're coming from a device that you're currently deaily driving, here are some good things to backup before you backup, disable Wifi and remove the simcard to avoid overlapping sync issues.

remove sim!

backup sms, mms, calls, 2FA, OPML, and NewPipe

Refresh login to nextcloud and bitwarden on separate machine for backup purposes

Test lineage
sms, wifi, phone calls, coverage, sdcard, crashes

if a working one is found

Get the MicroG for LineageOS latest build of the one that worked

Use payload-dumper-go to extract neccesary flash components

Follow Lineage install instructions

minimal setup

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
