# Template
# 2021 December 29

## Question
Suppose you are given a SQL table containing the brands of shoes (field name: brand) as well as the shoe price (field name: price). The database is called shoe_info. You are tasked with updating the prices in this database for a few brands of shoes. Specifically, you have been asked to update all Nike shoe prices to $100, and all Adidas shoe prices to $85. Using SQL, write a query to perform this action.

## Solution
We will have 2 queries, one for Nike branded shoes, and the other for Adidas branded shoes.

### Adidas Query
```
UPDATE shoe_info
SET price = 85
WHERE brand = adidas;
```

### Nike Query
```
UPDATE shoe_info
SET price = 100
WHERE brand = nike;
```