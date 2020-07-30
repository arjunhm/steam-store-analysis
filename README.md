# About the project
Steam is a video game digital distribution service by Valve.  
With over 20 million users, its the largest platform where games can be bought and linked to the user's account.
In this project, we scrape data from the [Steam store](https://store.steampowered.com/) and analyze the data.


# Data Collection
Scraped the data from the [Steam store](https://store.steampowered.com/) using Python and BeautifulSoup.

Collected information such as
- Title
- Developer & Publisher
- Release Date
- Price
- Genre
- Related tags
- Game description
- Minimum System Requirements
- Recommended System Requirements
- Game Rating

# Analysis

## Data Preparation

A lot of effort was put into preparing the data which included tasks such as 
- Dropping duplicate data
- Dropping games with very few reviews
- Dropping games which were Demos or DLCs (Downloadable Content, an expansion to a base game)
- Converting data types (prices of games from string to float)
- Collecting unique tags for all games
- Converting release date to datetime object
- Converting tags from string to list
- Label Encoding game ratings. (Overwhelmingly Negative - 0 to Overwhelmingly Positive - 8)
- Add a score column based on the rating and the vote count

## Data Analysis/Visualization
- Top games of all time
- Most popular games based on genre/tag
- Price of popular games over the years
- Popularity of genres over the years (Based on rating/games released)
- Pie Chart of distribution of genres

# Future work
- [ ] Filter games based on System requirements
- [ ] Create a web app for easier access
- [ ] More visualizations 

