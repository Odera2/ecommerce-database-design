# E-commerce Database Design

📦 A relational database schema for a modern e-commerce platform — built as a group assignment to demonstrate ERD planning, SQL implementation, and structured data modeling.



## 🧠 Project Objective

To design and implement a comprehensive e-commerce database using MySQL, incorporating entities like products, variations, categories, brands, images, and attributes. This includes:

- Entity-Relationship Diagram (ERD)
- SQL schema with 12 interrelated tables
- Structured and scalable relational design



## ERD
The following Entity-Relationship Diagram (ERD) illustrates the structure of the e-commerce database. It includes tables for products, variations, categories, brands, images, attributes, and more. All relationships and foreign key dependencies are visualized for clarity and normalization.

## ecommerce-erd.png
(Located in the /diagrams folder)

Legend:

Primary Keys are underlined.

Foreign Keys are connected with arrows.

All table relationships are normalized to avoid data redundancy.

Tables like color, size_option, and product_attribute handle product variations and custom details.


##  Data Flow Summary

This e-commerce database is designed to model how product data flows from general information to purchasable items:

1. **Products** are stored in the `product` table and linked to a `brand` and `product_category`.
2. Each `product` can have multiple **variations**, which are defined by combinations of `color` and `size_option` in the `product_variation` table.
3. Every unique combination of variation becomes a **purchasable item** (`product_item`) with its own price, SKU, and stock quantity.
4. **Product images** and **attributes** (like material or weight) are linked back to each `product` for richer content.

This structured approach ensures data consistency and scalability across multiple variations, colors, and sizes.

##  SQL Schema Overview

The database includes:
- Products and Categories
- Brands and Images
- Sizes and Colors
- Product Variations and Items (SKU-level)
- Product Attributes (material, weight, etc.)
- Fully normalized structure with referential integrity


## Contributors

This project was completed collaboratively by the following team members:

| First Name | Last Name     | Email Address                 |
|------------|---------------|-------------------------------|
| Stanly     | Odera         | oderas596@gmail.com           |
| John       | Gadiru        | johngadiru@gmail.com          |
| Michael    | Uke           | michealuke@rocketmail.com     |
| James      | Gitau         | jamesgitau092@gmail.com       |
| Adams      | Kiptalam      | adamskiptalam0@gmail.com      |
| Peter      | Oenga         | hel567kem@gmail.com           |
| Peter      | Verdict       | maundupeter28@gmail.com       |
| Johnson    | Akinyemi      | akinyemi2505@gmail.com        |
| Salome     | Kungu         | sallykijo@gmail.com           |
| Kevin      | Mokua         | kevinzmokua@gmail.com         |
| Capis      | Otieno        | capisokoth@gmail.com          |
| Anezwa     | Bangani       | anezwabangani3@gmail.com      |
| Leon       | Kariuki       | lkariuki749@gmail.com         |

##  How to Run

1. Open MySQL Workbench or your SQL client.
2. Run the script:
   ```sql
   source ecommerce.sql;


