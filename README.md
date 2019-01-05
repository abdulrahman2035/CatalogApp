# Catalog App Project

#Project description 
Is a web application provides a list of items within a variety of categories as well as integrates third party user registration and authentication
and allow registered users to add,edit and delete their own items and catigories.

# Prerequisites to run the project:
   1. install Python3.7.1.
   2. install VirtualBox.
   3. install Vagrant.
   4. download a FSND virtual machine from: https://github.com/udacity/fullstack-nanodegree-vm.
   5.Install Flask to your machine by using this command: sudo python3 -m pip install --upgrade flask
   6.Install sqlalchemy to your machine by using this command: sudo python3 -m pip install --upgrade sqlalchemy
   7.Install oauth2client to your machine by using this command: sudo python3 -m pip install --upgrade oauth2client
   8.set up the database to your machine by using this command: python3 database_setup.py
   9.populate test data to the database by using this command: python3 seeder.py
   
# To run the project 
1.launch the Virtual Machine inside FSND virtual machine directory using command (vagrant up).
2.change directory to .vagrant using command (cd .vagrant).
3.copy the project directory into vagrant machine using command (scp -P 2222 -r ../CatalogApp vagrant@127.0.0.1:~/.).
4.log in into vagrant machine using command (vagrant ssh).
5.go inside project directory using command (cd CatalogApp).
6. Enter into item directory and run app.py (python3 app.py).

#API (JSON) Endpoints
1-Return JSON of all items inside the catalog
  example('/api/v1/catalog.json').
  
2-Return JSON of specific item 
  example ('/api/v1/categories/<int:category_id>/item/<int:item_id>/JSON')
  
3-Return JSON of all categories 
  example ('/api/v1/categories/JSON')
  
4-Return JSON of a particular category in the catalog 
  example ('/api/v1/categories/<int:category_id>/item/JSON')






