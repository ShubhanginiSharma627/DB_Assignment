# DB_Assignment

### 1. Relationship between "Product" and "Product_Category" Entities

In the database schema, the "Product" and "Product_Category" entities share a one-to-many relationship. Specifically, each product is associated with a single category, while a category can encompass multiple products. This relationship is established through the utilization of a foreign key column named "category_id" in the "Product" table. This column references the primary key "id" in the "Product_Category" table, serving as a bridge between the two entities.

### 2. Ensuring Valid Category Assignment for Each Product

To maintain data integrity and enforce the rule that every product must belong to a valid category, a foreign key constraint is employed. The "category_id" column within the "Product" table is defined as a foreign key, referencing the "id" column in the "Product_Category" table. This mechanism guarantees that any attempt to insert a new product with a category ID not present in the "Product_Category" table will be rejected by the database management system. In essence, this ensures that each product in the "Product" table is associated with a valid category, preventing the introduction of inconsistent or erroneous data.
