# Documentation

## Corpus
The corpus chosen for this assignment comes from a website made specifcially for webscraping, for those who want to practice and learn web scraping. The website's name is "Books to Scrape" which includes prices and ratings that were randomly assigned and have no real meaning. 
I only focused on the Horror genre, which includes 17 books. The books displayed are real publications by real authors such as Stephen King and dacre Stocker, however everything else is made up for practice purposes. 

## Scraped data
1. Product description of each book &rarr; This section was a bit challenging because the header for "Product description" <"div", id = "product_description"> is separate from the "paragraph" including the actual content of the descriptions, therefore i used ".find_next_sibling("p")".
2. Price of the book (made up) &rarr; taken from <"p", class_ = "price_color"> html tag
3. Availability &rarr; taken from <"p", class_ = "instock availability"> html tag
4. Rating &rarr; rating was originally in text form (e.g. "One", "Two") which was extracted from <"p", class_="star-rating"> html tag. It was then converted to numbers from 1 to 5

## Cleaning text
No cleaning of the data or text has been donw for this assignment 

## Terms and Conditions
I chose books.toscrape.com because as the first warning that pops up says: "This is a demo website for web scraping purposes. Prices and ratings here were randomly assigned and have no real meaning." This meant that there were no robots.txt or terms and condiions that I needed to look out for. 

## The scraped_data_A3.csv format
| Column | Description|
|----------|----------|
| TITLE    | title of the book  |
| AUTHOR    | name of the author of the novel  |
| GENRE    | type of literary genre  |
| URL    | url of the scraped page  |
| Description    | product description  |
| Price    | "price" of the novel  |
| Avalability    | amount of books "available"  |
| Rating    | "rating" of the book out of 5 stars  |
