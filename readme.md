# BoxStore Project

In this project I chose a data that has data from a box-store. This dataset has details about the products that the store sells, such as the manufacturer, the product name, model number of the product, serial number of the product, price of the item and more.

I took the following steps to complete the project. 
## Step 1: Data Storage:
* Then I used `MySql` database to store this data. MySql is a great option for this case as it gives me the ability to create the database on my local machine, and it offers great performance. 

## Step 2: Normalize the Data: `boxstore_normalize.xlsx`
* I used `MS Excel` to normalize the data. The data in its original format was just a single table that has all the information. This is not a good way to store data, as it makes the data more redundant and consumes alot of space. Instead I split this data into several smaller tables which will reduce repetition of data and makes the data more readable. This also gave me better performance. The data was split into the following tables:
    1. manufacturer (m)
    2. item (i)
    3. item_inventory (ii)
    4. item_type (it)
    5. item_price (ip)
    6. order_item (oi)
    7. orders (o)

## Step 3: Creating the data and inserting the data: `boxstore_build.sql`
* I used SQL to create the database and all tables in it. 

## Step 4: Creating more Data:
* I created more data in addition to  the original data. This would give me a more realistic scenario for creating my JOINs later. The following are the tables that I created:
    1. people (p)
    2. people_employee (pe)
    3. geo_address_type (gat)
    4. geo_country (gco)
    5. geo_region (grg)
    6. geo_towncity (gtc)
    7. tax (t)

## Step 5: Entity Relationship Diagram ERD: `boxstore_erd.drawio`
* An Entity Relationship Diagram (ERD) is a great way to understand the relationship between a dataset with several tables. I used `Draw.io` to create the ERD for this data. This diagram has all the tables that I had used in the project. 

![alt text](./image/erd.png)