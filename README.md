# ignis-tech-solutions-webscrap

BOT to scrap this website https://www.supremenewyork.com/

# Overview

This is a scraper built in Python using Beautiful Soup and Requests to scrape the supreme clothing website and automatically purhcase items in less than 3 seconds based on inputted keywords.

This allowed a user to purchase items for the inital price every Thursday morning when new items were released before they were sold out. Many items sold out with in 10 seconds.

# How this Works

In the file # SupremeMain.py,
I've created a list of products I would like to attempt to purhcase. The list contains products of the class product, which is defined in # productClass.py.
The bot will iterate through the list in order of priority and search for the product by the name and keywords entered. It will be able to match substrings of the product if you do not know the entire name. You can input any number of sizes and colors and it will select the first available one, again in priority by the order in the list. If you set the parameter any_color to True, if the bot is not able to find the desired colors you have denoted, it will select the first one it finds

SupremeFunctions.py: Functions to purchase the product and fill billing information
getLink.py: Functions to retrieve the link of the product
productClass.py: Class of the Product object, as well as the Card object, and Buyer object
SupremeMain.py: Purchases product
