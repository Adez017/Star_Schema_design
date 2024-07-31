# Star Schema Design for DVD Rental Database

## Project Overview
This project focuses on designing a star schema for the DVD rental sample database provided by PostgreSQL tutorials. The objective is to transform a normalized database structure into a star schema, which is commonly used in data warehousing and analytics for its simplicity and efficiency in querying.

## Star Schema Overview
A star schema is a type of database schema that consists of a central fact table surrounded by dimension tables. The fact table stores quantitative data (facts) about business processes, while the dimension tables store descriptive attributes (dimensions) related to these facts.

## Project Structure

### 1. Fact Table
- **FactRental**: This table stores transactional data about DVD rentals, including information like rental date, rental cost, and the associated customer and film.

### 2. Dimension Tables
- **DimCustomer**: Contains detailed information about customers, such as customer ID, name, address, and contact details.
- **DimFilm**: Stores details about the films available for rent, including film ID, title, genre, release year, and rating.
- **DimStore**: Holds data about the stores, such as store ID, location, and contact information.
- **DimDate**: A time dimension table that breaks down dates into day, month, quarter, and year, facilitating time-based analyses.

## Implementation Steps
1. **Extract Data**: Retrieve data from the DVD rental database's normalized tables.
2. **Transform Data**: Convert the extracted data into the star schema structure, ensuring that fact and dimension tables are properly defined and populated.
3. **Load Data**: Insert the transformed data into the star schema tables.

## Tools and Technologies
- **PostgreSQL**: The database management system used for storing and managing the data.
- **SQL**: Used for data extraction, transformation, and loading (ETL) processes.
- **Data Modeling Tools**: Used for designing and visualizing the star schema.
