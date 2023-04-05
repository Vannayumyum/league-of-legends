# Introduction to Riot API

A quick introduction to Riot API using the different tutorials available on web.
This tutorial was made with Python using Jupyter Notebook. 

Requirements:

- **Python environment**: Jupyter Notebook, Google Collab...
- **API key**: https://developer.riotgames.com/  (Don't share it)
- [ RiotWatcher](https://riot-watcher.readthedocs.io/en/latest/#) A thin wrapper on top of the [Riot Games API for League of Legends](https://developer.riotgames.com/apis)
- [Pandas package](https://pypi.org/project/pandas/)


# Objectives

The first objective is to manipulate some basic data from the Riot API like loading a player's profile and analyzing his last games or create game's summary like u.gg and op.gg . 

For further works we will focus on champions played at high elo to have a better understanding of the meta.
What are the most played champions in Challenger ? Which champs have the highest winrate ? Which champ is picked to counter such champ ?
We will obviously focus on pro players as they probably have the best understanding at the game.
As Riot Games API doesn't provide us a way to get rankings of the best players, we will need to scrap informations from websites that display ranked ladders. This will be done pretty soon. 
