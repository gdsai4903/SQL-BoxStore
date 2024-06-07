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
   git clone https://github.com/gdsai4903/SQL-BoxStore
   cd SQL-BoxStore
