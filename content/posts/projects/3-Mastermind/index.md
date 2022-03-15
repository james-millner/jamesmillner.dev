---
layout: page
permalink: "blackjack-cli"
title: "LeedsCodeDojo - Coding Kata - Mastermind :red_circle: :white_circle: :blue_circle: :black_circle:"
date: 2019-05-07
showAuthor: true
showDate: true
showReadingTime: true
---

Wasn't sure whether to bundle this in as a project, but thought why not! It's another piece of Kotlin code, just for a bit of fun.

It was the first [LeedsCodeDojo](https://leedscodedojo.github.io/) in quite a long time, hosted at Sky Betting & Gaming.

The goals of the evening were simple:

    Have fun
    Pair Program
    Learn something new!
    Create some logic that simulated the game Mastermind


As a result my entry is [available here](https://github.com/james-millner/micronaut-mastermind-cli). I opted to attempt 
it in Kotlin using Micronauts CLI functionality. This was good fun, but to be honest I wasn't very familiar with Mastermind the game.

Writing this blog post actually reminded me to update part of the Makefile again! 

### Requirements to run!
Clone the repo and follow:

* Easiest route:
  * Linux / Macos with a valid version of Java installed >= 9
  * run `make` to build
  * run `make run` to play!
* Windows / Not WSL - and without going down the NMakeFile route
  * Ensure you have Java installed 
  * run `./gradlew clean build`
  * run `java -jar build/libs/micronaut-mastermind-0.1.jar`

