---
title: iRacing Reports Discord Bot - Commands
---

## Commands

In the examples below, square brackets have been used to show the required arguments for each command. Round brackets have been used to show optional arguments that can be provided to provide more fine grained responses.

For some commands you can specify a particular season. Unless specified, this will default to the current season. To select a different season you include **##s#** in the `season` field, where the first two numbers are the year and the final number is the season; for example **22s3** for 2022 Season 3.

For some commands where it makes sense, if you specify a multiclass series you will need to provide an argument to also specify which class you're interested in.

### Standard Commands:
### `/cars [series] (class) (season)`
> Displays a list of cars in a class and the abbreviations to use for each of them in the other commands.

### `/balance [series] (class) (season) (week)`
> Displays information about the balance of performance for a class for a certain week of a series. Defaults to showing average race laps.

### `/schedule [series] (season)`
> Track schedule for a series. 

### `/driver [name] (category) (season) (week) (series)`
> Returns statistics about a driver's current season. If no category is provided the bot will return the output for the category that the driver has raced the most this season. You can also filter the information returned to a single series by providing a series abbreviation.

### `/previous_race [series] (class) (season) (week) (races_ago)`
> Returns information about a driver's most recent race. If a number is supplied, say 3, in the `races_ago` field, the race 3 races ago will be displayed.

### `/previous_races [series] (class) (season) (week)`
> Returns a list of a driver's most recent 10 races.

### `/championship [series] (season)`
> Output a table displaying the top 30 drivers in the championship standings. 

### `/strengthoffield [series] (season) (week)`
> Outputs a heatmap showing the strength of field of each time slot. 

### `/officialsessions [series] (season) (week)`
> Outputs a heatmap showing the number of times each time slot had official sessions. 

### `/participation [series] (season) (week)`
> Outputs a heatmap showing the participation for the series. 

### `/laps qualifying [series] (class) (season) (week) (division) (highlight) (chart_type)`
> Returns a table and chart displaying the week's best qualifying times. 

### `/laps race_fastest [series] (class) (season) (week) (division) (highlight) (chart_type)`
> Returns a table and chart displaying the week's best race lap times. 

### `/laps race_average [series] (class) (season) (week) (division) (highlight) (chart_type)`
> Returns a table and chart displaying the week's best average race lap times. 

### `/incidents [series] (season) (week)`
> Returns a table and chart displaying the week's incidents per corner data. 

### Utils:
### `/convert litres_to_gallons [litres]`
> Converts gallons to litres. 

### `/convert celsius_to_fahrenheit [celsius]`
> Converts celsius to fahrenheit. 

### `/convert gallons_to_litres [gallons]`
> Converts gallons to litres. 

### `/convert fahrenheit_to_celsius [fahrenheit]`
> Converts fahrenheit to celsius. 

### `/convert kph_to_mph [kph]`
> Converts kilometers per hour to miles per hour. 

### `/convert mph_to_kph [mph]`
> Converts miles per hour to kilometers per hour. 

### Team Subscriber Admin Commands:
### `/manage_team add [name] [color] [discord_user]`
> Adds a driver to a discord guild.

### `/manage_team remove [name]`
> Removes a driver to a discord guild.

### `/manage_team update [name] [color]`
> Updates a driver's highlight color.

### `/manage_team admin_role [role]`
> Allows any discord user who has the mentioned role access to the bot admin commands for this server. Note: you'll need to make a new role, or use an existing one.

### Subscription Required Commands:
### `/points [series] (season)`
> Returns three pieces of information; a table displaying the top 5 drivers in the series, along with highlighted team drivers. A table showing the points each driver has locked in for each week of the season, highlighting dropped weeks and the lowest current week's points (so you know what you need to beat to improve). Finally a line chart is included to give a good visual overview of each driver's championship season.

### `/week [series] (season) (week)`
> Returns information about how many races the team's drivers have completed this week in the series, along with the number of championship points they have currently for the week.

### `/irgains [series] (season) (week)`
> Returns information about the iRating gains/losses the team's drivers have had in the provided series.

### `/team quick_stats (series) (season) (week) (sortby)`
> Returns a list of the division for each driver in the team.

### `/team divisions (season)`
> Returns a list of the division for each driver in the team.

### `/team discord_mappings`
> Returns a list of the mapping to discord user for each driver in the team.

### `/team colors`
> Returns a list of the color hex code configured for each driver in the team.



