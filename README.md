# Blackjack Game (Python)

A simple **Blackjack card game** implemented in Python using **Object-Oriented Programming (OOP)** concepts.

The goal of the game is to get as close to **21** as possible without going over. The player competes against the dealer following the classic Blackjack rules.

---

## Features

- Standard **52-card deck**
- **Card, Deck, Hand, and Chips classes**
- Random **deck shuffling**
- **Hit or Stand** gameplay
- **Ace value adjustment** (1 or 11)
- Player betting system with chips
- Dealer automatically plays until reaching **17**
- Replay option after each round

---

## Technologies Used

- Python
- Object-Oriented Programming (OOP)
- `random` module

---

## Project Structure

The game is built using several classes:

### Card
Represents a single playing card.

Attributes:
- `suit`
- `rank`

---

### Deck
Represents a full deck of cards.

Methods:
- `shuffle()` → randomizes the deck
- `deal()` → deals a card from the deck

---

### Hand
Represents the cards held by a player or dealer.

Attributes:
- `cards`
- `value`
- `aces`

Methods:
- `add_card()`
- `adjust_for_ace()`

---

### Chips
Represents the player's betting chips.

Attributes:
- `total`
- `bet`

Methods:
- `win_bet()`
- `lose_bet()`

---

## Game Rules

1. Each player receives **two cards**.
2. One of the dealer’s cards remains **hidden**.
3. The player can choose:
   - **Hit** → take another card
   - **Stand** → keep current cards
4. If the player's total exceeds **21**, the player **busts**.
5. The dealer must hit until reaching **17 or higher**.
6. The highest value **≤ 21** wins.

### Ace Values
- **11 by default**
- Automatically converts to **1 if needed** to prevent busting.

---

## How to Run

### 1. Clone the repository

```bash
git clone https://github.com/yourusername/blackjack-python.git
