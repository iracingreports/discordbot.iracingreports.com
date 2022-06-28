---
title: iRacing Reports Discord Bot - Commands
---

## Commands

In the examples below, square brackets have been used to show the required arguments for each command. Round brackets have been used to show optional arguments that can be provided to provide more fine grained responses.

For some commands you can specify a particular season. Unless specified, this will default to the current season. To select a different season you include **##s#** in the `season` field, where the first two numbers are the year and the final number is the season; for example **22s3** for 2022 Season 3.

For some commands where it makes sense, if you specify a multiclass series you will need to provide an argument to also specify which class you're interested in.

### Standard Commands:
### `/series_abbreviations (season: 22s3)`
> Displays a table of series and the abbreviations to use for each of them in all the other commands. You will be prompted to select the category.

### `/cars [series_abbrev: imsa] (class_abbrev: gt3) (season: 22s3)`
> Displays a list of cars in a class and the abbreviations to use for each of them in the other commands.

### `/balance [series_abbrev: imsa] (class_abbrev: gt3) (season: 22s3) (week: 1)`
> Displays information about the balance of performance for a class for a certain week of a series. Defaults to showing average race laps.

### `/schedule [series_abbrev: imsa] (season: 22s3)`
> Track schedule for a series. 

### `/driver [name: Driver Name] (category: ) (season: 22s3) (week: 1) (series abbrev)`
> Returns statistics about a driver's current season. If no category is provided the bot will return the output for the category that the driver has raced the most this season. You can also filter the information returned to a single series by providing a series abbreviation.

### `/previous_race [series_abbrev: imsa] (class_abbrev: gt3) (season: 22s3) (week: 1) (races_ago: 3)`
> Returns information about a driver's most recent race. If a number is supplied, say 3, in the `races_ago` field, the race 3 races ago will be displayed.

### `/previous_races [series_abbrev: imsa] (class_abbrev: gt3) (season: 22s3) (week: 1)`
> Returns a list of a driver's most recent 10 races.

### `/championship [series_abbrev: imsa] (season: 22s3)`
> Output a table displaying the top 30 drivers in the championship standings. 

### `/strengthoffield [series_abbrev: imsa] (season: 22s3) (week: 1)`
> Outputs a heatmap showing the strength of field of each time slot. 

### `/officialsessions [series_abbrev: imsa] (season: 22s3) (week: 1)`
> Outputs a heatmap showing the number of times each time slot had official sessions. 

### `/participation [series_abbrev: imsa] (season: 22s3) (week: 1)`
> Outputs a heatmap showing the participation for the series. 

### `/laps qualifying [series_abbrev: imsa] (class_abbrev: gt3) (season: 22s3) (week: 1) (division: 2) (highlight: "driver name") (chart_type: Scatter|Box)`
> Returns a table and chart displaying the week's best qualifying times. 

### `/laps race_fastest [series_abbrev: imsa] (class_abbrev: gt3) (season: 22s3) (week: 1) (division: 2) (highlight: "driver name") (chart_type: Scatter|Box)`
> Returns a table and chart displaying the week's best race lap times. 

### `/laps race_average [series_abbrev: imsa] (class_abbrev: gt3) (season: 22s3) (week: 1) (division: 2) (highlight: "driver name") (chart_type: Scatter|Box)`
> Returns a table and chart displaying the week's best average race lap times. 

### `/incidents [series_abbrev: imsa] (season: 22s3) (week: 1)`
> Returns a table and chart displaying the week's incidents per corner data. 

### Utils:
### `/convert litres_to_gallons [litres: 20]`
> Converts gallons to litres. 

### `/convert celsius_to_fahrenheit [celsius: 30]`
> Converts celsius to fahrenheit. 

### `/convert gallons_to_litres [gallons: 10]`
> Converts gallons to litres. 

### `/convert fahrenheit_to_celsius [fahrenheit: 90]`
> Converts fahrenheit to celsius. 

### `/convert kph_to_mph [kph: 160]`
> Converts kilometers per hour to miles per hour. 

### `/convert mph_to_kph [mph: 100]`
> Converts miles per hour to kilometers per hour. 

### Team Subscriber Admin Commands:
### `/manage_team add [name: Driver Name] [color: #5522ee] [discord_user: @discord_handle]`
> Adds a driver to a discord guild.

### `/manage_team remove [name: Driver Name]`
> Removes a driver to a discord guild.

### `/manage_team update [name: Driver Name] [color: #5522ee]`
> Updates a driver's highlight color.

### `/manage_team admin_role [role: @role]`
> Allows any discord user who has the mentioned role access to the bot admin commands for this server. Note: you'll need to make a new role, or use an existing one.

### Subscription Required Commands:
### `/points [series_abbrev: imsa] (season: 22s3)`
> Returns three pieces of information; a table displaying the top 5 drivers in the series, along with highlighted team drivers. A table showing the points each driver has locked in for each week of the season, highlighting dropped weeks and the lowest current week's points (so you know what you need to beat to improve). Finally a line chart is included to give a good visual overview of each driver's championship season.

### `/week [series_abbrev: imsa] (season: 22s3) (week: 1)`
> Returns information about how many races the team's drivers have completed this week in the series, along with the number of championship points they have currently for the week.

### `/irgains [series_abbrev: imsa] (season: 22s3) (week: 1)`
> Returns information about the iRating gains/losses the team's drivers have had in the provided series.

### `/team quick_stats (series_abbrev: imsa) (season: 22s3) (week: 1) (sortby: Name|iRating|iRaing Change)`
> Returns a list of the division for each driver in the team.

### `/team divisions (season: 22s3)`
> Returns a list of the division for each driver in the team.

### `/team discord_mappings`
> Returns a list of the mapping to discord user for each driver in the team.

### `/team colors`
> Returns a list of the color hex code configured for each driver in the team.



