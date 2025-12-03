# Airbnb Data Analysis
#### A Practical Visualization Project

## The Dataset
The data used for this project is a set collected from Zenodo, which catalogs attributes about Airbnb rental vacation homes throughout major cities in Europe.
[Dataset](https://zenodo.org/records/4446043#.ZEV8d-zMI-R)

### Questions & Tasks
The exploration of the dataset aims to answer the following research questions:
 * How does the location of a rental affect its price?
 * How does the proximity of rental to a major city affect its price or quality?
 * How does the cleanliness of a rental affect its overall ratings?
 * What effects does the number of people staying in a rental have on its guest satisfaction?
 * Do rentals closer to train stations or restaurants differ in ratings?
## Initial Designs
### Sketches
![1758123890 3134089](https://github.com/user-attachments/assets/3f6978a4-5f32-407f-8cf1-f76a2fff8e70)
A series of preliminary sketches was outlined to rapidly ideate upon potential methods for visualizing the dataset. Shown above are a heatmap-style of rental unit pricing and a Voronoi-style diagram of the distance of units to the center of major cities.

### Prototypes
<img width="960" height="500" alt="image" src="https://github.com/user-attachments/assets/b95e937f-877e-4e2b-8582-753737548b25" />
For an initial prototype, I created a scatterplot/heatmap, which maps the longitude and latitude (geographic location) of a rental on the X and Y axis, with the color showing the normalized attraction index (how close it is to a nearby tourist attraction).

## Iterative Development
To ensure development progress, I outlined development milestones. The goal was that each week, I would come up with a new iteration of the viz, exploring how I can use different viz techniques in the same dataset to unlock new insights.


### Iteration 1
##### (Week 6)
I have tried to answer the question of "How does the price of a unit compare across its capacity?".
After visualizing this, there is a clear upwards trend on the average price as the person capacity increases. However, maximum price for a 2/3 person unit is higher than a 4/5/6 person unit. This could be a due to "extreme luxury" rentals meant for couples getaways.
https://vizhub.com/Camo651/90bec3308ff24ef8aa91ecedff0e38bc
<img width="957" height="483" alt="Screenshot 2025-10-01 104221" src="https://github.com/user-attachments/assets/3165d469-e816-49ba-9f11-9ad76c014812" />

### Iteration 2
##### (Week 7)
I have continued to explore the previous question. This week, I explored how distributions can be more effectively displayed. After some trial and error, the solution I came up with was to use a "scatterplot-like" system where each candlestick bar on the chart is not just a box, but a blob of points made up of each datapoint. This allows you to see the min/avg/max as before, but now the more detailed distribution of each candlestick on the plot.
<img width="952" height="478" alt="Screenshot 2025-10-08 064259" src="https://github.com/user-attachments/assets/c24821de-72d9-4ecd-b2b5-2dc8a1c23353" />

### Iteration 3
##### (Week 9)
This week, I have added color as a way to visualize the data. Previously the chart showed the density of its listings by how "packed" the bar was at that point, but I was not happy with that as it was not a very accurate way to see the data, though it looked nice and conveyed other helpful information. This week, I switched the scatterplot style bars to be heatmap style bars, which show the density of listings across the Y axis. This immediately changes what the data shows, which is that the vast majority of listings fall around the cheaper 2-person type. This was not shown well previously. I ultimately choose to use a blue to yellow gradient to represent the density gradient for accessability reasons, as blue and yellow remain contrasting in normal vision and in the major variants of colorblindness.
https://vizhub.com/Camo651/990cbdc9456245f4983543fcab127981
<img width="1036" height="623" alt="Screenshot 2025-10-22 073427" src="https://github.com/user-attachments/assets/9bd8e141-b61e-4ab8-8db1-c2e8b377e9dd" />

### Iteration 4
##### (Week 10)
This week I added interactivity to the viz in the form of selectors and a slider that allows the user to dynamically manipulate what is shown on the graph to make it easier to garner insignts from the chart.
https://vizhub.com/Camo651/f72935e7972344f5b31d38b78164c6fa
<img width="916" height="477" alt="image" src="https://github.com/user-attachments/assets/1bc602ec-1e66-4315-8e62-d777f8159b38" />

### Iteration 5
##### (Week 11)
This week I added more interactivity support, allowing for selecting multiple cities at once and having their data combined into 1 big viz. For polishing, I added a display map for the axis/filter names (not just raw column names), and put a title on the viz that dynamically updates to reflect what is being shown.
https://vizhub.com/Camo651/65f8fb81e64c4429a73ec5c18add7108
<img width="1332" height="862" alt="Screenshot 2025-11-05 081758" src="https://github.com/user-attachments/assets/38ee21c8-c92d-4e0a-9af8-c1f15157aa85" />

### Iteration 6
##### (Week 12)
This week I added a tooltip that shows the exact value the user is hovered over on the chat, as well as a sidebar with explanations for what each selectable attribute means in the context of Airbnb rentals.
https://vizhub.com/Camo651/c566afe81b104ca9aaff06ade5600122
<img width="1277" height="658" alt="image" src="https://github.com/user-attachments/assets/57f506f0-7df4-4acc-b8a7-8d1c73761d19" />

### Final Iteration
##### (Week 15)
This week, for the final iteration, I added per-column density calculations, logarithmic density scaling, and converted it to grayscale for clarity.
https://vizhub.com/Camo651/1245d63438794011a9a7bdc7f2822022
<img width="1269" height="710" alt="image" src="https://github.com/user-attachments/assets/32fbd7b1-2fc9-46d8-8468-2880cbfc242c" />
