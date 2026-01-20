# Discount_Eden_Standalone
Repository for the Discount Eden Project, a voxel based terraforming game that gives players the means and motivation to build big.

## Description
Embark on a terraforming adventure with a trio of cybernetic animal friends, turning a fiery hellscape into your own personal Eden one step at a time. Assuming nothing goes wrong, of course…

This voxel game will focus heavily on giving you the means and motivations to build bigger than any other game of its kind. Traditional challenges will largely be self imposed, with a greater focus on efficiency and environmental balancing than combat and boss fights. Create first, fight monsters later.

## Core Gameplay Loop
In the early game, the player will largely focus on making their small habitat self-sustaining, ensuring their long term survival. You’ll learn how to use scaled down versions of some of the major machinery you’ll have to construct later on, and start getting used to the inventory mechanics and decorative features available in the game as a whole

The mid game will be an age of vast infrastructure. This is where the blueprint system will take off, allowing players to fill their world with massive mining machines, sprawling production arrays, and the makings of a few impressive rocket silos. In between increasing the inward flow of resources, players can start to experiment with biological synthesis in contained environments.

As your machines start to make the global environment that little bit more friendly, players can start supplementing the mechanical infrastructure with biology, seeding in more and more life as it’s successfully catered to produce what the player desires.

The endgame will heavily focus on larger plants like trees and a variety of potential animals. Your machines will gradually become obsolete as self-sustaining ecosystems replace the functionalities they once filled.

The entire game is about letting players nudge the world in the directions they want it to go, balancing speed, risk, reward, and potential challenges that may never go away once introduced.

## Prototype
To start with, I plan on making a simple prototype showing off the blueprinting system I'd like to create for the game. The idea here is basically to essentially create a voxel based 3d modeling software that plays like a simple game. It'll come with a fairly narrow selection of blocks, with the assumption that creatives will use custom texture UV's to personalize their projects. Ideally, a UV editor would be built into this demo, as well as an easy way to set up block pallets.

As far as the actual building features, I want easy to use line tools with customizable thickness and block distribution. I want sculpting tools, copy/paste, and painting. All of it should be tailored to being as readable and user friendly as possible, and I want that philosophy to carry over into the actual game when the time comes. Building is not an afterthought in Discount Eden, and ideally it will be much easier than it currently is in any other voxel based game.

The prototype will have no progression, no factory systems, and no proper gameplay elements of any kind. It’s like a more barebones, but highly versatile version of Minecraft superflat on creative mode.

## Actual Gameplay Foundations
The "3d modeling" system outlined in the prototype will serve as the basis of the blueprinting and bot construction system in Discount Eden itself. This system, along with pallet cleanser storage, will sit at the foundation of the game. It will provide what I personally have wished to find in pretty much every voxel game I've ever played. A means to build big without sacrificing the need to gather materials or ignoring the functionality of the structure. This game is about planetary terraforming, and you need to build on a planetary terraforming scale.

Pallet cleanser storage is the gameplay version of the sort of pallet based system mentioned regarding the prototype. Storage entities in Discount Eden generally will not contain as much as storage entities in other games, but that's made up for by the fact that the player and construction bots both have universal access to everything contained in the global storage network. Your inventory will be like an advanced creative mode selection tool that makes it as easy as possible to find what you're looking for. I want basic filters to serve as toggles, not tabs. I want to give players the ability to sort blocks by color, filter by type, and toggle ghost views of materials not currently in the system. Where tabs WILL come into play is with the pallets. The base game will come with a few, and players will be able to easily create their own, making it easier than it has ever been to pick a build style and stick to it, never getting overwhelmed by the sheer quantity of available blocks or over-relying on the search bar to navigate to what you're actually looking for.

Getting throttled by stack sizes and inadequate inventory space will be done away with. Even basic block by block building will be much easier thanks to the storage system alone. The blueprinting system takes this to the next level, allowing a mix of block by block additions and versatile large scale edits. It won't be available right from the start of the game, as it won't be necessary for the scale involved, but it will come a lot more quickly than you might expect from a factory style game. Early game production will be limited to help new players get their feet under them, but it shouldn't be ugly. I will not be locking aesthetics behind progression any more than absolutely necessary.

