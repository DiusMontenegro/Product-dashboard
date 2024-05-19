==================
Product Dashboard
==================

Product Dashboard is a web application built using CodeIgniter. This application allows users to register, log in, edit their profiles, and interact with products by creating and replying to reviews. The first user to register will be designated as the admin, who has additional privileges such as creating, updating, and deleting products.

Features
========

- **User Registration**: Users can create an account.
- **User Login**: Users can log into their accounts.
- **Edit User Profile**: Users can update their profile information.
- **Admin Privileges**: The first registered user is the admin and can manage products.
- **Product Management**:
  - Admin can create new products.
  - Admin can update existing products.
  - Admin can delete products.
- **Reviews**:
  - Users can create reviews for products.
  - Users can reply to existing reviews.
  - Users can view product information and reviews.
- **Form Validations**: All forms include robust validation to ensure data integrity.
- **MySQL Database**: User information is saved in a MySQL database.

Installation
============

To install and run the Product Dashboard, follow these steps:

1. **Clone the repository**:

   .. code-block:: bash

      git clone https://github.com/DreaUltimate/Product-dashboard.git

2. **Navigate to the project directory**:

   .. code-block:: bash

      cd product-dashboard

3. **Install dependencies**:
   
   - Ensure you have Composer installed. If not, download it from https://getcomposer.org/.
   - Run the following command to install CodeIgniter dependencies:

     .. code-block:: bash

        composer install

4. **Configure the application**:
   
   - Copy the `env` file to `.env` and configure your database settings.
   - Set your database configuration in `.env`:

     .. code-block:: ini

        database.default.hostname = localhost
        database.default.database = your_database_name
        database.default.username = your_database_username
        database.default.password = your_database_password
        database.default.DBDriver = MySQLi

   - Update the base URL and other configuration settings as needed in `app/Config/App.php`.

5. **Run the database migrations**:

   .. code-block:: bash

      php spark migrate

6. **Run the application**:

   .. code-block:: bash

      php spark serve

   The application will be available at `http://localhost:8080`.

Usage
=====

Once the application is up and running, you can start using it as follows:

1. **Register a new user**:
   - Visit the registration page and create a new account. The first user to register will automatically be given admin privileges.

2. **Log in**:
   - Use your credentials to log in to the application.

3. **Edit Profile**:
   - Navigate to your profile page to edit your user information.

4. **Manage Products (Admin only)**:
   - As an admin, you can create, update, and delete products from the product management section.

5. **Create and Reply to Reviews**:
   - View product details and submit reviews.
   - Reply to existing reviews to engage with other users.

Form Validations
================

All forms in the application are equipped with comprehensive validation to ensure data integrity and user-friendly error messages.

Contributing
============

Contributions are welcome! Please fork the repository and submit a pull request for review.

License
=======

This project is licensed under the MIT License. See the LICENSE file for details.
