# The ROM-As-Intended Project

As an engineer and software developer, I have always been amazed (and jealous)
of the early cartridge and disc-based game releases.  As a development studio,
you had one shot to make the best game you could with the budget and time
provided. Once it shipped, that's that. Every now and then there could be one
or two (hardware) revisions released, but you can't recall or update what's
already in your customer's hands.  Likely all of the games from that era still
had glitches, but in my experience most were too arcane to reproduce naturally,
or otherwise didn't manifest noticeably in normal gameplay (kudos to the
testers back then).

Final Fantasy Adventure, as excellent as it is, is chockablock with glitches.
While I wholeheartedly appreciate the character infused by these lingering
issues, I wanted to create a version of the game that 'perfectly' reflected
Koichi Ishii-san's vision for Seiken Densetsu (the original Japanese name for
FFA).  The ROM As Intended (RAI) Project is thus a collection of glitch fixes
and curated improvements as part of an ongoing project to create a baseline ROM
patch for FFA. By design, there will be no creative additions outside of what
was expected to be the original director's intent. This patch includes two
parts:

1. **RAI-AR (at release)**: strictly focused on bug fixes that try to meet the
director's intended feature set on release. This includes things like warp
fixes, trigger tile glitches, and flaky PRNG.  2. **RAI-AD (at design)**: a set
of curated feature enhancements that try to capture the director's intent with
the game at the design review stage. This includes things like making the
follower leap with the player with chain pulls, removing the artificial gold
cap of 65535, and fixing the player/tile collision approach to be more logical.
The goal is not to make creative improvements, but rather finish the feature
list that was with little doubt 'intended' before the team ran out of time.
This patch sits on top of RAI-AR.

Let me acknowledge the elephant in the room: we don't know for sure what
Ishii-san's intent was over 30 years ago. That said, there are often context
clues within the code that make it clear whether a behavior was intended or
not. This is similar to determining "read-as-intended" for Dungeons & Dragons
rules, or even interpreting or translating ancient texts. As such, the RAI-AR
set of bug fixes aim to be rather indisputably "as intended".  The RAI-AD
curated feature enhancements are much less certain, and therefore are released
as a separate patch. The RAI project will likely never end. Glitches will
continue to be discovered as long as developers, speed runners, and casual
gamers continue to enjoy the game. 

# Development

This project uses a formalized process for making changes. Every update to
either RAI branch requires a pull request with certain details filled out,
including a matching linked Github Issue and thorough documentation on these
Github Pages site. Refer to the Github Readme in the
[RAI-AR](https://github.com/dagmorland/FFA-Musings/tree/raiar) and the
[RAI-AD](https://github.com/dagmorland/FFA-Musings/tree/raiad) branches for
details.

# Releases

I'm not there yet, but there will be releases posted through Github directly
and also to romhacking.net. I'll provide links once they are available.

**RAI Project patches require existing official ROM files. Support
Squaresoft!**

# RAI At Release Fixes

All fixes will be documented directly in the [Glitch Encyclopedia](glitch)

# RAI At Design Feature Enhancements

![Under Construction](img/coffee_break.gif)
