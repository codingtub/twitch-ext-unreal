# twitch-ext-unreal

![](twitch-unreal-game.gif)

## Description

This repo contains a proof-of-concept implementation to receive 2D screen click-events from a WebSocket and transform them to 3D world coordinates to enable movement.

### About the project

It was created as part of an in-game technologies course at my university with the vision to create a game that can be interactively played through a twitch live stream with the means of a custom extension to add further interface capabilities and the ability to directly interact with the game via clicking on the live stream ([the repo for the exension boilerplate](https://github.com/codingtub/twitch-ext-nextjs)). The clicks of the live stream are sent to a custom backend (this repo) and forwarded to the game (([this Unreal Engine 4 project](https://github.com/codingtub/twitch-ext-unreal))). This was done because Twitch extensions don't allow opening WebSckets in the extension directly, which makes a lot of sense regarding security. Those click events were then mapped from 2D Screen coordinates to 3D world space coordinates and used to simply move a player in a top-down setting to move across the screen, pretty great!

Feel free to use this concept for your own ideas and if you ever create an experience similiar to ours please [contact me](mailto:mr@codingtub.eu), I'd be happy to test it!
