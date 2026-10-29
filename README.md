# Web Programming Store Project

This repository contains a web application developed as part of the Web Programming course. The project is a small online store focused on managing customers and products, and it was built using PHP, HTML, CSS, and a simple layered architecture inspired by object-oriented web application design.

## Project Overview

The objective of this project is to provide a basic system for registering and listing customers and products in a web environment. It follows a structure that separates the application into:

- controller: handles the flow and coordination between user actions and business logic
- model: contains the domain classes, business rules, and database access logic
- view: contains pages displayed to the user and the styling files

This is an academic project intended to practice concepts such as MVC-style organization, form handling, database connectivity, and interface creation.

## Main Features

- Customer registration
- Customer listing
- Product registration
- Product listing
- Basic page navigation
- Use of stylesheets for layout and visual presentation
- Structured organization of classes and files to separate responsibilities

## Project Structure

The project is divided into three main folders:

- `controller`: contains the controllers responsible for customer and product operations.
  - `ClienteController.class.php`: manages actions related to customer registration and listing.
  - `ProdutoController.class.php`: manages actions related to product registration and listing.

- `model`: contains the data model, business logic, and database access classes.
  - `Cliente.class.php`: defines the customer entity.
  - `ClienteBusiness.class.php`: contains the business rules for customers.
  - `ClienteDAO.class.php`: handles persistence and retrieval of customer data.
  - `Produto.class.php`: defines the product entity.
  - `ProdutoBusiness.class.php`: contains the business rules for products.
  - `ProdutoDAO.class.php`: handles persistence and retrieval of product data.
  - `DBConnection.class.php`: establishes the connection with the database.

- `view`: contains the front-end pages and styles.
  - `index.html`: main landing page of the site.
  - `clientes/`: pages for customer registration and listing.
  - `produtos/`: pages for product registration and listing.
  - `css/`: style files used across the application.
    - `estilo.css`: main design stylesheet.
    - `menu.css`: menu styling.

## How the Application Works

The application follows a simple, organized flow:

1. The user interacts with a page in the `view` folder.
2. The controller receives the submitted data.
3. The controller creates an object from the model and sends it to the business layer.
4. The business layer validates and delegates the operation to the DAO layer.
5. The DAO communicates with the database through `DBConnection`.
6. The result is returned to the user through the page flow.

This separation of responsibilities helps keep the code easier to organize and maintain.

## How to Run It Locally

To run the project on your machine, follow these steps:

1. Clone the repository:

   ```bash
   git clone https://github.com/ana-athayde/php-web-store
   ```

2. Place the project in a local web server directory that supports PHP, such as XAMPP, WAMP, or a similar environment.

3. Make sure the database configuration in the project matches your local environment.

4. Open the project in a browser using your local server address.

5. Access the main page or the relevant customer/product screen to test the features.

## Notes

This project was developed as part of a course assignment and serves as a practical example of a small web system built with PHP and classic web technologies. It can be used as a base for learning and improving application organization, form processing, and database integration.

## Contributions

This is an academic project developed in collaboration with the instructor. Suggestions, improvements, and feedback are welcome.


