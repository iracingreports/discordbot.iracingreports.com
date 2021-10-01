---
title: iRacing Reports Discord Bot - Commands
---

## Commands

In the examples below, square brackets have been used to show the required arguments for each command. Round brackets have been used to show optional arguments that can be provided to provide more fine grained responses.

For some commands you can specify a particular week or season. To select a week you include a **w#** argument, where the # is replaced by the week you want; for example **w1** for week 1 of the season. To select a season you include a **##s#** argument, where the first two numbers are the year and the final number is the season; for example **20s3** for 2020 Season 3. If a season or week isn't specified, the bot will return information about the current week and/or season.

For some commands where it makes sense, if you specify a multiclass series you will need to provide an argument to also specify which class you're interested in.

Many commands have a shorter alias that can be used.

A [complete user guide](https://docs.google.com/document/d/10zXNU6L5Ljrlip4G_evH5ii4_z7gphy1MPv5jeBr4is/edit), with screenshot examples of each command is available.

### Standard Commands:
### `!series [category] (##s#)`
> Displays a table of series and the abbreviations to use for each of them in all the other commands. The category must be provided; either **road**, **oval**, **dirt**, **rx**, or **offroad**.

### `!cars [series] (class abbrev) (##s#)`
> Displays a list of cars in a class and the abbreviations to use for each of them in the other commands.

### `!balance [series] (class abbrev) (rlap|qlap|arlap) (w#) (##s#)`
> Displays information about the balance of performance for a class for a certain week of a series. Defaults to showing average race laps.
> Alias: `!bop`

### `!schedule [series abbrev] (##s#)`
> Track schedule for a series. 
> Alias: `!sched`

### `!driver [driver name] (category) (w#) (##s#) (series abbrev)`
> Returns statistics about a driver's current season. If no category is provided the bot will return the output for the category that the driver has raced the most this season. You can also filter the information returned to a single series by providing a series abbreviation.
> Alias: `!dvr`

### `!lastrace (category) (series abbrev) (r#)`
> Returns information about a driver's most recent race. If `r3` is supplied, the race 3 races ago will be displayed.

### `!lastraces (category) (series abbrev)`
> Returns a list of a driver's most recent 10 races.

### `!championship [series abbrev] (##s#)`
> Output a table displaying the top 30 drivers in the championship standings. 
> Alias: `!champ`

### `!strengthoffield [series abbrev] (w#) (##s#)`
> Outputs a heatmap showing the strength of field of each time slot. 
> Alias: `!sof`

### `!officialsessions [series abbrev] (w#) (##s#)`
> Outputs a heatmap showing the number of times each time slot had official sessions. 
> Alias: `!offs`

### `!participation [series abbrev] (w#) (##s#)`
> Outputs a heatmap showing the participation for the series. 
> Alias: `!part`

### `!qualifyinglaps [series abbrev] (w#) (##s#)`
> Returns a table and scatter plot displaying the week's best qualifying times. 
> Alias: `!qlaps`

### `!racelaps [series abbrev] (w#) (##s#)`
> Returns a table and scatter plot displaying the week's best race lap times. 
> Alias: `!rlaps`

### `!averageracelaps [series abbrev] (w#) (##s#)`
> Returns a table and scatter plot displaying the week's best average race lap times. 
> Alias: `!arlaps`

### `!incidents [series abbrev] (w#) (##s#)`
> Returns a table and scatter plot displaying the week's incidents per corner data. 
> Alias: `!incs`

### Utils:
### `!litres2gallons [number]`
> Converts gallons to litres. 
> Alias: `!l2g`

### `!celsius2fahrenheit [number]`
> Converts celsius to fahrenheit. 
> Alias: `!c2f`

### `!gallons2litres [number]`
> Converts gallons to litres. 
> Alias: `!g2l`

### `!fahrenheit2celsius [number]`
> Converts fahrenheit to celsius. 
> Alias: `!f2c`

### `!kph2mph [number]`
> Converts kilometers per hour to miles per hour. 
> Alias: `!k2m`

### `!mph2kph [number]`
> Converts miles per hour to kilometers per hour. 
> Alias: `!m2k`

### Team Subscriber Admin Commands:
### `!force_channel [#channel]`
> Configures the bot to only respond to commands run in a certain channel. Users will be reminded if they attempt to supply commands into other channels.

### `!default_series [series abbrev]`
> Sets the default series for a discord guild. With this set, if a command that requires a series abbrev is triggered with out a series being specified, it will fall back to the default.

### `!default_category [category]`
> Sets the default category for a discord guild.

### `!clear_defaults`
> Clears all default options for this discord guild.

### `!set_announce_options`
> Kicks off an interactive series of questions to allow configuration of the automatic announcements of race results for team drivers.

### `!set_announced_series [list of series abbrevs]`
> Sets the list of series to announce races from.

### `!set_series_channel [series abbrev] [#channel]`
> Creates a mapping between a series and a channel, such that any commands run in that channel will default to the provided series.

### `!add_driver [driver name] [color hex] [@discord handle]`
> Adds a driver to a discord guild.

### `!remove_driver [driver name]`
> Removes a driver to a discord guild.

### `!update_driver [driver name] [color hex]`
> Updates a driver's highlight color.

### `!bot_admin_role [@role]`
> Allows any discord user who has the mentioned role access to the bot admin commands for this server. Note: you'll need to make a new role, or use an existing one.

### Subscription Required Commands:
### `!points [series abbrev] (##s#)`
> Returns three pieces of information; a table displaying the top 5 drivers in the series, along with highlighted team drivers. A table showing the points each driver has locked in for each week of the season, highlighting dropped weeks and the lowest current week's points (so you know what you need to beat to improve). Finally a line chart is included to give a good visual overview of each driver's championship season.
> Alias: `!pts`

### `!week [series abbrev] (w#) (##s#)`
> Returns information about how many races the team's drivers have completed this week in the series, along with the number of championship points they have currently for the week.

### `!irgains [series abbrev] (w#) (##s#)`
> Returns information about the iRating gains/losses the team's drivers have had in the provided series.

### `!drivers (category) [irating|irchange|name]`
> Returns a list of the team's drivers, along with some basic information such as number of races for the season, current iRating and iRating gain/loss for the season. By default the driver's information will be for the category they've raced the most for the season, optionally you can specify a category type (road, oval, dirt, rx, offroad) to get the details for each driver in that category. Optional arguments of `irating`, `irchange`, and `name` are available to set the ordering of the list. Defaults to `irating`.

### `!drivers_division (category)`
> Returns a list of the division for each driver in the team.

### `!drivers_discord`
> Returns a list of the mapping to discord user for each driver in the team.

### `!drivers_color`
> Returns a list of the color hex code configured for each driver in the team.



