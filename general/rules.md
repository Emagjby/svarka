# Svarka — Custom 3-Hand Poker Game Documentation

## Overview

**Svarka** is an online multiplayer card game for 2 to 10 players per table.  
The game uses a custom 7-card deck and unique scoring rules, including a wild card and special point calculations.

---

## Game Setup

- **Players per table:** Minimum 2, maximum 10
- **Deck Composition:** Cards 7, 8, 9, 10, J, Q, K, A in four suits (♠, ♥, ♦, ♣)
- **Wild Card:** 7♣ (Seven of Clubs) — special rules apply

---

## Card Values

| Card | Value (Points) |
| ---- | -------------- |
| 7    | 7              |
| 8    | 8              |
| 9    | 9              |
| 10   | 10             |
| J    | 10             |
| Q    | 10             |
| K    | 10             |
| A    | 11             |

---

## Scoring Rules

### Pairing by Symbols

- Cards are paired or grouped by **suit symbol** (♠, ♥, ♦, ♣) to form pairs or triples.
- Scoring sums the card values in the pair or triple.

### Hand Types & Scoring

| Hand Type                | Description                                      | Score Calculation                |
| ------------------------ | ------------------------------------------------ | -------------------------------- |
| **All Different Suits**  | No pairs or triples; highest card value counts   | Highest card value               |
| **Pair of Same Suit**    | Two cards share the same suit                    | Sum of card values               |
| **Three of a Kind Suit** | Three cards share the same suit                  | Sum of card values               |
| **Special Double Aces**  | Two Aces together (any suits)                    | Fixed 22 points (11 + 11)        |
| **Wild Card (7♣)**      | Counts as 11 and connects to highest pair/triple | Adds +11 points to connected set |

---

## Wild Card Rules (7♣)

- The **7♣ is wild** and counts as 11 points.
- It connects to the **highest card or pair/triple** to maximize the hand value.
- Examples:
  - If connecting to a pair of K♥ and Q♥ (both 10 points each = 20), wild adds 11 → total 31 points.
  - If connecting to two Aces (22 points), wild adds 11 → total 33 points.

---

## Special Maximum Scoring Hands

| Combination                       | Score |
| --------------------------------- | ----- |
| Three Aces (any suits)            | 33    |
| Double Aces + 7♣ Wild            | 33    |
| Three Sevens (including 7♣ Wild) | 33    |

---

## Gameplay Flow (High-Level)

1. Players join a table (2-10 players).
2. Deck is shuffled and cards are dealt.
3. Players receive 3 cards each.
4. Players evaluate their hands based on the scoring rules.
5. Player with the highest scoring hand wins the round.
6. In case of tie, resolve by highest individual card value or pre-defined suit hierarchy (♠ > ♥ > ♦ > ♣).
7. Next round starts or players leave/join.

---

## Multiplayer Specifics

- Real-time or turn-based online play.
- Players can create or join tables.
- Chat and player status indicators available.
- Game state synced across all players with server authority.

---

## Additional Notes

- No AI opponents — multiplayer only.
- Emphasis on social interaction and competition.
- Wild card creates exciting strategic possibilities.

---
