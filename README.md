# **PyMongo insertion of extracted data into MongoDB collection**

This repository contains Python code to extract the attributes of the top-8 most expensive Bored Apes from the Bored Ape Yacht Club NFT collection built on the Ethereum blockchain. The code uses Selenium to access the collection page, select all apes with "Solid gold" fur, and sort them from "Price high to low." The resulting detail pages for each of the top-8 most expensive apes are stored locally as html files.

The second part of the code parses each html file, extracts the attributes of each ape, and stores them as a document inside a MongoDB collection named "bayc."

## **Requirements**

The code requires the following libraries:

selenium  
pymongo  
bs4  
requests  

## **Usage**

1. Install the required libraries using pip install -r requirements.txt.  
2. Clone this repository.
3. In pymongo_insertion.py, update the working_direc variable with the path to your Chrome driver.
4. Run pymongo_insertion.py.
5. The program will access the Bored Ape Yacht Club collection page, select the top-8 most expensive apes with "Solid gold" fur, and sort them from "Price high to low." It will then save the detail pages for each ape as an html file.
6. The program will parse each html file, extract the ape's attributes, and store them as a document inside the "bayc" collection in a MongoDB database named "bayc."
Note: You will need to have a MongoDB server running on your machine for the code to work.