As for the general art style, I'm leaning towards blocks around a third the size of the player. I think the building system makes it easier to get away with that from a player perspective, so long as it can be managed performance wise. It should help just adding that extra little bit of potential detail, as well as helping to visually distinguish the game from what's come before. I do want to take inspiration from the simple versatility of Minecraft when it comes to actual textures. This may be a sci-fi game, but that shouldn't stop players from building medieval castles if they want to. Heck, I'd love to throw in a few as generated structures built by certain kinds of intelligent life players seed into their worlds.

As far as the computational side of things, nothing that renders in any given chunk should ever be functional. An aspect of the blueprinting system will include the ability to compress the calculations of full production lines into globally calculated increases and decreases. Everything will still look like it works up close, but it's all an illusion. The same philosophy will apply to plants and animals. The environment is determined by global calculations, not local animal behaviour.

## Details and other planned features
### Trains:

Trains will be everywhere. Every major storage structure you build will need to be physically connected to other parts of your factory. From a story/gameplay perspective, the global storage system is power hungry, and it wouldn't be efficient to have every single one of your factories tap into it when you can just physically send resources. That said, the trains themselves are purely decorative. If your storage systems are connected via a point to point monorail line, everything will just work without materials needing to be physically transferred. Computationally, everything actually DOES connect to the global storage system. Connecting rail lines is functionally a bit like connecting power lines. It's just a requirement for your machines to turn on.

That may sound like a drawback, but it has some pretty major benefits. Your factories will be constantly filled with realistically long trains. They'll be able to run on splines, adding curves and movement to your builds that break away from the definitive voxel grid. General design philosophy will be that anything stationary will follow the voxel grid, and anything that moves will have more freedom. The length of your trains will reflect the general scale of your operations, but they won't kill your computer with computational complexity.

### Life:

I want to add as wide a variety of potential life as I can manage, with mod support for custom life forms. Creature synthesis won't be a Spore style abomination machine so much as a set of pre-determined species with configurable traits. Balancing your ecosystem will have a lot to do with managing lifespans, resource requirements, and waste outputs. Creatures will spawn in your world, but their spawn conditions will be dependent on more globally calculated parameters. Some forms of life are more dangerous than others, which leads me to my next feature.

### Space:

Most early plant life will be easy to contain and experiment on within planet side biodomes. The further you progress into the game, however, the more likely it is that something will break out and start a chain reaction that permanently damages your ecosystem. There's a certain time frame in which you can kill, uproot, or recapture everything that escapes, but left to its own devices for too long, any life that gets out WILL become part of the global ecosystem, growing or shrinking at a rate dependent on the current global environment. The easier the planet is to live on, the harder it is to contain dangerous life.

That's where your space station comes in. The station itself is basically just going to be a series of exo biodomes you can construct to safely experiment with more dangerous life without risking your ecosystem. Getting to space is the part I personally find the most interesting. Just like how I want to make use of relatively realistically scaled storage, I also want to make use of realistically scaled rockets, complete with interesting construction mechanics. Rockets will be built out of blocks and block like components, just like any other kind of machine. However, they will be easier to build with specialized silos than construction bots. For performance reasons, you can only have so many bots, and you don't want them constantly working on rockets that perpetually need to be replaced. In addition to getting you to your space station, they'll also be useful for launching AI colonies and spreading life to distant parts of the planet the player will never have time to reach.

### Tutorials:

I want a diegetic tutorial system focusing on that trio of clever animal friends I mentioned above. 

Along for the ride, you’ll have a relentlessly excitable fox to show you the ropes, jumping with joy and enthusiasm as he explains the basic gameplay. 

The cat, by contrast, is a condescending jerk who will berate you for every mistake, and who might occasionally go so far as trying to assassinate you. Unsuccessfully, of course. She’s not very good at being evil. The fox thinks they’re best friends, in spite of the cat’s best efforts.

The axolotl is kind of like this weird prophet character who occasionally goes on about things like “pressing space to jump,” or warns the player of some terrible evil that might come when the chunks start to crunch. Every time she speaks, The fox and the cat both pause what they’re doing and just stare at her like she’s insane.

Ideally, the dynamic between these three will be fun enough to witness that players won’t even notice that they’re learning stuff.

## Endnote
There's quite a bit more I've brainstormed about regarding this project, and nothing is set in stone. I'm open to ideas and desperate for all the help I can get. I'm doing my best to learn all I can, and get to a point where I can really start working on this as fast as possible, but college life is moving a bit more slowly than I'd like, and there's a lot of annoying gaps I have yet to fill.
