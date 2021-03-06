# Wipe Empty Playfields

I will first detail the setting we've configured for the server, and below I will outline the reasoning that went into deciding to do it. Please read both sections the first time you're here. The top section will be updated when we learn of more consequences of this change.

We've enabled "Wipe Empty Playfields" on the server. This action runs half an hour before biweekly reset (only on Fridays currently but we'll make it run on Tuesdays as well if possible).

The action will mark playfields that are empty, which means:

* No player-built structure exists on the playfields
* No player has logged out on the playfield

The action goes into effect on playfield restarts, and since we have nightly restart just 30 minutes later that will be taken care of for all playfields.

What happens when we wipe a playfield? This is a bit more unknown, but here are the effects we've encountered so far:

* Ships in space sectors that previously were permanently killed and gone, will respawn. It seems that which types of ships respawn is random, and it might be that the number of ships are random as well. We'll update this when we know more. The bonus is that **ships are now back**.
* Bases on the playfields seems to be fixed, both in position and type.
* Asteroids become "undiscovered", but our experience so far is that they're in the same location as before. Bookmarks should thus be valid. Please let us know if you can verify this, or verify that it is *not* the same location.
* Deposits likewise, they are in the same place, but they become "undiscovered". See section below on mitigation.-
* Registry for each player and faction will show stuff that was there before each wipe, and the first time you warp into the sector or playfield the registry for that playfield will become empty, and you will have to rediscover all stuff. Again, see section below on how to mitigate this.

Note that all of the above will *only* happen if no player-created structure exists on the playfield, and no player is logged out. If you've built something there, or parked a ship there, or you just logged out, everything stays the same.

# Why did we do this?

There was a growing discontent on the server between the players because of a problem with the Project Eden scenario. According to the scenario author, there is some new AI settings that needs to be applied to ships, and this has not been done. Without this setting, once a sector ship is killed, it will stay killed.

The author has also stated that he is not sure when, or even if, he will get to adding this AI setting.

Since sector ships are a good source of loot, players felt like they would have to start behaving like locusts, gradually moving through space and killing everything in their path. Additionally, for new players it would mean the start system and surrounding systems would quickly dry up of interesting stuff to do since players had already killed it.

We researched and learned that this "Wipe empty playfields" action would fix this by regenerating the playfields. What was unanticipated was that everything became undiscovered in the sector, and that apparently there is some randomization going on. The expectation we had was that the sector has been randomly created from some kind of random number seed, as the whole game is done like this, and this seed would stay put. Thus, the same stuff that had spawned there the first time, would be regenerated.

Alas, this did not exactly happen. It seems playfields are re-randomized to some extent which means that it seems that asteroid and deposit placements, ships and patrol ships, bases, and other stuff, are completely randomized. Simple tests so far has shown that some asteroids respawn exactly where they were before, but we need more data before we can conclude.

**This was unanticipated and we apologize for this but there is no easy way to go back.**

# What about the registry?

On first read of this page you might think the registry will start to fill up with junk, but it doesn't seem to be the case.

The registry will currently show everything you've discovered *before last nights wipe*. This means both locations (you can bookmark stuff in the registry), types of stuff there, and the number of things, are all from before the wipe. Since it seems the data is not completely wrong, you can use this to guide your re-exploration of playfields and decide which ones to go back to.

Upon first entry to the playfield after the wipe, registry for that playfield will become blank. You will have to rediscover everything. This is an unfortunate effect but we can't pick and choose which effects we want here, it's an all or nothing approach and currently the ship problem weigh more heavily on players. Additionally, see the next section on how to mitigate it and we expect this shouldn't be so bad going forward.

**Here's a tip**

If you want to go back to a planet to get some deposits, or to a sector to get some asteroids, you can bookmark the deposits or asteroids directly from your registry. These bookmarks seems to survive the wipe of the registry that happens when you enter the playfield and you can then move to them. You will then rediscover the undiscovered stuff at those locations, which should be the exact same thing as was there before.

# How do I mitigate this randomization

If you find "the golden playfield", with 45 Zascosium asteroids or some other important constellation of stuff, a way to mitigate this "becoming undiscovered" is to add a small structure to the playfield. You can also, as suggested above for the registry, bookmark the asteroids or deposits or whatever from the registry *before* you enter it. That way you still know what is there, and where it is.

As an example of structures, F12 will create small space satellites that will be placed in space sectors, and a small "land claim base" that we'll place on planets. The fact that there is a player-created structure on the playfield means it will not be wiped. This way we can mark those sectors we don't want to keep rediscovering.

More importantly, it also means that if you finally kill that Tovera-Class Dreadnought that zooms around your sector, and you add your own structure to it, that ship will never bother you again.

# What if?

If you have any questions, or comments, please don't hesitate to let us know. Since some of the consequences were unanticipated it is bound to ruffle some feathers. We understand that registry has become slightly less useful, and we don't like it either but it seems the choices we have are rather limited.
