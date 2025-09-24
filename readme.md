# Auto sniper

## Description

A program that looks at multiple car selling websites to search for specific cars and builds.
The program uses a single search query to search multiple websites in multiple countries.
The program collects the cars from the websites and presents it to the user.

## Goal

We want to create a website that searches a list of car selling websites all at the same time and returns the results to the user.
The program has to scrape car search result data from all given websites, and combine the data into a presentable form to the user.

## Search filters and details

| Manufacturer  | Models      | Years     | Distance driven (KM) |
|---------------|-------------|-----------|----------------------|
| BMW           | All         | 1975-2000 | <70,000              |
| Mercedes-Benz | All         | 1980-1996 | <70,000              |
| Mercedes-Benz | E500 / 500E | 1990-1996 | <120,000             |
| Ferrari       | All         | 1994-2001 |                      |
| Alpina        | 1900-2010   |           |                      |
| BMW           | M3 / M5     | 1980-2010 | <120,000             |
| Porsche       | 911 Turbo   | 1980-1997 |                      |
| Porsche       | 911 Turbo   | 1980-1997 | <100,000             |
| Audi          | RS4         | 2000-2001 | <150,000             |
| Mercedes-Benz | AMG         | 1995-2009 | <120,000             |

## Websites

| Country     | Website              | Priority |
|-------------|----------------------|----------|
| Netherlands | www.marktplaats.nl   | Low      |
| Germany     | www.kleinanzeigen.de | High     |
| Sweden      | www.blocket.se       | High     |
| Norway      | www.finn.nl          | Low      |
| France      | www.lebencoin.fr     | High     |
| Italy       | www.subito.it        | High     |
| Spain       | www.milanuncios.com  | High     |
| Portugal    | www.olx.pt           |          |
| Austria     | www.willhaben.at     | Low      |
|             | www.autoscout24.nl   |          |
|             | www.mobile.de        |          |

## Instructions

1. First, we want to get advice on the proper framework to use. A website is the goal, what kind of framework should we use that can handle this and also have a nice user interface?
2. We will start with a single website first: www.autoscout24.nl
3. My best guess is that to do this, we need URL create instructions for the listed websites, and than a way to manipulate these URL's to handle the search queries
4. So first we create the app/website, the framework, after that we will handle the websites one by one to add URL create methods
5. Initially we will just open all the results in new browser tabs to show the user the results for all websites
6. Later, we want to incorporate a method that scrapes the results from the search results to create a custom presentation format
7. On the websites, the search filters have to be selectable and customizable
