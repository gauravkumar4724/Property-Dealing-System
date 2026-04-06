# Property Dealing System

## Overview
A web-based real estate property management system (PMS) that enables users to buy, sell, and manage residential and commercial properties (houses, shops, land) across multiple locations. The system features a three-tier architecture with public portal, customer portal, and admin panel.

## Features

### Customer Portal
- User registration and profile management
- Browse properties by location and category
- Post properties for sale with image uploads
- Search and filter properties
- View property details and contact owners
- Submit feedback

### Admin Panel
- Manage locations: States, Cities, Areas
- Manage property categories
- Monitor properties and customer registrations
- Publish news and announcements
- View reports (Customer, News, Property)
- Manage user access and feedback

### Public Features
- Cascading dropdowns for location selection (State → City → Area) via AJAX
- Dynamic property search
- Welcome page with Buy/Sale sections

## Technologies Used
- **Backend**: PHP 5.3, MySQL 5.5
- **Frontend**: HTML, CSS, jQuery, Spry Framework
- **Database**: MySQL with tables for states, cities, areas, categories, properties, images, customers, admins, feedback, and news

## Installation and Setup
1. Ensure you have a web server (e.g., Apache) and PHP/MySQL installed.
2. Import the `pms.sql` file into your MySQL database to set up the schema and sample data.
3. Update `config.php` with your database credentials.
4. Place the project files in your web server's root directory.
5. Access the application via your browser.

### Default Credentials
- **Admin**: Username: `admin`, Password: `admin`

## Database Schema
The system uses 10 core tables:
- `state_master`, `city_master`, `area_master`
- `category_master`, `property_master`, `property_image`
- `customer_reg`, `login_master`, `feedback`, `news_master`

## Notes
- This is a legacy system using deprecated MySQL functions; consider modernizing with PDO or mysqli.
- Security improvements recommended: password hashing, SQL injection prevention.
- Sample data includes properties in Gujarat and other states.

## Usage
- Register as a customer to post/view properties.
- Admins can manage all aspects via the Admin panel.
- Use the search functionality to find properties by location and type.