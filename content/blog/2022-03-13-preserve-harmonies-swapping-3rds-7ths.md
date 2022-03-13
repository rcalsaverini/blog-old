---
title: Does swapping 3rds and 7ths preserve harmonic feel?
slug: preserve-harmonies-swapping-3rds-7ths
description: Do chords that swapp thirds and sevenths retain the same "harmonic feel"
author: Rafael S. Calsaverini
date: 2022-03-13T17:15:22.675Z
lastmod: 2022-03-13T20:28:30.099Z
draft: true
tags:
  - Music Theory
  - Negative Harmony
  - Chord transformations

categories:
  - music-theory
---

The ii-V-I chord changes are arguably the most basic stable of jazz harmony, and exploring what's so compelling about this chord is always a good way to diving into what's harmony in jazz is all about. Recently the youtuber [Charles Cornell](https://www.youtube.com/channel/UC4PIiYewI1YGyiZvgNlJNrA) published a [nice video](https://www.youtube.com/watch?v=alsQOE0vuoc) in his channel exploring how ii-V-I changes in major have a very nice pattern of leading tones involving thirds and sevenths, and how this drives the harmony forward in such a compelling way, by stacking compelling resolutions that continuously release the tension built by moving the chords around.

To drive the explanation home, Cornell made a strong assertion: most or all of the actual harmonic juice of a chord, at least in the context of jazz harmony is contained in the third and seventh. To drive this home he shows live in the piano how, if you throw away the root and fifth and only play thirds and sevenths, most of the harmonic feel of the ii-V-I changes are retained [^footnote1].

Then, further in the video [^footnote2], Cornell points out that the resolution from ii to V and from V to I work by inverting the resolving the seventh down a half step into the third of the new chord. This also makes the third of the previous chord, that's kept as a kind of pedal point in the new chord, to become the new seventh. In summary: thirds becomes sevenths and sevenths resolve into thirds. And that's the basic mechanism of the most widespread harmonic language of jazz.

# Thirds and Sevenths

That's not something super new and surprising but I think Cornell makes a good job in simplifying it and making it very pedagogic. But his explanation kind of lead me to ask myself some questions. In particular, forgetting about the resolutions and leading tones a bit, if most of the taste and color of a chord is contained in the thirds and sevenths, what happens if I change the other notes around it?

I could start by taking a chord, stripping the root and fifth, and tacking on two other random notes there and see what happens. Right? Let's try.

<script>
  const f = new Vex.Flow.Factory({
    renderer: { elementId: "boo", width: 500, height: 200 },
  });

const score = f.EasyScore();
const system = f.System();

system
.addStave({
voices: [
score.voice(score.notes("C#5/q, B4, A4, G#4", { stem: "up" })),
score.voice(score.notes("C#4/h, C#4", { stem: "down" })),
],
})
.addClef("treble")
.addTimeSignature("4/4");

f.draw();
</script>
<div id="boo"></div>

[^footnote1]: See the demonstration on the first 1:30 minutes of the video.
[^footnote2]: See the explanation beggining in 6:29 minutes into the video.
