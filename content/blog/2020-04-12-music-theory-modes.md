---
title: Music theory musings - negative harmony and chirality.
date: 2017-04-12 00:00:00 -03:00
categories:
- music-theory
tags:
- Music Theory
- Negative Harmony
- Set Theory (Music)
author: Rafael S. Calsaverini
draft: false
---

Recently I've been listening to a [12tone video](https://www.youtube.com/watch?v=SF8CdxcdJgw) on YouTube about negative harmony, a concept recently popularized by musician Jacob Collier. On the related links I found a bunch of videos from [this channel](https://www.youtube.com/channel/UCurOAVtqb7kM1siNlDynzFw) with "negative harmony" versions of many popular songs. They have a quite interesting sonority to them, and it struck me that even though the original songs had very strongly major or minor melodies, the transformed melodies had a quality about them that suggest other modes. So, I started musing about it and a few things popped in my head, so this is a write up of some of the stuff I realized. 

## What is Negative Harmony anyway?

There are many ways to understand negative harmony and I'm not going to pretend I'm able to give a full historical background. The video by the 12tone channel that I linked above does a much better job than I ever could of explaining this in a more general setting. Here in this post I'm mainly interested in this as a transformation that can be applied to a particular piece of music and that's how I'm going to describe and treat it, although this is just a drop in the ocean of what negative harmony is about. 

To understand what's the transformation being applied, consider the circle of fifths:

{{<tikz>}}
\begin{tikzpicture}

\pgfmathsetmacro{\CircleRadius}{3.5}
\pgfmathsetmacro{\LabelRadius}{\CircleRadius * 0.9}

% THE GRID
\draw (0,0) circle (\CircleRadius);
\foreach \X in {1, 2, 3, 4, 5, 7, 8, 9, 10, 11}
    {
        \draw (0,0) --++ (75 - \X * 360 / 12 : \CircleRadius);
    }

    \draw [ultra thick, dashed] (0, 0) --++ (75 : \CircleRadius);
    \draw [ultra thick, dashed] (0, 0) --++ (75 - 180: \CircleRadius);

% OUTER LABELS    
\foreach \X/\KeyText in {-5/D$\flat$, -4/A$\flat$, -3/E$\flat$, -2/B$\flat$, -1/F, 0/C, 1/G, 2/D, 3/A, 4/E, 5/B, 6/F$\sharp$} 
    {
        \draw (90-\X*360/12:\LabelRadius) node {\KeyText};
    }

\end{tikzpicture}


{{</tikz>}}


Here I drew a line between the notes C and G, extending it to slice the circle in two. If we are in the key of C, the transformation that takes the original song to its "negative harmony" version is reflecting the notes through that line that cut between the root of the key and the fifth. If you do that, the notes are transformed as follows.