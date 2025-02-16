---
title: "Quartz TWW Season 1"
description: "Fun numbers from a fine season"
---

# Item Level, M+ Score, and Total M+ Completed by Day

Bubbles are colored by class and represent the number of M+ completed.

{{< chart "S1_ilvl_m+score_m+done.html" >}}

# Item Level Race by Day

{{< chart "S1_ilvl_race.html" >}}

# Item Level Over the Season

*Tap names in the legend to turn them on and off. Double-tap a name to toggle everything else off and on. 
Zoom by dragging a rectangle on the plot, and double-click it to reset.*

{{< chart "S1_ilvl_season_lines.html" >}}

# Weekly M+

This is M+ done over the course of each game week, so they build up as you do M+ during the week, then reset to zero 
on Tuesday. Darker colors are lower level keys, brighter colors are higher levels.

*You can zoom in for more detail on any one player, and hover for more detail. Double-click to reset zoom.*

{{< chart "S1_mplus_player_grid.html" >}}

# Total Dungeons Run

{{< chart "S1_total_team_dungeons.html" >}}

# Dungeons Run By Day

Total of each dungeon run each day of the season. 

Note the odd data on the first of the year. I *think* this is a bug
in the data from WoW Audit, but I need to dig deeper to be sure.

{{< chart "S1_team_dungeons_by_day.html" >}}


# Crests

All crest types earned over the season.

{{< chart "S1_crests_player_grid.html" >}}

# About the data

I captured the raw data which goes into
our [WoW Audit sheet](https://docs.google.com/spreadsheets/d/1DbjOMe0K3tkRHiYiK1Q8ak5ESCMuTLPm7iQgTfd2k_g/edit?gid=241918221#gid=241918221)
every hour throughout the season and dumped it into a MongoDB timeseries collection. You can see this data in the first
many rows of the [raw_data tab](https://docs.google.com/spreadsheets/d/1DbjOMe0K3tkRHiYiK1Q8ak5ESCMuTLPm7iQgTfd2k_g/edit?gid=1533083597#gid=1533083597).

I've done some minor data cleanup, and computed "game weeks" and "game days" for many of these plots.
Game days are assumed to start at 7am, except for Tuesdays.
The game week starts based on a best-effort recognition of the weekly reset.

TODO: toss all the code into github and link it here.

# About this site and the plots

I was never a web or user interface developer. I made these plots largely with the help of ChatGPT. The plots and this 
entire site is a bit janky, but I'm not currently inclined to put more effort into polishing it. 

If anyone has some experience in these areas, I'd be happy to have you help!


