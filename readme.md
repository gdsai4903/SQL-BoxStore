# BoxStore Project

In this project I chose a data that has data from a box-store. This dataset has details about the products that the store sells, such as the manufacturer, the product name, model number of the product, serial number of the product, price of the item and more.

I took the following steps to complete the project. 
## Step 1: Data Storage:
* Then I used `MySql` database to store this data. MySql is a great option for this case as it gives me the ability to create the database on my local machine, and it offers great performance. 

## Step 2: Normalize the Data: `boxstore_normalize.xlsx`
* I used `MS Excel` to normalize the data. The data in its original format was just a single table that has all the information. This is not a good way to store data, as it makes the data more redundant and consumes alot of space. Instead I split this data into several smaller tables which will reduce repetition of data and makes the data more readable. This also gave me better performance. The data was split into the following tables:
    1. manufacturer (m)
    1. item (i)
    1. item_inventory (ii)
    1. item_type (it)
    1. item_price (ip)
    1. order_item (oi)
    1. orders (o)

## Step 3: Creating database and inserting data: `boxstore_build.sql`
* I used SQL to create the database and all tables in it. 

## Step 4: Creating more Data:
* I created more data in addition to  the original data. This would give me a more realistic scenario for creating my JOINs later. The following are the tables that I created:
    1. geo_address_type (gat)
    1. geo_country (gco)
    1. geo_region (grg)
    1. geo_towncity (gtc)
    1. people (p)
    1. people_employee (pe)
    1. tax (t)

## Step 5: Entity Relationship Diagram ERD: `boxstore_erd.drawio`
* An Entity Relationship Diagram (ERD) is a great way to understand the relationship between a dataset with several tables. I used `Draw.io` to create the ERD for this data. This diagram has all the tables that I had used in the project. 

![alt text](./image/erd.png)

# BoxStore Project

This project involves working with data from a box store, including details about the products sold, such as the manufacturer, product name, model number, serial number, and price. The project encompasses data storage, normalization, database creation, data expansion, and visualization using an Entity Relationship Diagram (ERD).

## Table of Contents
- [Project Description](#project-description)
- [Step 1: Data Storage](#step-1-data-storage)
- [Step 2: Normalize the Data](#step-2-normalize-the-data)
- [Step 3: Creating Database and Inserting Data](#step-3-creating-database-and-inserting-data)
- [Step 4: Creating More Data](#step-4-creating-more-data)
- [Step 5: Entity Relationship Diagram (ERD)](#step-5-entity-relationship-diagram-erd)
- [Installation](#installation)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Project Description
The BoxStore project involves handling a dataset from a box store. The dataset includes comprehensive details about the products. The goal of the project is to efficiently store, normalize, and manage the data in a MySQL database, create additional realistic data, and visualize the relationships using an ERD.

## Step 1: Data Storage
I used `MySQL` to store the data. MySQL is a suitable choice due to its performance and the ability to run a local database instance. It enables efficient data handling and storage.

## Step 2: Normalize the Data
The data was normalized using `MS Excel`. Initially, the data was in a single table, which led to redundancy and inefficiency. The data was split into several smaller, normalized tables to improve performance and readability.

The following tables were created:
1. `manufacturer (m)`
2. `item (i)`
3. `item_inventory (ii)`
4. `item_type (it)`
5. `item_price (ip)`
6. `order_item (oi)`
7. `orders (o)`

The normalized data is saved in the file `boxstore_normalize.xlsx`.

## Step 3: Creating Database and Inserting Data
The database and all necessary tables were created using SQL scripts. The script for this step is in the file `boxstore_build.sql`.

## Step 4: Creating More Data
Additional data was created to simulate a more realistic scenario and facilitate JOIN operations later. The additional tables created include:
1. `geo_address_type (gat)`
2. `geo_country (gco)`
3. `geo_region (grg)`
4. `geo_towncity (gtc)`
5. `people (p)`
6. `people_employee (pe)`
7. `tax (t)`

## Step 5: Entity Relationship Diagram (ERD)
An ERD is a valuable tool for visualizing the relationships between the tables in the dataset. The ERD for this project was created using `Draw.io` and is available in the file `boxstore_erd.drawio`.

![Entity Relationship Diagram](./image/erd.png)

## Installation
To set up the project locally, follow these steps:

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/boxstore-project.git
   cd boxstore-project
