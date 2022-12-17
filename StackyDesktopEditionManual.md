[Back](https://binary-station.github.io)
<hr>
<br>
## Stacky Desktop Edition manual<br><br>

----------

**Introduction**

----------

Welcome to Stacky Desktop Edition
<br>
A puzzle game about stacks

There are 2 panels each containing a stack.
You can apply operations on the left stack (working).
On the right is the target stack, cannot be modified
Scope is to recreate the right stack arrangement.

There are several puzzle generators of different difficulty.
So will not run out of puzzles. 

----------

**Manual**

----------

Stack notation explained:
<br>
operation (initial stack -- after operation stack)
<br><br>
Single cell operations:

dup   ( n -- n n )

drop  ( n -- )

swap  ( n1 n2 -- n2 n1 )

over  ( n1 n2 -- n1 n2 n1 )

rot  ( n1 n2 n3 -- n2 n3 n1 )

-rot  ( n1 n2 n3 -- n3 n1 n2 )

nip  ( n1 n2 -- n2 )

tuck  ( n1 n2 -- n2 n1 n2 )

<br>

Double cell operation:

2dup  ( d -- d d )

2drop ( d -- )

2swap ( d1 d2 -- d2 d1 )

2nip ( d1 d2 -- d2 )

2tuck ( d1 d2 -- d2 d1 d2 )

2rot ( n1 n2 n3 n4 n5 n6 -- n3 n4 n5 n6 n1 n2 )

2-rot ( n1 n2 n3 n4 n5 n6 -- n5 n6 n1 n2 n3 n4)    

<br>

n means 1 stack element

d means 2 stack elements next to each other

----------

**Credits**

----------

A game by Binary Station
<br>
Contact:

greengolem.net@gmail.com

