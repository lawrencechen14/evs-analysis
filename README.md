# Beyond EVs: Electric Vehicles Data Analysis

We are performing an analysis of electric vehicles, specifically of what factors are associated with electric vehicle adoption, how we can model and forecast EV adoption towards the future, how existing electrical infrastructure needs to change to adapt to increased EV adoption rates, and how can we display our findings clearly.

Our project is comprised of four major parts:
- Exploratory data analysis of an electric vehicle population in a certain geographic area.
- Constructing a machine learning model that forecasts electric vehicle adoption in the area.
- Feeding the output of the forecasting model as an input to another model that determines the sustainability of electrical infrastructure given increased adoption of EVs.
- Creating a map that displays which areas of the geographic area is most susceptible to strain on their electrical infrastructure due to EVs.

## Solution Demo

For our solution, we created an interactive map that highlights our findings on infrastructure preparedness by ZIP code for electric vehicle energy consumption in Washington State. Users can hover over areas of the map to learn more about each ZIP code. This map details how many additional EVs each ZIP code’s electric infrastructure can support at a certain year, for all years between 2021 and 2050. On the map, green ZIP codes have a good amount of remaining energy capacity to support many more electric vehicles, while the yellow ZIP codes have less capacity, and red ZIP codes have the least.

<img width="925" alt="Screen Shot 2020-04-27 at 8 48 36 PM" src="https://user-images.githubusercontent.com/21212020/81616786-00262280-9399-11ea-9448-77020e1f0c60.png">

#### Figure 1: Map of Washington State displaying remaining number of EVs each ZIP code can support.

Each ZIP code also has its own marker, which is hidden behind a marker cluster, so that the map does not get too cluttered. Clicking on the cluster allows the user to zoom into parts of the map. Also for each marker, the tooltip provides information about the ZIP code number, city and county, and clicking it gives the user information about the population and how many EVs its energy infrastructure can support.

<img width="1203" alt="Screen Shot 2020-04-27 at 8 51 33 PM" src="https://user-images.githubusercontent.com/21212020/81616885-3368b180-9399-11ea-8011-9a406d45ddb0.png">

#### Figure 2: Tooltips and extra information providing ZIP codes, city and county, and population statistics.

### Packages Used
The main packages that we used for our project was the `sklearn` Linear Regression model, `statsmodels` ARIMA model, and the `folium` map visualization library. These libraries are linked below:

- Sci-kit Learn Linear Regression Model: https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.LinearRegression.html
- Statsmodels ARIMA Model: https://www.statsmodels.org/stable/generated/statsmodels.tsa.arima_model.ARIMA.html
- Python Folium Visualization: https://python-visualization.github.io/folium/

## Accessing the Interactive Maps
In order to view the solution demo, you need to clone or download the repository and navigate to the appropriate directory. The full maps are included in the `markered-maps` folder in this GitHub repository. Each map is an HTML file that can be viewed by opening it in a web browser, preferably Google Chrome or Firefox. In order to access the interactive map, follow these steps:

1. Clone the repository.
2. Change into the `markered-maps` directory.
3. Open one of the three sample maps with a web browser, and the map will be displayed on the browser.

## Running the Code

#### For demoing purposes, it is not recommended to run the Jupyter notebook code but rather to access the interactive maps as outlined in the above section.
The code is all localized to a Jupyter notebook, so to run the code, you must either:

1. Install the Jupyter notebook through `pip` or `conda` by following the instructions here: https://jupyter.org/install
2. Download a Python 3 Anaconda distribution through this site: https://www.anaconda.com/products/individual

*Note that the code will not run correctly without the datasets being linked to certain paths, but since these datasets were quite large they are not included in this repository. The datasets can be pulled however from online public sources.*


