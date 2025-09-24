# Auto sniper

## Description

A program that looks at multiple car selling websites to search for specific cars and builds.
The program uses a single search query to search multiple websites in multiple countries.
The program collects the cars from the websites and presents it to the user.

## Goal

The program has to scrape car search result data from all given websites, and combine the data into a presentable form to the user.
The challenge is to have a specific interface that creates the search URL for each website.
Depending on the complexity, either the HTML result has to be returned, or the list of cars can be scraped from the result page and transformed into a custom format.

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

## Prompt

1. First, we want to get advice on the proper framework to use. A website is the goal, what kind of framework should we use?
2. As in initial goal, we want a list of the search queries for the websites so we can with a single press on a button search on the given websites and open the result page
3. How do we proceed with fitting the search prompts for all websites? Should I use the developer console to get info on the search URL?
4. Perhaps we should start with a single website first: www.autoscout24.nl