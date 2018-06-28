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
