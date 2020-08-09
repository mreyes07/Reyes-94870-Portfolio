
# Reyes-94870-Portfolio
Victoriano Reye’s Profolio Telling Stories with Data Summer 2020 at Carnegie Mellon University. 

-[About Me](#about-me)

# About Me
My name is Vic, my pronouns are he/him, and I am in the Arts Management Program at Heinz. I previously worked at the Thomas Merton Center doing data management. I’m currently a volunteer with SistersPGH, Covaid.co, and Pittsburgh Mutual Aid doing case management and fundraising. My plans after graduation are to find a job in the social service sector, publish comics, and get a cat.

# What I Hope To Learn
I don’t have much formal teaching on data visualization so it is all pretty new to me. I mostly hope to learn better design techniques for communicating complex information as well as simple data visualization software techniques.

# Portfolio
## Assignment: Visualizing Government Debt

All these charts use the same data from OECD.org which has the debt-to-GDP ratio of countries all over the world over time. The debt-to-GDP ratio is described on the website as “Debt is calculated as the sum of the following liability categories (as applicable): currency and deposits; debt securities, loans; insurance, pensions and standardised guarantee schemes, and other accounts payable.” Data is missing for some years including 2019. 

Despite all charts using the same data, the three charts below communicate different things and have different uses. As shown in the Visual Vocabulary document from FT graphic, bar graphs communicate a ranking. In this case the ranking is of countries that have the most debt. This chart is the easiest to understand of the three. It gives us a clear line up and uses a simple color palette with enough contrast to clearly see different elements. The list of countries is hard to read because it is slanted and cramped but, the mouse over tabs clear up information so this didn’t confuse me too much.
<iframe src="https://data.oecd.org/chart/61Ls" width="950" height="713" style="border: 0" mozallowfullscreen="true" webkitallowfullscreen="true" allowfullscreen="true"><a href="https://data.oecd.org/chart/61Ls" target="_blank">OECD Chart: General government debt, Total, % of GDP, Annual, 2015</a></iframe>

The second chart is the hardest to read for me. It is a compilation of multiple charts smushed into one. It is useful in giving a picture of the patterns of each country's debt. It is also taking the extra step from the first graph and communicating debt overtime. It is hard to get a hold of at first but it is communicating a lot of information and is the best at emphasizing each individual country's debt and probably would be best for predicting the future debt of a country. However, it would be hard to read if you wanted to compare countries two each other for a given year, like done in the first graph.
<div class="flourish-embed flourish-chart" data-src="visualisation/3178225" data-url="https://flo.uri.sh/visualisation/3178225/embed"><script src="https://public.flourish.studio/resources/embed.js"></script></div>

In my third graph I attempted to make a graph that communicates the information of the second graph while also showing a country ranking from year to year. I created a dot graph which also contains a time lapse. I also added a color gradient so it would be easier to see changes that were drastic overtime. I was trying to communicate a lot in this graph. It does not illustrate patterns of individual countries over time as the fist one does. However, I think it is successful showing broad shifts in countries while still being able to easily compare them over the years. It is definitely not as clear as the first graph but it has the added benefit of showing shifts over time.
<div class="flourish-embed flourish-scatter" data-src="visualisation/3186746" data-url="https://flo.uri.sh/visualisation/3186746/embed"><script src="https://public.flourish.studio/resources/embed.js"></script></div>

All graphs could use some rewoking in terms of labeling and decription. What the Debt-to-GDP and Total % of GDP could be explained or phrased more clearly for the average viewer. The title could also do a better job at illustrating why we are looking at the graph in the first place and why it is important or interesting.

## Assignment: Critique by Design

<img src="https://c0.piktochart.com/v2/uploads/4ff5230e-f2eb-4016-9187-64a2e6ef86d3/6eeebab7684f656d9d7f3fc005c5f43bbd98d575_original.png?1569845676=" alt="It's not about crime">

I choose to redesign the It's not about crime plot from the website https://mappingpoliceviolence.org/. I choose this graph because I think this website is an incredibly clear and accessible way to get information on police violence data but this graph was the hardest for me to understand. The statement is clear, that there is no correlation between violent crimes and killings by police. However, the choice to do a 3 way axis with a limited number of cities confused me and made it harder to understand the chart. Additionally the rate for police killings and the rate for violent crime were not calculated the same way and while one had an axis of 0-20, the other had an axis of 0-12. I felt that the chart could be seen as miss leading to a viewer who was on the fence about these topics and I felt the chart could communicate the same information while being less manipulated.

In my first wireframes I attempted to make the chart as simple as possible and tested different variables that could communicate the same information. I put only two variables and plotted the axis to better show the correlation (or lack thereof) between violent crime and the number of police killings. I felt this proved the point about the lack of relationship better than plotting each individual city twice.
<img src="https://user-images.githubusercontent.com/14946947/88243898-e38f4c00-cc5f-11ea-9b8d-80fc3c169ed8.png" alt="sketch 1">
<img src="https://user-images.githubusercontent.com/14946947/88243892-df632e80-cc5f-11ea-883d-506a2ae7892e.png" alt="sketch 2">

I showed these sketches to two of my housemates (one is a neuroscientist and the other is an artist) and the beast insights I got was that:
1. While they could easily tell what the graph was trying to say to them, they struggled to understand the scope of the data and what each point was. 
2. The Xs were confusing and it would be better for me to use circles.
3. I shouldn't use one variable that is measured by rate and one that is measured by raw number as this is still being deceiving. 

I took these insights into consideration and made a second wire frame that would be the guide for my final visualization. In this version I adjusted the rate of average crime so that it was by population per 1M to match the rate of police killing. I also added the information about the rate into the axis titles as done in the original graph. Additionally, I added more description into the subheadings to specify that each data point is a police department.
<img src="https://user-images.githubusercontent.com/14946947/88243888-db371100-cc5f-11ea-9a25-c1c1a6e6bc51.png" alt="sketch 3">

The first step to creating this graph was making minor adjustments to how rate was calculated in the data. However, when I did this the numbers for crime rate were much higher than even just the raw number. I did not want to portray the data this way because I felt it would mislead people on how much crime there actually is. I tried to adjust the rate of killings by police to per population of 1K but when doing that many of the numbers dropped to less than 0. I felt like this rate would make the killings rate to abstract and would be harder to read the graph. I tried to then just graph the plot by raw numbers but the graph turned out to make a much less effective visual. Additionally I realized that using raw numbers was not as meaningful without context of population.
<img src="https://user-images.githubusercontent.com/14946947/88243756-78457a00-cc5f-11ea-8de6-af7c6d5cd9ce.png" alt="first try">

The final design did not end up being as different as the original as I had initially imagined. However, I think it is still more successful at illustrating a lack of relationship. After this exercise I have a better appreciation for the original as I struggled for hours trying out different variables and couldn't come up with a design that was much different.
<img src="https://user-images.githubusercontent.com/14946947/88246235-e7bf6780-cc67-11ea-913f-cc62b94b2cb1.png" alt="it's not about crime redesign">

## Assignment: Final, The Danger of Criminalizing Sex Work
<a href="https://carnegiemellon.shorthandstories.com/the-danger-of-criminalizing-sex-work/index.html">Final Project</a>
<br>
<br>
<a href="https://mreyes07.github.io/Reyes-94870-Portfolio/final_project_VicReyes.html">Documentation</a>

