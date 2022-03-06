---
layout: page
title: From idea to cartridge
---
## Preface

December 24, 2000. It's my 10th birthday. Finally comes the presents time, and
at last, my grandma is passing me over this big box, puzzling me with what could
ever be inside. Could I imagine at the time that by opening it, my life will be
changed forever?

Inside that box there was a Nintendo Entertainment System, or to be precise, an
unlicensed taiwanese [famiclone](https://en.wikipedia.org/wiki/Famiclone) called
Dendy. From the instant I plugged it to the TV, countless hours passed by as a
blink of an eye. All hopes for me to become a doctor, an astronaut or a
record-breaking athlete were gone forever. By the moment I finished my first
game, Contra, I was dead sure that I wanted to become a game developer. I had no
clue how and when and what was the magic that made the characters respond to
button presses and moved the projectiles around. Hell, I didn't even knew that a
profession such as "game developer" existed! But I was super determined to
master this wizardry and one day, make my own game.

Years passed by, and here I am, 31 y.o. at the moment of writing, Solution
Architect in a huge AAA gamedev company. There are millions of active players
enjoying our 3D ultra-realistic MMO action shooter. But the dream of making my
own game for that 8-bit console that shaped my life, is still waiting in the
box.

Now, it's time to open it.

## Making a game for the NES
This is a first article of a series, in which I'll show in detail how to make a
simple, yet complete game for the Nintendo Entertainment System, starting by
drafting the idea and going all the way to flashing the final game ROM to a real
cartridge, in quite a unique gamedev experience that will teach you a lot about
hardware, optimizations and clever hacks.

I must be honest with you - it won't be easy and it will take time. Game
development is a complex craftmanship that requires knowledge and skills in a
lot of CS fields and remains hard even today, with the availability of
sophisticated game engines, powerful hardware, lots of tools that automate
routine work for us, libraries and frameworks, all supported by modern operating
systems. Developing a game for an old 8-bit console, which processing power is
outperformed by orders of magnitude by even the cheapest modern smartwatch, is
going to be a challenge. We have just 2KiB of RAM, no operating system, no SDKs
or high-level programming languages, no primitives for drawing stuff on the
screen or reading input. We have just the raw hardware and we must speak to it
with the only language it understands: assembly.

Despite the fact that the NES is almost 40 years old, a lot of the things you'll
learn are still applicable today. The 6502 assembly language for instance, which
we'll use to program the NES, was meant to be written by humans and is
dead-simple, especially if compared to the ultra-complex x86-64 assembly of the
modern multi-core CPUs. Being able to understand how the CPU works and to
program it in assembly is a rare skill that few developers possess today and
it's far from being useless or obsolete. Your programming in high-level
languages will benefit a lot from it too: once you grasp the understanding of
the low-level hardware operation, you will intuitively start writing more
efficient code in C, C++ and even scripted languages. Sometimes, assembly is the
only tool at your hand, for example, when reverse-engeneering programs without
original source code or when debugging some obscure crash on a release build
without debug symbols. In order to show something on the screen and play some
sound effects, you'll communicate with the console's graphics and audio chips
and read buttons from the gamepads by doing I/O via memory-mapped registers, a
thing that virtually all modern device drivers do. A much funnier way to learn
hardware programming, than diving head-first into the Windows Driver Frameworks
API, isn't it?

During the development process, I'll make use of some existing tools, made by
the big community of enthusiasts for aiding in NES development (commonly called
*NESdev*), others will be made from scratch by me for this project. For example,
the music will be composed using existing tools, such as
[FamiTracker](http://famitracker.com/), but for building the game levels I'll
make my own level editor, tailored specifically for this game.

All the software and assets I'm going to make throughout this series, including
the game, will be made open source and available on GitHub, so you can explore
and tweak it at your will, for own fun and experiments.

Let's get started!

Read next: [Shoot'em Up! - the game](/nesdev/02-the-game)
