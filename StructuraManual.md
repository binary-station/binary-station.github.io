[Back](https://greengolem.github.io)
<hr>
<br>
## Structura manual<br><br>

**Introduction**

----------

Structura is a rather unique sci-fi real time strategy set in space.

Its a hybrid of rts and fps, emphasis on combat and survival

, the economy is important for the war effort.

You are the commander of a combat unit of the Human Resistance Fleet.

Build your economy for war, modify the unit by adding components,

explore, expand and survive the savage waves of enemies attacks.

Scan and destroy enemies, plan your defenses, jump the unit to safety.

<br>


**Story**

----------

The remains of the human race is scattered across the galaxy. 

As the enemy destroyed our worlds mercilessly, humans had to adapt.This war is known as the endless war.
We never seen an enemy or capture one, only intelligence is on their technology, and after all this time we have no answer to why …

The Resistance fleet was created.The unit is the main combat vessel , an ark, storing couple of hundreds human personalities in a cybernetic simulation.
Nobody seen a real human in hundreds of years.

You are commander of the unit 1237. As the endless war rages, your mission is clear you do not forgive or forget.

Survival is taking a heavy toll, especially when units are lost.After a unit is destroyed some human shards can be recovered.And later recomposed into the simulation.But a part of the personality is lost forever.

The destruction continues and the remains of humanity barely survives.
Its just a matter of time…

<br>

**Interface**

----------

<br>

**Resources**

----------

basic resources:

- matter
- antimatter
- energy

composite resources:

- salvage
- tech
- monolith
- shards

Initial resources available at game start:
matter          0
antimatter   0
energy          200
Check resource costs for components.
Its important to have a stable economy.

<br>

**Economy**

----------

<br>

**Unit**

----------

The ship , stores resources and components can be attached.

The sentinel and the kernel are important parts of the unit.
Check:

- components section for descriptions, resource costs.
- sentinel,kernel section

Requirements to construct a new unit:

- attach a platform
- attach an adapter (depending on type of unit you want to construct: )

adapters available: standard, fortress, recon, deathstar

- resource costs

( m: 30 am: 10 e: 10 monolith: 10 salvage: 10 tech: 10 shards: 10 )

For an description on how to attach components to the unit check the “Attach components howto”.

<br>

**Sentinel**

----------

The multi function defender of the sentinel.
Sentinel can carry a limited amount of resources:
m: 0, am: 0, e: 200
Can be used for sentinel operations or as cargo ship.

The sentinel starts as docked to the unit.
All sentinel operations can be done from the main menu: Main > Sentinel
Once in undocked state energy is consumed by the internal systems.
If out of energy operations will not work anymore , like firing lasers.

Sentinel movement will not be restricted as the engines are powered by a remote energy transfer from the unit.
This energy transfer has a limited range , don't pass the limit or the sentinel will be stuck with no way to move.
If you arrive in this situation only way out is to self destruct and reconstruct the sentinel.
Main > Sentinel > Selfdestruct, Reconstruct

Slot layout
Front:
2xlaser mounts
Mid:
1x left slot, 1x right slot
Core:
1 core slot
Back:
1x left slot, 1x right slot

<br>

**Kernel**

----------

Each unit has a kernel at its core.
Inside the kernel is a cybernetic simulation, storing several hundred personalities of humans.
This is how the human race survives the war.
So the unit and other components are just a cocoon for the kernel.

The commander is picked from this uploaded humans.
The unit activities are coordinates from inside the kernel, there are some automated systems that run anyway even if the kernel is stopped.
Also the kernel provides enemy detection, early warning system around the unit , this is known as kernel range.
To increase the range should be a priority.

Only one kernel can exist even if several units are built.
The kernel can be  moved from unit to unit in case of danger.

To access Kernel facilities use the menu:
Main > Kernel

<br>

**Components**

----------

The unit can have components attached on one of the directions:
up, down,left,right,front, back
A component needs to be linked to the unit as described below:
unit → socket → tunnel → component
So a socket and a tunnel attached on the same direction is needed to be able to add the component.

List of all components with resources cost:

<br>
- sockets

Basic component is directly linked to the unit.
Only a tunnel can be attached to it.
Sockets can store resources, some components used the resources from the socket.

Socket operations
Main > Components > Sockets

- Transfer Mode
- Storage Type
- Transfer
- Storage release
- All Storage release
- Storage fill

( cost m: 10 am: 5 e: 5 )

<br>
- tunnel

Can only be attached to a socket.
Any other component can be attached after a tunnel.
The size of the tunnel can be set by using the attach command.

( cost m: 20 am: 0 e: 20)

Common part for the (power plant, mine, accelerator):
This components starts inactive, to bring online resources are needed on socket/tunnel linked to the unit.

Attach a Logistic center, is a requirement to be able to move resources to the sockets.
The component will use resources from the socket/tunnel linked to it.
Move resources to the corresponding socket:
Main > Components > Socket > Storage fill

The components will produce its output and shutdown automatically if no resources left on the socket.

<br>
- power plant

One of the most important components, having a stable economy is key.

Produces energy, attach a power plant to remove the emergency power state on the unit.
(Emergency power state m: -2 am: -2 e: -2)
After the power plant construction the unit is stable (m: 0 am: 0 e: 0).
By default the power plant is inactive, doesn't produce energy.

Once the resources are in place online the power plant:
Main > Components > Powerplant > Online

(cost m: 50 am: 50 e: 10)
(output m: 0 am: 0 e: +9)

<br>
- mine

Mine matter from asteroids.
Attach a mine Main > Unit > Build > Attach component
By default the mine is inactive.

Once the resources are in place online the mine:
Main > Components > Mine > Online

Select the mine (left click) and then right click select the asteroid to mine.
The transporter will bring in matter until the asteroid is depleted and destroyed.

(cost m: 10 am: 0 e: 5)

<br>
- accelerator

Generates antimatter.
Attach the accelerator Main > Unit > Build > Attach component
By default the accelerator is inactive.

Once the resources are in place online the accelerator:
Main > Components > Mine > Online

(cost m: 10 am: 0 e: 5)
(output m: 0 am: +1 e: -1)

<br>
- battery

Can store energy for the unit.Max energy per battery 500.
Matter and am are consumed to store energy into the battery.

Battery operations:
Main > Components > Battery > 

- Battery level - prints battery level to the console
- Recharge - recharge the battery using unit energy
- Energy release - release the energy from battery to unit

(cost m: 10 am: 20 e: 50)

<br>
- recycler

Input matter, antimatter and energy and it creates a monolith.
A monolith uses containment fields to store all resources in a stable form.

Main > Components > Recycler >

- Transfer - transfer resources to produce the monolith
- Online
- Offline

(cost m: 20 am: 20 e: 20)

<br>

**Howtos, help**

----------

Besides the manual, help is available anytime in game (in main menu).

Howtos available in the menu:
Main > System > Howtos
This replaces the tutorial so i advise to read them they show how to do useful operations in the game.

For general information:
Main > System > Help

<br>

**Credits**

----------

A game by GreenGolem Games
<br>
Contact:
greengolem.net@gmail.com
