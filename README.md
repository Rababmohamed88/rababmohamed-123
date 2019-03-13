# Item Catalog Project
An Udacity Full Stack Web Developer 2 Nanodegree project.

This application provides a list of items within a variety of categories 
as well as provide a user registration and authentication system.
Registered users will have the ability to add, edit, and delete their own items.

## Steps to run this project

1. Download and install [Vagrant]
2. Download and install [VirtualBox]
3. Open terminal, and type
   ```bash
   vagrant up
   ```after navigating to vagrant
4. then type in terminal,
   ```bash
   vagrant ssh
   ```
5. Type `cd /vagrant/` to navigate to the shared repository.
6. Install or upgrade Flask:
    ```bash
    sudo python -m pip install --upgrade flask   
	```
7. Run the following command to set up the database:
    ```bash
    python database_setup.py
    ```
8. Run the following command to insert dummy values. 
    ```bash
    python populate_database.py
    ```
9. Run this application:
    ```bash
    python app.py
    ```
10. Open `http://localhost:5000/` in your favourite Web browser.

## The following are available to public:

Catalog JSON:`/api/v1/catalog.json`
-Display all items in the catalog.

Catalog item JSON:`/api/v1/categories/<int:category_id>/item/<int:item_id>/JSON`
-Display a particular item in the catalog.

Categories JSON:`/api/v1/categories/JSON`
-all the categories in the catalog.
