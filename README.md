# Object-Oriented CLI Blackjack Game

An interactive, terminal-based implementation of the classic Blackjack (21) casino game, engineered in Python using Object-Oriented Programming (OOP) principles and ASCII terminal art.

---

## Overview

This project implements standard Blackjack rules using clean Python OOP class structures. It features dynamic ASCII card visualization, deck creation, automatic Ace adjustment algorithms (handling 1 vs. 11 logic), dealer AI rules (hitting under 17), and game state tracking over multiple consecutive rounds.

---

## Key Architecture & Features

### 1. Object-Oriented Design

* **`Card` Class:** Encapsulates rank, suit, numeric value, and UTF-8 suit symbol rendering ($\spadesuit, \clubsuit, \varheartsuit, \vardiamondsuit$).
* **`Deck` Class:** Generates a standard 52-card deck, handles shuffling via `random.shuffle()`, and manages pop/deal operations dynamically.
* **`Hand` Class:** Tracks player/dealer cards, calculates real-time hand totals, flags natural Blackjacks, and renders customizable ASCII card graphics.
* **`Game` Class:** Manages game loops, input validation, dealer turn rules, and outcome checks.

### 2. Gameplay & Logic Features

* **Dynamic Ace Value Handling:** Automatically evaluates Ace cards as 11, reducing to 1 if the total hand value exceeds 21 to prevent busting.
* **Dealer Hidden Card Mechanism:** Conceals the dealer's hole card until the player stands or completes their turn.
* **Standard Casino Dealer Strategy:** Dealer hits automatically on hand totals under 17 and stands on 17+.
* **ASCII Art UI:** Clean card frames rendered directly in the terminal interface.

---

## Quick Start / Usage

### Prerequisites

* Python 3.6+

### Running the Game

Run the Python script directly in your terminal or Google Colab:

```bash
python Blackjack.py

```

### Sample Interface

```text
========================================
           🎰 BLACKJACK 21 🎰           
========================================
How many games do you want to play?: 1

----------------------------------------
ROUND 1 OF 1
----------------------------------------

👤 YOUR HAND
┌───────┐ ┌───────┐ 
│ K     │ │ A     │ 
│   ♠   │ │   ♥   │ 
└───────┘ └───────┘ 
Total Value: 21

👑 DEALER'S HAND
┌───────┐ ┌───────┐ 
│ ░░░░░ │ │ 8     │ 
│ ░░░░░ │ │   ♦   │ 
└───────┘ └───────┘ 

🔥 BLACKJACK! You win!

```

---

## Repository Structure

```text
├── Blackjack.ipynb    # Complete Google Colab Notebook
└── README.md          # Project documentation

```
