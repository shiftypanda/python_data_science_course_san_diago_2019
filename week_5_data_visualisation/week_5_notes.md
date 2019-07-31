# week 5 notes

## types of visulasiations
https://youtu.be/iyERyfDJtl4

## key design principles
https://youtu.be/Lsjm0PSDekQ

### Elegance
* Elegance of presenting of findings, map overlay colour scheme clear display of information rather than numerics
* focus on what is relevant
* be stylish if possible


## Notebook: Data Visualization
Bookmark this page
Please download the notebooks for this week so you can follow along with us during the videos and play with the code yourself.

## matplotlib
https://youtu.be/B8c45qzsESU

* easy to produce quick plots of data
matplotlib tries to make easy things easy and hard things possible
https://matplotlib.org/

lots of other tools
seaborn, ggplot, altair, bokeh, plotly, folium




## world development indicators
https://youtu.be/PK_8cXbaRik

## basic plotting in matplotlib part 1
https://youtu.be/cYFY-ZgM6yU

explring CO2 emissions for united states
plot.plot command to make basic plot

plt.title('C02 emissions;)

plt.hist() creates histogram
pass it ndarray, then 10 for number of bins, noraml false, faceolor
e.g. plt.hist(hist_data, 10, density=False, facecolor='green')

slect differnet year

plotting histogram against different other countries

plt.subplots() gives figure and axis back seperately

plt.hist calling 
plt.hist(co2_2011['Value'], 10, normed=False, facecolor='green')

annotate method allowing to show poiting to one specific places
ax.annotate("USA",
            xy=(18, 5), xycoords='data',
            xytext=(18, 30), textcoords='data',
            arrowprops=dict(arrowstyle="->",
                            connectionstyle="arc3"),
            )

common features from matplotlib
- bar chart
- axes
- axes labels
- figure labels
- legend
- asesthetics
- annotatinos



## basic plotting in matplotlib part 2
https://youtu.be/GlR-V0GtRfE

Second part of dat set
aim to look at line charts and scatterplots

calling min anx max on columns so that they are on the same year and staging
needing to truncate areas if shows mroe ifnormation on it

really helpful to look at the commands for plttoign groups
remembienr msot of thet ime i would be creating a mask intialyl to gather right data and then send that thorugh to the matplotlib library for further display.

I experiement with UK data and produced some interseting additios showing there has acutaly been a decline in CO2 emissions over time.


## matplotlib additional examples
https://youtu.be/Tw_VXI5xiqM

lots of differnet other way sto display informaiton
short scritps to go through and check for any missing data



## folium example
https://youtu.be/mOU59G29V7o

when importing and installing on conda use conda install -c folium conda-forge

chloropleth maps binds panda data frame and json geometreis
key_on what to link features to

note funciotn now depcreated shoudl use class instead



## Visualization Libraries
Bookmark this page
The following list provides a few plotting libraries for you to get started based on their use case(s).  This list is focused on providing a few solid options for each case rather than overwhelming you with the variety of options available.

The foundation: Matplotlib, most used plotting library, best for two-dimensional non-interactive plots. A possible replacement is pygal, it provides similar functionality but generates vector graphics SVG output and has a more user-friendly interface.

Specific use cases:

Specialized statistical plots, like automatically fitting a linear regression with confidence interval or like scatter plots color-coded by category.

seaborn: it builds on top of Matplotlib and it can also be used as a replacement for matplotlib just for an easier way to specify color palettes and plotting aestetics
Grammar of graphics plotting, if you find the interface of Matplotlib too verbose, Python provides packages based on a different paradigm of plot syntax based on R's ggplot2

ggplot: it provides similar functionality to Matplotlib and is also based on Matplotlib but provides a different interface.
altair: it has a simpler interface compared to ggplot and generates Javascript based plots easily embeddable into the Jupyter Notebook or exported as PNG.
Interactive plots, i.e. pan, zoom that work in the Jupyter Notebooks but also can be exported as Javascript to work standalone on a webpage.

bokeh: maintained by Continuum Analytics, the company behind Anaconda
plotly: is both a library and a cloud service where you can store and share your visualizations (it has free/paid accounts)
Interactive map visualization

*folium: Creates HTML pages that include the Leaflet.js javascript plotting library to display data on top of maps. *plotly: it supports color-coded country/world maps embedded in the Jupyter Notebook.

Realtime plots that update with streaming data, even integrated in a dashboard with user interaction.

bokeh plot server: it is part of Bokeh but requires to launch a separate Python process that takes care of responding to events from User Interface or from streaming data updates.
3D plots are not easy to interpret, it is worth first consider if a combination of 2D plots could provide a better insight into the data

mplot3d: Matplotlib tookit for 3D visualization

## Notebook: Coding Practice
Bookmark this page
It's important to get practice with the programming concepts of the week.  If you haven't already done so, please download the notebooks for this week and work through the examples.

If you are wanting to practice and test your knowledge by developing other notebooks, you can access these by signing up for the Verified Certificate program -- for those looking to more robustly document their knowledge and skills.  This can also put you on the path to earning a MicroMasters in Data Science, if that would be helpful to you!

## case study 1 cholera
https://youtu.be/U_D6TwZKQWQ

case study looking at data visualtion in undersntaindg how chororea spread
remains public health threat
bacteira infeciton diarrhea

1854 identifeid how cholera spread
well water contamination
was thought to be due to smelling something bad
John Snow - scientist, anaesthetist theory that cholera 1839 was waterborne
lived near to find where everyone who got the water from and deaths
outliers helpful for idenitnfy why things were happenign, workhouse had noinfecitosn in area of braod street because they had their own water supply
baby had become ill with cholera near to pump, they had not disposed of nappiy waste problay wentinto cesspit that then filetered into the water pump
this then led to water sanitation

he completed map to visualise the deaths from choelra related to pump


## case stud 2 napoleans march
https://youtu.be/4PDBHBX9d1o

frances russian campaign of nappoelas russian campaingin 1812
Charles Jospeh Minard
using visualisations in statistics

lines showing nameof river with startof troop number and then at end of campaing
plan was to attack smaller russian army near border
however russian army refused to engage french army in direct conflict, they would retareat destroyign supplies
after invading moscow waited for surrender for over a month btu didnt happen and witner started to set in. They were attacekd whilst fleeing by russian army.
Temperatures often below zero

6 differnet types of data being displayed
- lat, longof army
- size of army
- dist traveled
- temperature during retreated


## Case Study 3 - Interactive Visualization of World Data
Bookmark this page
One of the pioneering educators of Data Visualization, Professor Hans Rosling's videos on world development have inspired a whole generation of data scientists.  Please feel free to watch this short clip from BBC below:

200 Countries, 200 Years, 4 Minutes - The Joy of Stats

Hans Rosing passed away February 7, 2017.  We encourage you to read more about his life and achievements in his obituary.

sources 
https://www.youtube.com/watch?v=jbkSRLYSojo
https://www.theguardian.com/global-development/2017/feb/07/hans-rosling-obituary

Global health working to show
animating data 

life expectancy, showing Prof Hans Roslings 
