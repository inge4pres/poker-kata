# Poker Kata
A Software Engineering kata to test your programming and design skills, based on the No Limit Texas Hold'Em poker card game.

## Goal
The goal of the kata is to create a card game with the rules of [No Limit Texas Hold'Em](https://en.wikipedia.org/wiki/Texas_hold_'em#Rules).

The kata is divided into 3 parts:

1. start phase: implement a card deck and distribute cards to players
2. play phase: flop, turn, river
3. showdown phase: decide who wins the pot

each of which _can_ be solved separately, although it's not mandatory.

To complete the kata the program should run a single hand, assigning 2 cards to 6 players, running the deal of flop, turn and river, and declaring a winner based on the best hand.

### Constraints

* The card deck contains in total 52 cards: 13 (A-2-3-...-J-Q-K) cards for each type (Hearts, Diamonds, Spades, and Clubs).
* Deterministic hands: the deck is shuffled only at the start of every hand, not in the play phase; replaying a hand from the same deck should produce the same result.
* The cards distributed to players should be randomized, and the deck cards should also be dealed at random, but it does not matter if the randomization is cryptographically secure.
* To mimick the game, the dealer _must_ throw away 1 card before each of the deal phases: flop, turn, river, so that at the end of a hand, exactly 20 cards are played, and 33 remained in the deck.


## Non-goals
* Handling bets from players

## Why is it good?
All 3 phases have details and axis of complexities that can be astracted away with multiple techniques: it also tests how fast an implementation can be refactored when new constraints come into play.

## Contribute!
This kata is open for improvements, if you have ideas on how to make it more spicy, raise an issue!
