---
layout: page
title: Reconnaissance
---
The first step before attempting any attack and starting exploiting is
information gathering, i.e reconnaissance, aka _recon_.

It should be done as more passively as possible, trying to not leave any
footprints and warnings about the upcoming attack and thus be performed
silently, gathering information from open sources such as DNS servers, Google,
social media, the actual target websites, etc.

Every bit of information counts, as you can infer from it details about possible
account names, organization structure, network topology, servers and operating
systems, etc.

## Common vectors

* Who are the people? Do they have an "About Us" page? Sure they do. Are they
  present on some socials? Sure they are. Every bit of info could be useful for
  social engineering attempts later. Names, email addresses, phone numbers,
  social profiles, sportclubs, subscriptions, etc. Humans are the weakest point
  in the security system.
* Who is servicing them? Hosting, website development, CDN, mail servers, etc.
  Maybe the webmaster uses the same wordpress constructor over and over again,
  not even the most up-to-date? Maybe the hosting provider has some free hosting
  plans, that you can try and infer a great detail of information?
* Who they are hiring? Maybe some open positions on Linkedin? Those could reveal
  precious information about what technologies are used in the infrastructure,
  and even reveal some problematic areas, that need to be addressed.


## Tools
Before starting recon ops, obtain the highest level of anonymity possible, by
using a VPN, a proxy or Tor. Or all three. You must not leave traces.

* [Google](https://google.com) - Your best friend.
* [viewdns.info](https://viewdns.info) - A collection of tools for looking up
  IP, DNS, MX records and more.
* [centralops.net](https://centralops.net) - Dossier building tools for quick
  recon, that use nslookup, dig, traceroute, etc under the hood.
