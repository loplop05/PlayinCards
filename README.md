Blackjack Game (Python)

A simple Blackjack card game implemented in Python using Object-Oriented Programming (OOP) concepts.

The goal of the game is to get as close to 21 as possible without going over. The player competes against the dealer following the classic Blackjack rules.

Features

Standard 52-card deck

Card, Deck, Hand, and Chips classes

Random deck shuffling

Hit or Stand gameplay

Ace value adjustment (1 or 11)

Player betting system with chips

Dealer automatically plays until reaching 17

Replay option after each round

Technologies Used

Python

Object-Oriented Programming (OOP)

Random module

Project Structure

The game is built using several classes:

Card

Represents a single playing card.

Attributes:

suit

rank

Deck

Represents a full deck of cards.

Methods:

shuffle() → randomizes the deck

deal() → deals a card from the deck

Hand

Represents the cards held by a player or dealer.

Attributes:

cards

value

aces

Methods:

add_card()

adjust_for_ace()

Chips

Represents the player's betting chips.

Attributes:

total

bet

Methods:

win_bet()

lose_bet()

Game Rules

Each player receives two cards.

One of the dealer’s cards remains hidden.

The player can choose:

Hit → take another card

Stand → keep current cards

If the player's total exceeds 21, the player busts.

The dealer must hit until reaching 17 or higher.

The highest value ≤ 21 wins.

Ace values:

11 by default

Automatically converts to 1 if needed to prevent busting.
