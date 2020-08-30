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

- start small
  - [ ] build a program that can read in a recipe from provided url
  - [ ] return ingredient nutritional information from food database api
  - [ ] return ingredient cost from food database api (instacart?)
  - [ ] aggregate nutritional and food cost info for entire recipe
  - [ ] calculate nutritional and food cost info per serving of recipe