# DB-Assignment

## Answers

### 1)

The relationship between the "product" and "product_category" entities is a "one-to-many" relationship, indicated by the line connecting category_id in the "product" table to the id in the "product_category" table, with a "1" near the "roduct_category" table.

### 2)

Ensuring that each product has a valid category involves several steps:-

- Foreign Key Constraint: Implement a foreign key constraint in the "Product" table for the category_id column that references the id column of the "Product_Category" table. This constraint ensures that any category_id entered in the "Product" table must exist in the "Product_Category" table, thereby enforcing the validity of the category for each product.

- NOT NULL Constraint: Apply a NOT NULL constraint on the category_id column in the "Product" table. This ensures that every product inserted into the database must have a category id specified, preventing products from being categorized as 'undefined' or having no category.
