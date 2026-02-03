# Used-Car-Dataset

## About
This notebook was adapted from a project of mine for the "CSMODEL" course of De La Salle University Manila. This project was done by group, and I feel fortunate that I worked with wonderful people for this.
In particular, this project was worked on by the following:
- Abiño, Renz Wendell
- Detablan, John Daniel
- Reynoso, Markus Nikolo
- Yap, Remus Guderian (*Yours truly*)

So, special thanks to them!

## Dataset

The dataset was built through web scraping from a website called [CarDekho](https://www.cardekho.com/) where used cars are listed. But since web scraping was used and no other additional information regarding the data collection was provided, there may be complications:

- **Data inaccuracy**. Errors or inconsistencies in the original listings from the website may happen such as null values, incorrect inputting of values, or even duplicate values.
- **Bias in listings**. It is likely that the web scraping was done sequentially from page 1 onwards. With this, the dataset may not represent the entire used car market population. Also, the website CarDekho is an Indian website and as we will see later on, majority of the cars for sale are from Indian car brands.

Each row of the dataframe corresponds to one car containing the attributes of the car, while each column corresponds to a specific attribute of the car. The dataset contains 8128 data points with 14 columns/attributes in total.

| Column Name            | Description |
|------------------------|-------------|
| `name`            | The name of the car model |
| `year`   | The year the car was manufactured |
| `selling_price`  | The selling price of the car in Indian currency. |
| `km_driven`           | The total kilometers driven by the car |
| `fuel`              | The type of fuel of the car |
| `seller_type`         | The type of seller (Individual, dealer, other) |
| `transmission`       | Type of transmission (Manual/Automatic) |
| `owner` | First owner, second owner, other |
| `fuel_efficiency`      | The fuel efficiency of the car (km/ltr/kg)|
| `engine`         | The car's engine measurement in cubic centimeters (cc). It refers to the amount of air and fuel that can be pushed through the cylinders in the engine.|
| `max_power`         | Brake Horsepower (BHP), a measure of actual usable power produced by an engine factoring friction|
| `seats`         | The number of seats in the car |

