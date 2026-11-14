# finalProject
For use in the class I'm taking.

It's all well and good to do cool data manipulation, but...
## What do we gain from it?

In this case, we're learning a lot about fruit and vegetables, and the average economics surrounding them.

Example: AverageRetailPrice vs. AveragePricePerCupEquivalent has a correlation value of 0.590135, meaning they're moderately positively correlated. Those were a lot of big math words, but essentially it means if something has a higher sticker price, it will generally cost more per cup you eat. 

Example 2: PreparationYieldFactor vs. AveragePricePerCupEquivalent has -0.290670, indicating a moderate negative relationship. This means that as the yield of your food goes up, the price goes down. (Like when you use apple juice concentrate and add water, making the actual price per cup of the final product incredibly low.)

This is great info, but it's also just info. What did I learn from my visualizations?

insert visualizations and what I learned here

Now that you (hopefully) understand what this project is meant to accomplish, here's how I did it:
### Step 1 and Step 2: Find a Dataset, and Import it

I got my CSVs from the links below.
https://www.ers.usda.gov/data-products/fruit-and-vegetable-prices 

(https://www.ers.usda.gov/media/6240/all-vegetables-average-prices-csv-format.csv?v=33692) 

(https://www.ers.usda.gov/media/6210/all-fruits-average-prices-csv-format.csv?v=54815) 

Now that I have the data, I can import it like so:

```
import pandas as pd
fruit = pd.read_csv('fruit-prices-2023.csv')
veg = pd.read_csv('vegetable-prices-2023.csv')
```

### Step 3: Data Cleaning
Fruit and Vegetables had commas separating the base name and the type, but I wanted a separate column for fruit names, so I made one.
It made future plots immensely easier.

### Step 4: Data Manipulation
Among other things, I grouped by produce name to find the max price per cup, sorted in descending order. Then I filtered that to find the ten priciest fruits, and ten priciest vegetables, and finally merged the fruit and vegetable DataFrames to make a scatterplot, which leads me into...

### Step 5: Visualizations
In all visualizations Fruit is mostly purple and pink, and Vegetables are generally teal, blue, and green. This keeps things easy to read and tell apart across different visualizations.


### Step 6:


