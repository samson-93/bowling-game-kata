# bowling-game-kata
This repository is the boilerplate code for getting started with the Bowling Game Kata in dotnet.

I originally wrote this in .NET 8.0, but have ported it over to .NET 9.0 for the time being.

## Kata

### Background

A completed game of bowling consists of 10 frames. In each frame, the player has two opportunities to knock down 10 pins. The score for the frame is the total number of pins knocked down, plus bonuses for strikes and spares.

A _spare_ occurs when the player knocks down all 10 pins in two tries. The bonus for that frame is the number of pins knocked down by the next roll. For example, if you get a spare in the 3rd frame, and in the fourth frame your first roll knocks down 5 pins, your score in the 3rd frame would be 15 (10 + bonus of 5).

A _strike_ occurs when the player knocks down all 10 pins on the first try. The bonus for that frame is the value of the next two balls rolled.
In the tenth frame, a player who rolls a spare or strike is allowed to roll the extra balls to complete the frame. However, no more than three balls can be rolled in the tenth frame.

### Instructions

- Write a class `Game` with two methods
- `void Roll(int pins)` is called each time the player rolls a ball. The argument is the number of pins knocked down.
- `int Score()` is called only at the very end of the game. It returns the total score for that game.

## References

I originally discovered this kata via [ardalis' kata-catalog repository](https://github.com/ardalis/kata-catalog/blob/main/katas/Bowling%20Game.md)

This kata originates from [Uncle Bob's walkthrough](http://butunclebob.com/ArticleS.UncleBob.TheBowlingGameKata)
