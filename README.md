# Grocery-Retail-Perdiction

# Introduction
The aim of project is to build a model that accurately forecasts product sales. The model ensures there are just enough products in store at the right time.

## Data specifications:

### Item dataset:
1.  No of items (item_nbr): 4100
2.  No classes: 337
3.  No of families: 33
4.  No of unique class+family : 337


### Store dataset:
1. No of stores: 54
2. No of city: 22
3. No of state: 16
4. No of unique state + city : 22
5. No of store type: 5

From 33 families, only 9 of them have float value in unit sales.

From 337 classes only 35 of them have float value in unit sales.

## Pareto Analysis:
From 337 classes only 70 of them make 80% of total sold items. → Pareto analysis: almost 20% (67.4) of classes make 80% of total sales.

From 33 classes only 6 of them make 83% of total sold items. → Pareto analysis: almost 20% (6.6) of classes make 80% of total sales.

From 4100 items only 1624 of them contribute in 80% of total unit sales .


## Data Transformation:

state → remove (to reduce dimensionality)

year → remove 

class → MinMax scale (normalise) 

store_nbr → MinMax scale (normalise)

weekday → MinMax scale (normalise)

cluster → MinMax scale (normalise)


dcoilwtico → standard scaler

item_nbr → standard scaler


onpromotion → leave the same

holiday → leave the same


month → sin, cos

day → sin, cos

others → one-hot encoding
