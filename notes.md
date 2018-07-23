# h&dsa 2018 ws proposal — dat

## intro

[Summer Academy 2018: A Open call for participation](https://hackersanddesigners.nl/s/Events/p/Summer_Academy_2018%3A_Open_call_for_participation)

> - Proposed workshop formats are: 1/2 day, 1-day, or 2-days. Shorter intermission are also possible for newbies.
> - Hands-on means of production should stay central during the workshop.
> - The proposal should cover aspects of design, artistic research, and programming. If you need support on one of the aspects, consider finding a collaborator via the H&D network.
> - Giving a workshop can be quite intensive. We therefore advise to collaborate with 1 or 2 people on submitting proposals.

## idea

turn raspberry pies into dat pies. moving from the internet to the web. play more fluidly between online and offline. expand how you can share data.

inspired by [this repo](https://github.com/new-computers/dat-pi) (dat-pi), and the [early discussion](https://github.com/new-computers/dat-pi/issues/3) they went through.

- [here a guide](https://guides.newcomputers.group/installing-dat-raspberry-pi.html) on how to do it by hand
- [here](https://github.com/new-computers/seeder) a functioning prototype of the plug and play version
- [homebase](https://github.com/beakerbrowser/homebase) does the server setting up for dat
- use [enoki](https://enoki.site) to setup p2p websites and share stuff
- [Rotonde](https://louis.center/p2p-social-networking/) for an ad-hoc social network?
- setup a lan between pies?

## collateral

~~propose to use scuttlebutt with ad-hoc groups (and a common pub?) to chat throughout the summer academy, as last year slack was used for.~~ 

## material

- 3-5 raspberry pies w/ wireless and microSD modules

## notes 28062018

### pre ws

- test router!
- install raspian, test wifi, node.js 

### during ws

- install dat (on pies and on people's laptop) and hypercored on pies
- install beaker browser
- make websites w/ panel.enoki.site through beaker browser
- add website dat url to index.dat
- use some version of [pask](https://github.com/nonlinear-thinkering-group/pask) to run the MUD exercise!

### todo

- make index dat-based website where people can add new dat urls
- come up w/ MUD based game exercise, look up previous workshop in the week to make theme / output connections 

### ref

- [MUD](https://en.m.wikipedia.org/wiki/MUD)
- [hyperdungeon](https://github.com/cblgh/hyperdungeon)
- [dwarf fortress](https://en.m.wikipedia.org/wiki/Dwarf_Fortress)

## setup raspberry pi

refs:

- [burn raspian.img onto sd card](https://www.raspberrypi.org/documentation/installation/installing-images/mac.md)
- [setting WiFi up via the command line](https://www.raspberrypi.org/documentation/configuration/wireless/wireless-cli.md)
- [connect to wifi and setup dat](https://github.com/new-computers/guides/blob/master/guides/installing-dat-raspberry-pi.md)
- [setup persistent dat on raspberry pi](https://docs.datproject.org/server)
  - w/ [pm2 and startup hook](https://pm2.io/doc/en/runtime/guide/startup-hook/)
  
- [Seeder from ncwg](https://newcomputers.group/seeder.html)
## MUD gameplay

### sketch

- here's an idea: 
  - each room in the MUD is a dat
  - each player designs a room, and gets some information or an artifact to hide, like maybe a key.
  - each player also gets a goal, or something to find in the other players rooms, and perhaps a character or role
  - players in the same room can chat, and perhaps swap items
  - you get a kind of distributed emergent gameplay, where the "state" of the game is distributed between the dats

### notes 02072018

- each laptop is a dungeon
- dungeons can ally between each other and or face / confront each other in order to get each others' key (dat adddress) and or items
- each dungeon design their own room: a description with what's going on in there, what happens when you enter it, etc)
- each dungeon has to make their own content (room description, characters (? or is this random), items the dungeon owns
- dat pies: DAOs, genesis masters, chatbots, and possibly taverns?
- magic rules happen every now and then: eg. everyone passes to the person next to them their laptop (dungeon) and they have to perform some action over the dungeon (delete a file, rename a file, add a file) or take over and being in charge of that dungeon
- these *magic rules* are coordinated by the dat-pies acting as DAOs, and executing rules written in their smart contracts
- dependancy graph: everytime a peer get a new key of another dungeon, they have to add the key to their dat and because of that, then they will be able to visit that dat and see which items the dungeon has
- the above action is enable by the use of a map, displaying the other dats / dungeon you have visited
- internet affect points: hate speech, social justice warriors, trolls, fake news, headline-clickbaiters
- peers trade items etc in the DAOs, in this way alliances can be formed or disregard and peers can combine the items they start the game with with other items and being able to perform specific actions (eg combining two objects to execute a specific action and get the desired output)

# notes 20180718

- pies act as:
  - shops
  - DAOS (weather, NPCs, etc)

### short description of your workshop

*hypermush* is an introduction to p2p technologies, their functioning and user-application, disguised as a [multi-user-shared-hallucination](https://en.m.wikipedia.org/wiki/MUSH) (MUSH) videogame.

MUSH are an evolution of [MUD](https://en.m.wikipedia.org/wiki/MUD), multi-user-dungeon: early multiplayer text-based adventure videogames from the '70s.

We're gonna use the MUSH game dynamics to explore the p2p [dat protocol](https://datproject.org/), and  build shared interconnected narratives by way of dungeon explorations, user group formation, file tradings, key discovery... until it gets hyperreal.

![mud](http://www.mobygames.com/images/shots/l/78247-questron-apple-ii-screenshot-this-dungeon-is-multi-leveled.png)

### schedule and practical information

- `10:00` Introduction
	- 
- `10:30` Installing beaker
- `10:45` Explaining beaker
	- Visiting sites
	- Seeding a site
	- Forking
	- Editor
	- Versions
	- Hashbase
- `11:30` BREAKER
- `11:45` Playing some more
	- Installing Dat commandline
	- Installing Dat on raspberry pies
	- Homebase
- `13:00` LUNCHOKI
- `14:00`
	- [dat shopping list](https://github.com/jimpick/dat-shopping-list)
	- [hypercast](https://github.com/louiscenter/hypercast)
	- [hyperchat](https://github.com/frnsys/hyperchat)
	- [hyperdocs](https://github.com/frnsys/hyperdocs)
	- [Rotonde](https://github.com/Rotonde/rotonde-client)
- `15:00` [Enoki](dat://panel.enoki.site/)
- `16:00` hypermush
	- character design
	- dungeon design 
	- play
- `17:00` BEERKER

People needs to bring their laptop. moreover, it is suggested to make use of the outcomes of the previous days (files, ideas, etc) to inform the design of the dungeon and the general gameplay of the MUSH.
