[Back](https://binary-station.github.io)
<hr>
<br>
## Nerva manual<br><br>

## Description

Nerva is a board game that utilizes three chess boards and backgammon pieces.

## Game pieces (per player)

Three chess boards and backgammon pieces.

Total 192 backgammon pieces

96 white 

96 black

1 white king

1 black king

## Scope/Story

In Nerva, two powers collide across the battlefield. Players must expand their influence by 

capturing neutral territory, strengthening their positions through geometric connections, and 

hunting for the enemy’s hidden King.

## Initial placement

Align the three boards horizontally (Left, Middle, Right).

No pieces are placed initially. The empty places are considered neutral.

A player can capture a neutral teritory by placing a piece.

When the game begin each player decide a place for their king,

note it on a paper and keep it for yourself.

The kings are hidden until a player try to capture their location on the board.

In this case the player that knows the position will place the king on the board.

## Attacks

Every piece strength is determined by its relationship to other pieces of the same color.

| Connection Type | Bonus | Applied To |
| :--- | :--- | :--- |
| Orthogonal (Sides/Front/Back) | +1 | Defense |
| Diagonal (Corner-to-corner) | +1 | Attack |
| Stacked (2 Boards) | +2 | Attack & Defense |
| Stacked (3 Boards) | +3 | Attack & Defense |

## Actions

On your turn, you perform one primary action: The Capture.

* Place a piece on neutral territory on any of the three boards.

* By attacking a enemy piece calculate your Attack Power against that piece Defense Rating.

* If your Attack exceeds the Defense, you can replace the enemy piece with your own, capturing it.

## Win condition

Reveal and then kill the enemy king.

## Notation

How to record games, use the following:

[BOARD IDENTIFIER]_[POSITION]

board identifier:

* B1 - for the right board
* B2 - for the middle board
* B3 - for the left board

position:

use the algebraic notation in chess

examples:

1. B1_A3 2. B2_F5 3. B1 B5 etc

<br>

**Credits**

----------

A game by Binary Station Studio
<br>
Contact:

<binary.station.studio@gmail.com>
