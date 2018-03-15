# Get Leaderboard

Get a full list of all the players in the database and all their associated analytics, ordered by current ranking. 

**URL** : `/leaderboard`

**Method** : `GET`

<!-- **Auth required** : NO

**Permissions required** : None -->

## Success Response

**Code** : `200 OK`

**Content examples**

For a leaderboard where only two players exist in the system and one series has been played between them: 

```json
[
    {
        "Avg Points/Game": 5,
        "Avg Win Margin": 1,
        "Game Wins": 2,
        "Last Name": "Stiklickas",
        "Ranking": 1,
        "Game Losses": 1,
        "Shutouts": 0,
        "Series Win %": 100,
        "Game Win %": 66.67,
        "Series Wins": 1,
        "Points Scored": 15,
        "First Name": "Sara"
    },
    {
        "Avg Points/Game": 4,
        "Avg Win Margin": 0,
        "Game Wins": 1,
        "Last Name": "Lerner",
        "Ranking": 2,
        "Game Losses": 2,
        "Shutouts": 0,
        "Series Win %": 0,
        "Game Win %": 33.33,
        "Series Wins": 0,
        "Points Scored": 13,
        "First Name": "Daniel"
    }
]
```