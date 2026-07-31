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
summary: "Introducing Narrly, a side project that came out of watching a good friend do the same boring hour of work over and over again."
showComments: true
showTableOfContents: true
---

![Pixel art of a surfer riding a wave, the Narrly mascot](images/narrly-thumb.png)

Most of my side projects start with something I've been nosey about. A file format, a language I've not used, an API I fancied poking at. Narrly didn't. Narrly started with someone else moaning at me, and honestly, it's been all the better for it.

## The Boring Hour

That someone is Ross Martin. Ross and I go back to the University of Huddersfield, and he's the same good friend I built [DartsNow](/projects/1-dartsnow/) with through the pandemic. So we've got form for this sort of thing.

Ross edits video for a living, and a while back he was telling me about a chunk of his week that he described, roughly, as an hour of his life he'd like back. Every time. On every project.

I asked him to walk me through it properly, mostly because I was being nosey, and it turns out the problem is beautifully dull.

## Guide, Master, and a Lot of Scrubbing

For anyone who's never been near an edit suite (me, until recently), here's the shape of it.

When you're cutting a video, you usually put a rough voiceover down on the timeline first. A scratch track. It's not the one that ends up in the finished thing, it just gives you something to cut the pictures against. That's the **Guide**.

Later, the proper voiceover gets recorded in a session. One long recording, the script read from top to bottom, with retakes, coughs, false starts, "sorry, can I go again", the lot. That's the **Master**.

Now the fun bit. Someone has to go through that long Master recording, find the take that matches the first line on the timeline, drag it into position, and then do exactly the same for the second line. And the third. And every line after that, for as long as the script is.

It's not hard work. That's what makes it so annoying. It's just scrubbing, squinting at waveforms, and dragging, over and over, and any editor with a deadline is doing it when they'd rather be doing the actual editing.

Ross wasn't asking me to fix it. He was just complaining, which is a much better starting point for a side project than a feature request.

## So We Built Narrly

Narrly does that matching bit for you.

You drop in your Guide and your Master, hit the button, and it works out which takes in the Master belong to which lines in your Guide. You get back a multi-track WAV with your Guide on the first channel and the takes stacked above it, each one sat at the right point on the timeline. Import it like any other file, then mute, solo and cut as normal.

That's it. It's not trying to edit your video, and it isn't going to write your script. It does the one boring hour and then gets out of the way.

Under the bonnet there's a web app, a backend, and a chunk of audio processing doing the heavy lifting. I'll leave it there for now, partly because the interesting bits deserve a post of their own, and partly because I'm still busy breaking them.

## Shipping It Properly

Here's the bit that's actually stretched me.

I've got a folder full of repos that stop the moment the interesting problem is solved. This time I wanted to take one all the way out into the world, and it turns out "all the way" involves a lot of things that aren't code.

A domain. A terms page. A privacy policy that I actually had to sit and think about, because people are uploading work that isn't theirs to give away. Deciding what happens to those files (they're processed on our own kit in the EU, they never go near a third-party AI platform, and they're binned when you close the tab). Writing an FAQ in plain English rather than the version I'd write for another engineer.

None of that is glamorous. All of it took longer than I expected. I've got a lot more sympathy now for people who ship products for a living.

There's no sign-up, no login, and we don't ask for your name or your email. It's free while it's in early access, mostly because it's early and I'd rather have feedback than a payment page.

## A Head Start, Not a Finished Edit

I'll be straight about what it is. Narrly won't place every take perfectly, and it isn't meant to make the final call. It shows you what it found before you download anything, so nothing quietly disappears on you, and you should still check the output before you rely on it for something that matters.

It's meant to save you the boring hour. That's the whole pitch.

## Give It a Go

It's live at [narrly.tech](https://narrly.tech). Drop two files in and see what comes back.

If you edit video and it's rubbish for your workflow, I genuinely want to hear about it. You can reach me at [hello@jamesmillner.dev](mailto:hello@jamesmillner.dev).

And Ross, if you're reading this, that's your hour back. You owe me a pint.
