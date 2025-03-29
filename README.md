# HW5 - Getting Started with SQL

## Authors:
- Tejesh Annavarapu
- Srujan Katukam
- Anumandla Muralidhar Reddy
- Ajaykumar Reddy Rachala

## Instructor:
- Thomas Gyeera

## Database Design Overview:
This project involves creating and managing a **Customer Shopping Database** that tracks customer purchases and product information. The database is designed to store data about customers, products, and their transactions, with a focus on normalization and efficient querying.

### Key Entities:
1. **Customers**: Stores demographic information about each customer (e.g., name, email, join date).
2. **Products**: Contains details about products available for purchase (e.g., name, price, category).
3. **Purchases**: Tracks transactional data, linking customers to products they purchase, including quantities, total amounts, and payment information.

### Relationships:
- **Customer-to-Purchase**: One-to-many relationship (A customer can make multiple purchases).
- **Product-to-Purchase**: One-to-many relationship (A product can appear in multiple purchases).

### Entity Attributes:
- **Customers**: 
    - `customer_id`
    - `age`
    - `gender`
    - `location`
  
- **Products**:
    - `product_id`
    - `item_name`
    - `category`
    - `size`
    - `color`
    - `season`
  
- **Purchases**:
    - `purchase_id`
    - `customer_id`
    - `product_id`
    - `purchase_amount`
    - `payment_method`
    - `shipping_type`
    - `discount_applied`
    - `promo_code_used`
    - `subscription_status`
    - `previous_purchases`
    - `purchase_frequency`

## Database Design Rationale:
- **Normalization**: The schema separates customer, product, and purchase data to minimize redundancy.
- **Efficient Querying**: Relationships between tables via foreign keys enable fast, structured data retrieval.
- **Behavioral Analysis**: The design supports analysis of customer shopping patterns, product popularity, and sales trends.

## Diagrams:
1. **Entity-Relationship Diagram (Chen Notation)**: Visual representation of entities and their relationships.
2. **Crow’s Foot Diagram**: Highlights the entities, attributes, and cardinality of the relationships.

## SQL Schema Creation:
SQL scripts are provided to create the tables for the Customer Shopping Database, along with sample data insertion for testing the schema.

## Sample Data:
The assignment includes inserting 15 records into the database to simulate actual shopping behavior and test the queries.
