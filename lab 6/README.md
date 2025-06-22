# Lab 6: Market Basket Analysis with Apriori and FP-Growth

Import note: I had to delete the order_products__prior.csv file from the repo because it breaks Github's 100MB file limit. If you wish to test the project, you will need to download the CSV from keggle yourself, which you can do from here: https://www.kaggle.com/datasets/psparks/instacart-market-basket-analysis

## Purpose
In this lab, I applied association rule mining using the Apriori and FP-Growth algorithms on the Instacart Market Basket dataset. 
The goal was to identify frequent itemsets, generate association rules, and visualize meaningful patterns that could inform product recommendations or marketing strategies.

## Insights

- The most frequently purchased items were fruits: bananas, organic strawberries, and bagged apples.
- Both Apriori and FP-Growth produced identical itemsets and rules when applied to the top 20 products with a 0.01 support threshold.
- The strongest rule found was "Organic Fuji Apple → Banana" with a support of ~2%, high confidence, and a lift > 1.3, indicating a solid association.
- FP-Growth was significantly faster than Apriori, especially as the dataset size increased.

## Challenges

- Running Apriori on the full dataset caused kernel crashes due to memory usage. To resolve this, I limited the analysis to the top 20 most frequently purchased products.
- Balancing support thresholds was tricky: too high filtered out everything, too low caused performance issues.
