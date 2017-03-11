# Genergy
Genergy is a [roguelike](https://en.wikipedia.org/wiki/Roguelike) developed in under 7 days for the [7DRL challenge](http://7drl.roguetemple.com/jsp/viewGames.jsp#). It was my first entry into 7DRL, and my first "complete" roguelike.

There were much grander plans for Genergy than those which ended up in the game for the 7DRL release - the ideas behind the game are, in my opinion, quite strong.

If you're curious about the development process, check out my [devlog](https://sgtcodfish.com/7drl). This also pretty accurately describes how much time I had - I had to work and I did some pre-planned stuff which limited how much time I could realistically spend on the game.

## Gameplay
The game is incredibly simple as it stands; you run around the room and kill monsters, which are 3 different levels of deadly:

- `g` - Gremlins - small, common, and easy to kill. Will attack quickly and can see you from a long distance away. Don't get overwhelmed!
- `W` - Witches - middle of the road in terms of damage, but easier to sneak up on than gremlins. Approach with care!
- `O` - Ogres - thoroughly nasty and hard to kill. Long range magic highly recommended - go too close and you'll regret it very quickly.

The movement controls are shown as part of the UI at the bottom of the screen.

To throw thermal energy bolts, press `z` and then a direction key. Watch your capacitor (at the bottom of the screen) - if you don't have enough energy, you can't use energy bolts!

To quit, press `q`.

## The Idea
The goal of Genergy was written on the 7DRL submission page:

> The intention is to experiment with semi-realistic energy transfer as an implementation of magic and see what gameplay emerges from that. This will be my first 7DRL, and hopefully my first "finished" roguelike!

I had wanted to get a lot more types of energy usage into the game - think using kinetic energy to push things away, or stealing potential energy to bring things crashing down to earth. This was to be powered by collectible "fuels" such as coal, uranium and biofuels, which would power your capacitor. Armour and weaponry would tie into the idea of energy as a mechanic. If I keep working on the game - which is a distinct possibility, and is also the reason I've not opened the source yet - I intend to explore this idea in a lot more depth.

As an example of a feature that I didn't have time to implement: using a kinetic blast to get ogres away from you, so you can avoid their incredibly damaging hits. Some more details of my thinking about the game are in the [devlog](https://sgtcodfish.com/7drl).

## Platform Specific Details
### macOS
Genergy is tested on macOS El Capitan and seems to run during gameplay. Ncurses is required to run the game; if you don't have it, you might be able to find it through homebrew, but my impression is that the executable should just run.

Many of the stability issues seen in Ubuntu don't seem as severe on macOS, so if you get the chance, this might be the platform to go for.

### Ubuntu
#### 16.04+
Genergy has been tested to work on Ubuntu 16.04 and Ubuntu 16.10 and runs fine and dandy. You'll need curses installed, but that should be it.

That means if the game doesn't run, you probably need to do:

```sudo apt-get install libncurses5```

or something similar, to get ncurses on your system.

You might run into random segfaults while running the game; this is unfortunately a side effect of being rushed to complete it. :(

#### 14.04
Unfortunately, the game basically doesn't run on Ubuntu 14.04, as the game uses many C++14 features.

### Windows 10
Hopefully coming soon!

### Problems + Troubleshooting
Raise an issue on this repo if you need help and I'll do my best!

## Hashes
These hashes were created before the midnight deadline I set myself on 2017-03-11.
```
sha256sum 7drl/macOS/genergy 7drl/ubuntu16.10/genergy
87aa60a595e780efe08f47f34934b6600b0dd495ebbf88d950d26d68b9b957d9  7drl/macOS/genergy
2cc5d2ab1eb4c941f52e9b3f54d7f61a9669de15f5d6acb53e066816e746b980  7drl/ubuntu16.10/genergy
```
