[Back](https://greengolem.github.io/StructuraHowtos)

**Howto socket operations**


The sockets are directly linked to the unit on the 6 directions

Sockets store resources

The storage type: matter, antimatter, energy, combined

The socket mode: storage, buffer, transport, reject, discard

For all sockets operations:

Main > Components > Socket

Main operation is to transfer resources, depending on the storage type and socket mode.

Default socket mode is transport, default storage type is combined

From unit to socket:


Unit > Components > Socket > Transfer

From socket to unit:

Unit > Components > Socket > Storage release


Also there exists mass operation that affect all existing sockets:

Unit > Components > Socket > All Storage release

Unit > Components > Socket > Storage fill
