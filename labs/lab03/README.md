# Lab 03: Practice SOLID Principles

Build a product/ordering system API in Python (using Flask, FastAPI, or Django). Include the following models within that API:

## Product Structure

- Internal ID (auto-increment)
- Product number (e.g., "ABC-123")
- Product description
- Unit cost

## Order Structure

- Internal ID (auto-increment)
- Product ID (foreign key)
- Order number (e.g., "12345")
- Quantity
- Total

## Operations to Include

* List all products in the catalog
* List a specific product in the catalog by product number
* Accept a new order for a single product
* Retrieve a specific order's details by order number

Use a database of your choice (SQLite, PostgreSQL, etc.) for persisting your catalog and order information. Feel free to preload the catalog with a set of products. If you are not comfortable working with a database, you can use in-memory data structures instead (but know that when the process running your API stops, you will lose your data).

The key focus of this lab is to practice the SOLID principles - i.e., build the components of your API in a loosely-coupled manner, layer components in modules correctly, etc. such that the components of your API are clean and well architected. For example, whatever storage/persistence strategy you use, the rest of the API should not need to know or care. Ensure that functionality is sufficiently isolated to modules and that each module is insulated from the others (to prevent brittle coupling).
