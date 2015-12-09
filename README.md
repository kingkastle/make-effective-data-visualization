## Summary:
This project is part of the Udacity Data Analyst Nanodegree Project 5, with the aim of sharing knowledge with others.
This is a dimplejs example based on the flight data from RITA that you can find at:

http://stat-computing.org/dataexpo/2009/the-data.html

The graph represents the evolution in terms of number of flights per year versus total distance accumulated per airline per year for the period between 1988 to 2008.

Check it out in b.locks: http://bl.ocks.org/kingkastle/raw/7188565a417968331fda/

## Story:
This graph represents the evolution of the commercial aviation, in particular US airlines during the period 1988-2008, the main parameters represented are:

  - Total flights per year
  - Average Flight Distance per year
  - Total Airlines per year
  
Based on these variables and its evolution during the period, the following conclusions can be made:

1. Constant increase of the Average flight distance: While years pass there is a constant increase of the average flight distance for all airlines, a probable reason for this would be the technological evolution of the aircrafts. It seems airlines compete each other to reach new destinations further away or create new further appart connections.
2. Increase of the Number of Flights: In the overall, the amount of flights per year gradually increases except for two particular years: 2002 and 2008. As we know, 11-September 2002 and economical crisis in 2008 could be the events to explain this decrease in the overall number of flights.
3. Market fragmentation: What happend after 2002? there are a bunch of new airlines into play, after the aviation crisis in 2002 new investors invested in new airlines?... These questions go beyond the scope of this graph.

## Older Versions

The files: 
  · output_previous.tsv
  · index_previous.html

Correspond to the previous dimple graph submmited, but after instructors' notes, this version was disregarded.

## Design

This current version is much simpler, in terms of coding, than the previous version. However it is much easier to interpretate.

This current version is motivated by the comment of the last instructor's review:
"I do think this visualization (Previous visualization, in this case) is explanatory and that you've found a really interesting story to tell (average flight distance is increasing and airlines are flying more flights). My only criticism is on the design choices and how the information is displayed. This project can be very subjective to grade, but I think there is a clearer way to encode the information so that your story really comes through. I made a rough draft plot in R that I'd like you to consider. http://postimg.org/image/dbgq31bb9/ My version is quite over plotted, but I've changed the encoding so that year is on the x-axis, plot type is a line chart, average flight is on the y-axis, and point radius is the number of flights. Your main conclusions about the data have to do with time (story section 1, 2 and 5). It's important to feature the time variable as a position encoding because it's so important to your story (position is usually the most important encoding for a reader). To avoid over plotting, you could actually make multiple plots based on market strategy: one plot for the big legacy airlines, one plot for regional short distance airlines. Or categorize airline by market type and give airlines with the same market type the same color. Right now, it's really hard for me to follow the trends over time. I have to mentally choose an airline, and with each new year try to locate its color as it skips around. But I can't really follow two airlines at once to compare them or see general trends over time because so many airlines come in and out of the data set. But again, I like the story you're telling."

So, starting from instructor's example, I decided to focus on the main bullets that the graph wants to convey:

1. Evolution of the flight per year
2. Evolution of the average flight distance per year
3. Evolution in the number of airlines

Based on these points, I created this simple graph which clearly shows the evolution of this points. At this stage, I don't try to create a fancy graph, like the previous one, but a graph that conveys the right message in the simplest possible way. So in the x-axis is represented the time variable, the first y-axis includes the total flights per year computed for all airlines, secondary y-axis includes the averaged flight distance averaged for all airlines per year and the bar chart includes the total number of airlines per year.

To end, contrary to the instructor's recomendation of representing all the airlines, I prefer to represent the resulting numbers of all of them, as I think this is a better way to convey the right message and of course, avoid overplotting issues that may confuse readers.



## How to use it

1. Download the data from the RITA portal: http://stat-computing.org/dataexpo/2009/the-data.html
2. Download the carriers.csv file from: http://stat-computing.org/dataexpo/2009/carriers.csv
3. In the Python file, on line 4, change the path to use the one where all your downloaded files from the previous points are
4. The Python file creates the file: "output3.tsv", place this file where index.html is
5. Open index.html and enjoy!

## Resources

Main resource used is: http://dimplejs.org/advanced_examples_viewer.html?id=advanced_storyboard_control

## Feedback

Here are some comments I received from some colleagues:

Colleague 1: 
What do you notice in the visualization?
Every year is quite different for each airline.
What questions do you have about the data?
It looks there is a lot of variation from year to year
What relationships do you notice?
Flights increase per year
What do you think is the main takeaway from this visualization?
Everything changes each year.
Is there something you don’t understand in the graphic?
Everything is clear for me, all is easy to see in this graph.

Colleague 2: 
What do you notice in the visualization?
There is an almost linear increase of the flights per year except for 2002, probably due to September 11?
…
What questions do you have about the data?
None, it is clear info.
…
What relationships do you notice?
1) Seems to be a linear correlation between flight number and distance per airline
2) Seems not to be any correlation between average delay per flight and number of flights per year or distance.
…
What do you think is the main takeaway from this visualization?
Basically, the selection of these 3 variables.
…
Is there something you don’t understand in the graphic?
No

Colleague 3:
What do you notice in the visualization?
You can see how airlines increase their business (number of flights) and how airlines evolve through the years.
What questions do you have about the data? 
I can find a correlation between delay and distance or number of flights.
What relationships do you notice? 
Number of flights and distance are correlated.
What do you think is the main takeaway from this visualization?
See the market evolution
Is there something you don’t understand in the graphic? 
Everything is clear

Udacity Coach:
He inspired most of the changes since the first version.


