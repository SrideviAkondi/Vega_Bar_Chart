# Vega_Bar_Chart
Created interactive multiform visualization system in Tableau and separate single forms in Vega

The visualization system should contain two views:
- A choropleth map on the left that shows state boundaries and uses a sequential segmented colormap to encode the total amount of losses 
- A bar chart on the right that expresses the amount of loss with aligned horizontal position and separates the damage type with vertical position.
- The colormap encodes the sum aggregated losses of all types of damage
- The bar chart encodes the sum aggregated losses for all the states

### The two data files are provided: 
- us-10m.json – containing state boundaries
- losses2015_transformed.csv – containing the 2015 indemnities per state

### Interaction and linked views: 
- When the user hovers over a state on the left view then the bar chart will show only the data related to that state. 
- Aggregation of losses is no longer over the entire US, rather it is only over the highlighted state (e.g. TX)
- When the user hovers over a bar corresponding to a specific type of damage then the map encodes only the data related to that damage.
- Aggregation of losses is no longer over all damage types, rather it is only over the highlighted damage (e.g. Drought)
