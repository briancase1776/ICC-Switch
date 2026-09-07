# ICC-Switch

A name held open. There is no design here yet, and that is deliberate.

## The idea, as far as it got

A fitting with one inlet and exactly two outlets, taking **one** pattern.
What matches goes down the first outlet; what does not goes down the
second. Not a filter that drops — a partition. Nothing on the wire
vanishes, and the invariant is structural rather than promised: for every
payload in, exactly one payload out.

One pattern, not two. The fitting derives the second leg by negation.
Given two patterns trusted to be complements, a payload matching neither
is lost and one matching both is duplicated, silently and depending on
the data.

Binary, and chainable. No single fitting picks from a list of
destinations; it answers yes or no about outlets fixed by the wiring. A
switch, not a router — SPDT, not Ethernet.

It came up looking for a gate: a station on the wire that could enforce
form without ever touching content.

## Why it may not need to exist

Two things came out of thinking about it that argue against building
anything here at all.

**A gate can be a party rather than a fitting.** Reading and deciding is
something no fitting may do — but parties read; that is what parties are
for. A doorman sits at a seat in the map like anyone else, holding an end
in and two ends out, and writes to one of them. No new fitting, no
inspection anywhere in the plumbing, and the bay already knows how to
seat a party.

**And the deciding may be address bits rather than content.** If a party
writes to the end that goes where it wants, nothing in the middle has to
read anything, and the shape decides the cables as it always has.

## What would have to be true before building it

Something has to want a partition that a party cannot do for itself, and
there has to be a second caller for it. Neither is true today.

## Where the thinking is

- [ICC-Tee#1](https://github.com/briancase1776/ICC-Tee/issues/1) — why the
  split is not a tee, and the layer problem that raised
- [Moot#28](https://github.com/briancase1776/Moot/issues/28) — the control
  pair, which is where a refusal would have a leg to travel down

There is no CLAUDE.md here. Writing one would mean inventing the design
this repo does not have.

## Licence

MIT. See LICENCE.TXT.
