# Data Visualization Project

## Data

The data I propose to visualize for my project is a dataset of information about Airbnbs around Europe.
[Dataset](https://zenodo.org/records/4446043#.ZEV8d-zMI-R)


## Questions & Tasks

The following tasks and questions will drive the visualization and interaction decisions for this project:

 * How does the location of a rental affect its price?
 * How does the proximity of rental to a major city affect its price or quality?
 * How does the cleanliness of a rental affect its overall ratings?
 * What effects does the number of people staying in a rental have on its guest satisfaction?
 * Do rentals closer to train stations or restaurants differ in ratings?

## Sketches
![1758123890 3134089](https://github.com/user-attachments/assets/3f6978a4-5f32-407f-8cf1-f76a2fff8e70)
I really like the Voronoi style Viz, as it can show how attributes of a rental change depending on the proximity to a hub city.

## Prototypes
<img width="960" height="500" alt="image" src="https://github.com/user-attachments/assets/b95e937f-877e-4e2b-8582-753737548b25" />
I have made this prototype scatterplot/heatmap, which maps the longitude and latitude (geographic location) of a rental on the X and Y axis, with the color showing the normalized attraction index (how close it is to a nearby tourist attraction).

## Milestones
Each week, I would like to come up with a new iteration of the viz, exploring how I can use different viz techniques in the same dataset to unlock new insights.


## Update 1 (Week 6)
I have tried to answer the question of "How does the price of a unit compare across its capacity?".
After visualizing this, there is a clear upwards trend on the average price as the person capacity increases. However, maximum price for a 2/3 person unit is higher than a 4/5/6 person unit. This could be a due to "extreme luxury" rentals meant for couples getaways.
https://vizhub.com/Camo651/90bec3308ff24ef8aa91ecedff0e38bc
<img width="957" height="483" alt="Screenshot 2025-10-01 104221" src="https://github.com/user-attachments/assets/3165d469-e816-49ba-9f11-9ad76c014812" />

## Update 2 (Week 7)
I have continued to explore the previous question. This week, I explored how distributions can be more effectively displayed. After some trial and error, the solution I came up with was to use a "scatterplot-like" system where each candlestick bar on the chart is not just a box, but a blob of points made up of each datapoint. This allows you to see the min/avg/max as before, but now the more detailed distribution of each candlestick on the plot.
<img width="952" height="478" alt="Screenshot 2025-10-08 064259" src="https://github.com/user-attachments/assets/c24821de-72d9-4ecd-b2b5-2dc8a1c23353" />
