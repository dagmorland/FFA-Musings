[*Back home*](index)

# The Glitches

This section documents every glitch fixed in the [RAI Project](rai).

## Trigger Tile Bugs
A trigger tile is a visible or invisible metatile (16x16 px block) that either
causes damage from spikes/lava, or more importantly executes internal scripts
like 'load a new room' or 'reveal a staircase'. There are multiple ways trigger
tiles can be skipped, which leads to warps, or puzzles that have to be reloaded.

<div style="border: 1px solid #e1e4e8; padding: 20px; border-radius: 6px; background-color: #f6f8fa; margin-bottom: 20px;">

### Trigger Tile Misses from 8 Pixel Snapping

#### Synopsis

Because the game operates on an 8 pixel grid, sometimes the game will call a
function to snap an 'actor' (a player, an enemy, an NPC, or even snowmen and
chests) back on to the grid. This happens for players when they return from
invincibility frames to a normal condition (i.e., a few seconds after being
injured). This also happens for non-player actors when their current action
(e.g., move up, move left, shimmy in place) ends. Ironically, even
Ice-magic-induced snowmen and empty chests have actions. These actions do
nothing, but they still do the nothing action and then snap to the nearest 8
pixel boundary. This is why pushing snowmen/chests often looks jittery -
they're snapping to a boundary every couple seconds. Unfortunately, the
function that snaps an actor back on grid also skips checking if they were
snapped to a trigger tile.

#### Origin

This was the first glitch I encountered as a 7 year-old in 1992. While chasing
down 'Man' in Wendel, I got hit by a rabite and was knocked back to the
previous screen.  While having invincibility frames, I tried going back south
into Wendel, but instead wound up warping to the Mana Shrine because I missed
the trigger tile. This glitch is also the reason for one of the most common
annoyances in FFA: puzzle room failures.  The speedrun community has plenty of
horror stories of completing a snowman puzzle room only for the staircase to
not appear. It's not *always* this bugs fault, but it *usually* is.

#### Rationale to Fix

Ishii-san certainly would not have wanted players to struggle with puzzle rooms
even when performed correctly, nor would he have wanted players to warp around
without reason.

#### Possible Exploits

There are not many places the player can use this to their advantage. The
Wendel to Mana Shrine warp is not positioned to allow the player to continue in
the Mana Shrine... it's a dead end. I'm sure there are other potential places
to exploit this, but given the difficulty to pull this off, and requiring to
get hurt beforehand, they aren't currently being used in the speedrunning
community. As for snowmen/chests not triggering puzzle tiles, that's just
annoying, not exploitable.

#### Example

Completing a puzzle that doesn't work like it should.
Warping from Wendel to the Mana Shrine.

</div>

![Under Construction](img/coffee_break.gif)
