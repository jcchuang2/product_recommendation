# Online Store Sale Improvement with Relational and Graph Data Analysis

Team Members: Joshua Chuang, Joyce Hu, Zijie Feng

Presentation: [Recording](https://drive.google.com/file/d/1kbVcB59W6N5vQX86bweIFm1WyUkZXM20/view?usp=sharing)

Report: [Link](link)

## Summary
Using relational and graph data methods, we aim to improve online store sales through enhanced product recommendation. We used Amazon sales data and performed data analysis, such as finding the top rated items, sales per category, trends in product prices, and upselling items. For product recommendation, we looked at a collaborative filtering model, a personalized pagerank model, and lastly, a hybrid model, combining the two previous models. These methods were able to successfully capture item popularity and personalized recommendations, which will ultimately lead to improvement in sales.

## Data
The original data source can be found on [Kaggle](https://www.kaggle.com/datasets/karkavelrajaj/amazon-sales-dataset?resource=download).

The project datasets can be found in `data/`, where `transactions_brand(products).csv`, `transactions_brand(ratings).csv`, and `transactions_brand(users).csv` correspond to the Products, Ratings, and Users tables. These datasets will be used in creating the relational and graph databases.


`transactions_brand(products).csv`
* product_id - Product ID
* product_name - Name of the Product
* category - Category of the Product
* brand - Brand of the Product
* release_date - Date that the Product was posted

`transactions_brand(ratings).csv`
* user_id - User ID
* product_id - Product ID
* rating - Rating of the Product

`transactions_brand(users).csv`
* user_id - User ID

## Instructions

### Relational Database
Use `relational_db.sql` and `prod_rec_demo.sql`

### Graph Database
1. Create project in Neo4j Desktop.
2. Add DBMS and add `transactions_brand(products).csv`, `transactions_brand(ratings).csv`, and `transactions_brand(users).csv` to the project import folder.
3. Start the DBMS and open Neo4j Browser.
4. In the browser, commands and queries found in `collaborative_filtering.cypher` and `pagerank.cypher`.
