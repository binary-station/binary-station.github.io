[Back](https://binary-station.github.io)
<hr>
<br>
## Tomis manual<br><br>

## Description

    Tomis is a space board game that utilizes a standard chess board and backgammon pieces.

## Game pieces (per player)

    1 base (king)
    4 inactive gates (black backgammon pieces)
    4 active gates (white backgammon pieces)
    4 jump gates
    8 frigates (pawns)
    2 sentries (towers)
    2 towers (bishops)
    1 flagship (queen)
  
## Scope/Story

    In Tomis, two fleet commanders engage in a space battle.
    The objective is to utilize the available structures and ships to defeat the enemy and destroy their base.

## Initial placement

    Base
        The white player starts first by placing the base on their back row.
        Next the black player places their base.
        The base can be placed anywhere on the back row.
    Gates
        The inactive gates are placed first.
        One gate is placed per row, one per turn, starting from the back row.
        Gates must be positioned at least one step away from the base.
        Only one gate can exist per row.
    Frigates, Sentries, Towers, Flagship
        These pieces can be placed anywhere on the back row,
        except directly on a gate.
    Flagship
        The flagship is only available after a frigate arrives on the back row of the enemy.

## Attacks

    Attack point = AP (Attack Point)

    AttackPoints:

    The base has no attack points.
    Frigates, Sentries, Towers, Flagship (1 AP).

    Attack effects:
    
    A stalemate occurs when the attacker and defender have the same APs (no effects).
    An attack is successful if the number of APs is larger than the target's APs.
    After a successful attack, a piece is removed from the board.
    
    Frigate Attacks (1 step):

      \ | /
        #

    Sentry Attacks:

       \ /
        #
       / \

    Tower Attacks:
        |
      - # -
        |
  
    Attack examples:
    
      1 frigate vs. 1 frigate => stalemate (neither can destroy each other).
      2 frigates vs. 1 frigate => successful attack (2 AP vs. 1 AP).

## Actions

    Base
    Gate
        Place a marker to transform an active gate into a jump gate.
    Jump Gate
        The default jump range is 2 (horizontal, vertical, or diagonal movement).
        Rotate the marker to determine the direction of the jump.
        To destroy a jump gate, 2 APs are required during a jump if the target is also a jump gate.
    Frigates
        Move 1 step forward or sideways (no backward movement).
        Can attack the front, left, or right.
        Each frigate has one AP.
        To capture a piece, two APs are required.
        Once on a gate, a frigate can choose to activate or deactivate it (replace the pieces accordingly).
        Gate Jump:
            Jump to the next or previous active gate (only 1 step).
            If the target gate has an enemy frigate, 2 APs are required to capture it by gate jump.
            If the target gate is inactive, no jump will be performed.
        Gate Strike:
            The frigate is on an active gate.
            The frigate can attack the upper/lower active gate in this configuration: x G x.
            Both the attacking frigate and the enemy frigate are destroyed.
        Jump:
            The frigate is next to a jump gate.
            The frigate will move 2 steps in the direction of the marker.
            A jump will not be performed if any of the passing rows have no gate.
            Modifying the direction of the marker takes one turn.
            If the gate has 2 markers the piece will jump 3 steps.
    Sentries
        Move similar to a bishop in chess.
    Towers
        Move similar to a tower in chess.
    Flagship
        Move similar to a queen in chess.

## Win condition

    The game is won when the enemy base is destroyed.
    A base is considered destroyed when it comes under attack by 3 pieces.

<br>

**Credits**

----------

A game by Binary Station
<br>
Contact:

<alexandruafrasinei@gmail.com>
