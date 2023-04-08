# Introduction to Riot API

A quick introduction to Riot API using the different tutorials available on web.
This tutorial was made with Python using Jupyter Notebook. 

Requirements:

- **Python environment**: Jupyter Notebook, Google Collab...
- [API key](https://developer.riotgames.com/): You have to register with your LoL account (Don't share it!)
- [ RiotWatcher](https://riot-watcher.readthedocs.io/en/latest/#) A thin wrapper on top of the [Riot Games API for League of Legends](https://developer.riotgames.com/apis)
- [Pandas package](https://pypi.org/project/pandas/)  


Main code can be found on the [Introduction-to-Riot-API.ipynb](https://github.com/Vannayumyum/league-of-legends/blob/main/Introduction-to-Riot-API.ipyn) file.  
[tutorial-web-scrapping.ipynb](https://github.com/Vannayumyum/league-of-legends/blob/main/tutorial-web-scrapping.ipynb) shows how to scrap informations from a website.

## Objectives

The first objective is to manipulate some basic data from the Riot API like loading a player's profile and analyzing his last games or create game's summary like u.gg and op.gg . 

For further works we will focus on champions played at high elo to have a better understanding of the meta.
What are the most played champions in Challenger ? Which champs have the highest winrate ? Which champ is picked to counter such champ ?
We will obviously focus on pro players as they probably have the best understanding at the game.
As Riot Games API doesn't provide us a way to get rankings of the best players, we will need to scrap informations from websites that display ranked ladders. This will be done pretty soon. 

## What has been done ( 09/04/2023)

- Basic functions using riot API such as: Summoner's profile info, game details and game resume, champions played...
- Web scrapping op.gg euw challengers ladder to get information about the first 100 top players.
- Champions played by the top 20 Challengers in their last 10 games. Gives an idea of the meta trend.
> **Note:** The request rate limit can slow your work. With a personnal key, you can get 20 requests every 1 second or 100 requests every 2 minutes. When we exceed this limit, an automatic time.sleep is called so you don't need to interrupt your run.

## What to do next
- Implements a function for the ban rates and pick rates
- Meta trending: Implements a function that counts the number of Challenger players that played a champ over an amount of game. If a champ was played a lot and only by a few of players => OTP? 
	>Ex: In the last 179 games of the first 20 Challengers , Riven appeared 24 times and she is the 13th most picked champ while she is not in the meta. could be explained by OTPs 
- Pick games with a deadline or within the same lol patch.
- Study champ pick order to get a better understanding at counter pick

