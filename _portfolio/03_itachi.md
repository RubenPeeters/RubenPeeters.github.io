---
title: "Itachi"
excerpt: "Multi-purpose python discord bot."
collection: portfolio
---

## Description

Itachi is a multi-purpose python bot, for the popular chatting platform Discord. The project started from a desire to have a personal assistant for using Discord and grew to be a place for me to grow my python skills. The bot had over 100.000 users at the time.

## Notable functionalities

### Chess

As an avid chess lover, I felt a desire, nay, a necessity to include a chess game into the bot. The game rules are, well, the rules of chess. One would start the game by issuing a challenge into a text channel, to which other users could react. The game begins with the first responder, locking the channel for further chess games until the game has ended. This to avoid spam of game messages.

### Global emotes

Discord has a paid version, called Nitro. This version of the software allows users, among other things, to use emotes that are only available in specific servers, to be used globally. As it turns out, it was possible to achieve a similar thing with the API.

A user can type emotes using following syntax: `:name_of_emote:`. This will then get replaced by a small version of the image, that is linked to `name_of_emote`, in combination with the list of servers the user is in. Behind the scenes, Discord gives these emotes a unique identifier, and hosts them at a link that can be reverse engineered. As a bot user is in many different servers, it has access to many of these emotes. By default, it can use all of them in all servers. Using this information, I allowed users to add their favorite emotes to the list of supported emotes for the bot (needed to give an overview of the emotes, and to ensure non-clashing emote names), and use them in a similar way as the original `:name_of_emote:`. Whenever users typed `;name_of_emote;` (note the semi-colon, as opposed to the colon), the bot would then reply with the emote that they referred too.

### Customizability

A command is run by prefixing your message with the bot's custom prefix, e.g. `!chess`. In this example `!` is the prefix, `chess` is the command. As some servers had a multitude of bots in their user list, these prefixes were bound to interfere with each other. To solve this problem, a per-server custom prefix was made available. The prefixes were added to a database, and loaded on set up.

### Music

Using FFMPEG, the bot had the capability to playback music. This was one of the functionalities I played around with the most, and was the most highly sought after addition to a bot at the time.

## Relevant technologies

- Python
- SQL
- FFMPEG

## Relevant links

[source code](https://github.com/RubenPeeters/Itachi)
