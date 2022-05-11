---
title: iRacing Reports Discord Bot - Version 3
---

# Version 3 in Beta Testing

Over the past months I've been working away on a total re-write of the iRacing Reports Discord Bot, I'm declaring that this is version 3! They key change is that users now interact with the bot using slash commands, rather than the current `!<command>` style commands. 

I currently have the new version 3 bot up and running in a #beta-bot-playground channel on the [iRacing Reports Discord server](https://discordbot.iracingreports.com/discord). Please give it a shot and find any bugs before I roll it out to all the subscribers' servers.

Along with the switch to slash commands I've also taken the time to make huge refactors of many of the related backend systems. From the database schema, to the website, the way the bot announces race results, to how we integrate Patreon. 

These efforts were kicked off in response to a change that Discord announced some time ago, and will be enforcing come the end of August; verified bots will no longer be able to listen for commands in chat channels. Because of this change, the iRacing Reports bot had to be switched over to use the new slash commands system. For info about this change from Discord's side of things: <https://support-dev.discord.com/hc/en-us/articles/4404772028055>

While on the surface of things the version 3 bot may seem like it is merely at feature parity with the currently running production bot (ie: version 2), the list of improvements under the hood is quite lengthy. I've put in a lot of effort to make the most popular commands as efficient as possible. For example, the `/driver` command is now muuuuuch faster than the old `!driver` command... and it even includes more information than before!

Crucially, many of the "behind the scenes" changes have been implemented in order to open the door on some new ideas that I've had, and common feature requests that have been made by users, over the 2+ years that the bot has been alive. Many of these "wouldn't it be cool to have" ideas were previously impossible without huge changes to some of the core assumptions I made when I originally started the project. Well, those huge changes have been made. Expect more features to be rolled out once the switch over to the new version 3 bot is completed.
