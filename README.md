# once-upon-a-game
 Presentation on data roles in business as part of the assessment of the Data Landscape module at the Data Analyst Program at Hyper Island - Stockholm.

---

Hi, my name is Guilherme and I'm going to talk a little bit about data in games.

Almost every game today collects player data. They are needed for testing, balancing and monetisation, so data is considered at every step from the very beginning of the game production until it's out in the wild.

But that story is better told backwards. We're gonna begin with the end.

Once upon a time, there were some players that never played the game again. And retention target for D1, which is the number of players that returned from D0, was way below 40%, the market average for top games. The product owner, an executive producer (stakeholder), had to make some decisions and approve some changes in the game.

For that, a Data Analyst created dashboards to see where the game lost players, using a funnel view with the most important player actions during D0. They could see that from a 100% of players that installed the game, not even 50% of them finished the tutorial. And the aimed 40% never finished the second round.

With a plethora of visualisation tools, some of them even tailor made by the Data Engineers for the studio, they got a better sense of where and how to act.

But they only could do that because the data they had were sound. And that's another problem.

How to ensure the accuracy, quality and availability of data generated in the game?

Data Analysts, Data Scientists, basically all the data team responsible for delivering reports (stakeholders) relied on the Data Engineers and Quality Assurance Analysts that created and tested the pipelines and APIs with which the data were retrieved and stored. They were responsible for the data architecture.

They used Java to build the APIs, Python to write distributed ETL pipelines (extract, transform and load), SQL or Golang, MongoDB for the databases. So that all the data created would be properly cleaned, tagged, organised, stored and made easily available for analyses. Easily said, but hard to do.

And how did they know the kind of data they should retrieve? Which events in the game triggered the acquisition of data? That's finally the beginning of the story.

To keep an eye for the right data, The Data Scientists worked closely with the Producers and Game Designers (stakeholders) to know what to track.

For example, the Game Combat Designers wanted to know which weapons were the most used and what was the win rate of each one; the Game Economy Designers, responsible for balancing and keeping track of engagement in the game, needed to know how many matches were played per session and how many sessions a player had per day.

With something as simple as a spreadsheet, they came up with a tracking plan, a tracking design with all the events that had to be implemented in the game that would trigger the acquisition of data — for example, a match, the fight with a boss, accepting a quest, when items were found or bought. And that design was handed to the programmers or even data engineers, at the very first development stages of the game.

So once upon a game, data were designed, implemented, tracked, retrieved, transformed, stored and visualised.
