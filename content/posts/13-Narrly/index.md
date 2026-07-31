---
layout: page
permalink: ""
title: "Narrly There 🏄"
date: 2026-07-31
draft: true
thumbnail: "images/narrly-thumb.png"
showAuthor: true
showDate: true
showReadingTime: true
showSummary: true
summary: "Introducing Narrly, a side project that came out of a good friend describing the same repetitive job on every project he works on."
showComments: true
showTableOfContents: true
---

![Pixel art of a surfer riding a wave, the Narrly mascot](images/narrly-thumb.png)

I've always been interested in seeking side projects that are interesting, and solve real world problems. Although like many engineers
there's many a side project on the shelf at any time. However this article is a little different, and introduces a project I'm proud of. 

Oh, and one that works well!

## Where It Started

This all started with a friend mine Ross Martin. Ross and I go back to the University of Huddersfield, and he's the same good friend I built 
[DartsNow](/projects/1-dartsnow/) with through the pandemic. So we've got form for this sort of thing and work well together.

Ross is a freelance editor and colourist, with a wide array of experience across TV & Film space. A while back he 
was telling me about a chunk of his week that he described, roughly, as an hour of his life he'd like back. Every time. On every project.

Ross walked me through it properly, mostly because I was being nosey. But I'd also been whittering on to Ross about having a crack at building
something new. With some of the new AI capabilities I was confident we could give something a punt, and it turns out the problem itself is
straightforward. It's just repetitive, and there's a lot of it.

## Guide, Master, and a Lot of Scrubbing

For anyone who's never been near an edit suite here's the shape of it.

When you're cutting a video, you usually put a rough voiceover down on the timeline first. A scratch track. It's not the 
one that ends up in the finished thing, it just gives you something to cut the pictures against. That's the **Guide**.

Later, the proper voiceover gets recorded in a session. One long recording, the script read from top to bottom, with 
retakes, coughs, false starts, "sorry, can I go again", the lot. That's the **Master**.

Now the fun bit. Someone has to go through that long Master recording, find the take that matches the first line on the 
timeline, drag it into position, and then do exactly the same for the second line. And the third. And every line after that, for as long as the script is.

It's not particularly hard work. That's what makes it so annoying. It's just scrubbing, squinting at waveforms, and dragging, over 
and over, and any editor with a deadline is doing it when they'd rather be doing the actual editing.

## So We Built Narrly

Narrly does that matching bit for you.

You drop in your Guide and your Master, and it works out which takes in the Master belong to which 
lines in your Guide. You get back a multi-track WAV with your Guide on the first channel and the takes stacked above it,
each one sat at the right point on the timeline. Import it like any other file, then mute, solo and cut as normal.

Alternatively you can export a single-track, which is Narrlys combination of the best matched
takes. Interested to see how much this option gets used, but it's there if required.

That's it. It's not trying to edit your video, and it isn't going to write your script. It does the repetitive part and 
then gets out of the way.

Under the bonnet there's a web app, a backend, and a chunk of audio processing doing the heavy lifting. I'll leave it 
there for now, partly because the interesting bits deserve a post of their own, and partly because we're still working on refining 
it all.

## Shipping It

It would be hard to not include that using LLM's has enabled me to work faster, albeit in areas. It's not all been smooth sailing though, it's certainly 
created a mess that's hard to be untangled as well. I wanted this to be built in technologies that I could still 
step into, still be able to wrestle with when I eventually hit the usage limits. 

It terms of making it look professional, it's all tied up with: a domain. a terms page. A privacy policy that I actually 
had to sit, review and think about, because people are uploading work that isn't theirs to give away. Deciding what happens to those files
(they're processed on our own kit in the EU, they never go near a third-party AI platform, and they're binned when you close the tab).
Writing an FAQ in plain English rather than the version I'd write for another engineer, after all it isn't a purely technical write up.

There's no sign-up, no login, and we don't ask for your name or your email. It's free while it's in early access,
mostly because it's early and early feedback is valuable right now.

None of that is glamorous. All of it took longer than I expected too! Because I want to be confident in the outcome we ship. I want to confidently
stand behind the stack, know it inside and out and have confidence that it still solves the problem at hand.

## A Head Start, Not a Finished Edit

Narrly won't place every take perfectly, and it isn't meant to make the final 
call. It shows you what it found before you download anything, so nothing quietly disappears on you, and you should
still check the output before you rely on it for something that matters.

It's meant to save you the repetitive part of the job. That's the whole pitch in a nutshell.

## Give It a Go

It's live at [narrly.tech](https://narrly.tech). Drop two files in and see what comes back.

If you edit video and it's rubbish for your workflow, I genuinely want to hear about it. You can reach me at [hello@jamesmillner.dev](mailto:hello@jamesmillner.dev).
