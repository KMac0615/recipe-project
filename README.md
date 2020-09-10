# recipe-project

Development work on creating a python program that takes a recipe url, or manually input recipe, and calculates cost and nutrition per serving. This is my first idea and work on building a python project. I am hoping to eventually build it into a website using Flask.

## background

I am interested in tracking food costs and nutritional information for recipes that I make. However, I haven't found a resource that calculates both without personally documenting ingredients and how much they cost in an Excel spreadsheet. *Light Bulb* I have primarily used Python for data analysis and decided this would make a good project to gain different experience in Python.

## idea

- Input:
  - recipe url
    - return recipe into a 3-column dataframe [ingredient qty., qty. measurement, ingredient]
    - use food database API to pull in cost based on IP location [python package ipinfo]
  - manual recipe
    - will require ingredients, amounts, and measurements

## development

- [ ] url
  - [ ] build a program that can read in a recipe from provided url
    - [x] beautifulsoup and requests to scrape
    - [x] automate scraping ingredients regardless of url
      - tests: 
        - [ ] theleangreenbean.com
        - [ ] tasty.com
        - [ ] budgetbytes.com
        - [ ] recipes.com
        - [ ] thefoodnetwork.com
    - [ ] parse recipe ingredients into readable format
  - [ ] return ingredient nutritional information from food database api
  - [ ] return ingredient cost from food database api (instacart?)
  - [ ] aggregate nutritional and food cost info for entire recipe
  - [ ] calculate nutritional and food cost info per serving of recipe

- [ ] manual
  - [ ] recipe form
    - [ ] qty, unit, ingredient
    - [ ] ability to add additional ingredients
  - [ ] test db to store ingredients
    - [ ] tables
      - [ ] products
      - [ ] prices
      - [ ] locale
      - [ ] stores

## resources

- https://hackersandslackers.com/scraping-urls-with-beautifulsoup/
- https://hackingandslacking.com/scrape-structured-data-with-python-and-extruct-ee1305493307
- https://realpython.com/python-web-scraping-practical-introduction/
- https://towardsdatascience.com/how-to-web-scrape-with-python-in-4-minutes-bc49186a8460
- https://towardsdatascience.com/web-scraping-regular-expressions-and-data-visualization-doing-it-all-in-python-37a1aade7924
