[Back](https://binary-station.github.io)
<hr>
<br>
## Constanta

### Intro

My odd entry for the LEGENDARY Leadwerks Retro Summer Game Tournament 2018.

It is a mass multiplayer game, the factions are at war and need your help to capture more teritory.
Faction available: red, white, black, green, yellow.
Choose you faction and provide a unique name to join.

### Details

Game map is formed by a cube of cubes (9 cube side).So 729 selectable territories.
You can navigate the map in first person view.

The game starts at world 0 , 19 worlds are available each with its own territories.
Below you can see how the world is structured and how worlds are indexed:
-9 -8 -7 -6 -5 -4 -3 -2 -1 0 1 2 3 4 5 6 7 8 9
You can navigate this worlds using left right keys.

For example you are in world 0 at beginning, pressing left key moves you to world -1, pressing right move to world 1.

Each player start with 100 energy.

Energy regenerates by 1 point every 5 seconds.Max available energy 100.

Capture territories by left clicking, the cube gets colored with your faction color (cost 10 energy).
Right click neutralize an enemy cube and turn it to default blue (cost 100 energy).

Another way to capture enemy territory:

Red player select a cube in world 0.
To capture that, you need to capture the same territory in adjacent worlds -1 and 1.

Cube 0 (white) Cube 0 (red) Cube 0 (white)

world -1        world 0      world 1

Territory 0 from world 0 is captured by white.


Client has a config.json text configuration.
Add your own server in there to play.

Cmd line option to start your own server on another ip/port: server.exe -ip="some ip" -port=someport
Client remembers any number of local players,
so you can actually use multiple clients but only one at the same time on same computer (because it captures mouse movement).

Input reference:

w - up

s - down

a - strafe left

d - strafe right

e - fly up

q - fly down


left - move left world

right - move right world

esc - menu


mouse look

left click - capture free cube

right click - neutralize enemy cube


### Download

Available for windows.

&nbsp;&nbsp;&nbsp;&nbsp;[Constanta](https://www.leadwerks.com/community/files/file/3643-constanta/)

