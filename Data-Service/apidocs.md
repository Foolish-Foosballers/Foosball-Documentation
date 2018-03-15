# Foosball-Data-Service

Microservice that will interface with our PostgreSQL database containing information about players and games.

## API Documentation

We provide a number of routes to our PostgreSQL database hosted on Heroku. They are organized below by which table they query in the database. For a full overview of our database schema, click [here](schema.md).

### Players

Routes that query the Players table in our database:

* [getPlayers](api/getPlayers.md) : `GET /players`
* [createPlayer](api/createPlayer.md) : `POST /players`
* [getPlayerById](api/api/getPlayerById.md) : `GET /players/<id>`
* [updatePlayer](api/updatePlayer.md) : `PUT /players/<id>`
* [removePlayerById](api/removePlayerById) : `DELETE /players/<id>`
* [getPlayerByUsername](api/getPlayerByUsername.md) : `GET /players/user/<username>`
* [getRankings](api/getRankings.md) : `GET /rankings`
* [updateRankings](api/updateRankings.md) : `PUT /rankings`
* [getLeaderboard](api/getLeaderboard.md) : `GET /leaderboard`

### Games

Routes that query the Games table in our database: 
* [getGames](api/getGames.md) : `GET /games`
* [createGame](api/createGame.md) : `POST /games`
* [getGameById](api/getGameById.md) : `GET /games/<id>`
* [removeGameById](api/removeGameById.md) : `DELETE /games/<id>`

### Series

Routes that query the Series table in our database: 
* [getSeries](api/getSeries.md) : `GET /series`
* [createSeries](api/createSeries.md) : `POST /series`
* [removeSeriesById](api/removeSeriesById.md) : `DELETE /series/<id>`

### History

Routes that query the History table in our database: 
* [getHistory](api/getHistory.md) : `GET /history`
* [createHistory](api/createHistory.md) : `POST /history`

