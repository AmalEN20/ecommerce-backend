<!-- omit in toc -->
# E-Commerce Back End

<!-- omit in toc -->
## Description

This is the back end application for an e-commerce website using Express, MySQL, Sequelize and dotenv. By creating an environment variable file with database name, MySQL username, and MySQL password, user can connect to a database using Sequelize. When the application is invoked, the server is started and the Sequelize models for categories, products, and tags are synced to the MySQL database. User can create, read, update, and delete data in the database by testing API POST, GET, PUT, DELETE routes in Insomnia.

<!-- omit in toc -->
## Table of Contents
- [Installation](#installation)
- [Usage](#usage)
- [License](#license)

## Installation
- Install Node.js v16 and npm
- Install MySQL Server
- Install Insomnia
- Install npm packages:
  ```
  npm install
  ```

## Usage
1. Change the name of `.env.EXAMPLE` file to `.env`
2. Enter your MySQL username and MySQL password in the `.env` file:
    ```yaml
    DB_NAME='ecommerce_db'
    DB_USER='<your_mysql_username>'
    DB_PASSWORD='<your_mysql_password>'
    ```
3. Create and select your database with MySQL shell commands:
    ```
    mysql -u root -p
    ```
    ```shell
    mysql> source db/schema.sql;
    mysql> quit;
    ```
4. Seed the test data to your database:
    ```
    npm run seed
    ```
5. Execute the app and run the server:
    ```
    npm start
    ```
6. Use Insomnia to test API POST, GET, PUT, DELETE routes.
- Walkthrough video
<video src=" "></video>
