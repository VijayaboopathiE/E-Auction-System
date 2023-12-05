# E-Auction System (PHP)

## Overview

The E-Auction System (PHP) is an online platform designed for conducting electronic auctions. It provides a user-friendly interface for both auctioneers and participants to engage in transparent and efficient bidding processes.

## Features

- User Registration and Authentication
- Auction Creation and Management
- Item Listing with Descriptions
- Bidding Mechanism
- Real-time Updates
- Winner Declaration
- Payment Integration
- Admin Dashboard for Monitoring

## Installation
    
### Prerequisites

- [PHP](https://www.php.net/) installed
- [MySQL](https://www.mysql.com/) or [MariaDB](https://mariadb.org/) installed and running
- [Composer](https://getcomposer.org/) installed

### Steps

1. Clone the repository:

   ```bash
   git clone https://github.com/VijayaboopathiE/E-Auction-System-php.git
   
2. Navigate to the Project Directory
   
   cd E-Auction-System-php

3. Install Dependencies

   composer install

4. Set Up the Database

* Create a MySQL/MariaDB database for the application.
* Import the database schema from database/schema.sql. You can use a tool like MySQL command line, phpMyAdmin, or any other MySQL client for this.
* mysql -u your_username -p your_database_name < database/schema.sql
  

Certainly! Below is a more detailed installation guide for a PHP-based E-Auction System using MySQL/MariaDB as the database.

Installation Steps:
1. Clone the Repository
bash
Copy code
git clone https://github.com/yourusername/e-auction-system-php.git
2. Navigate to the Project Directory
bash
Copy code
cd e-auction-system-php
3. Install Dependencies
bash
Copy code
composer install
4. Set Up the Database
   
Create a MySQL/MariaDB database for the application.
Import the database schema from database/schema.sql. You can use a tool like MySQL command line, phpMyAdmin, or any other MySQL client for this.
bash
Copy code
mysql -u your_username -p your_database_name < database/schema.sql

5. Configure Database Connection
   
Update the database configuration in config/database.php with your database credentials:
    return [
    'driver'   => 'mysql',
    'host'     => 'localhost',
    'database' => 'your_database_name',
    'username' => 'your_username',
    'password' => 'your_password',
    // ...
];

6. Set Up Environment Variables
   
Create a .env file in the root directory and configure it with the necessary variables. You can use the provided .env.example as a template.
APP_ENV=development
APP_KEY=your_app_key

DB_CONNECTION=mysql
DB_HOST=localhost
DB_DATABASE=your_database_name
DB_USERNAME=your_username
DB_PASSWORD=your_password

7. Run the Application

   php -S localhost:8000 -t public

8. Access the Application
   
Open your web browser and navigate to http://localhost:8000. You should see the E-Auction System interface.   

9. Register an Account and Start Using the System
   
* Register an account or log in if you already have one.
* As an auctioneer, create a new auction and add items for bidding.
* As a participant, browse ongoing auctions, place bids, and monitor auctions in real-time.

## Usage
1.Access the application through your web browser.

2.Register an account or log in if you already have one.

3.As an auctioneer, create a new auction and add items for bidding.

4.As a participant, browse ongoing auctions, place bids, and monitor auctions in real-time.

5.Auctioneer can declare winners and proceed with the payment process.
