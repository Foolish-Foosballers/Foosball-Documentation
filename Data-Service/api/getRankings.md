# Get Rankings

Get a full list of all the players in the database and all their associated information, ordered by player ranking.

**URL** : `/rankings`

**Method** : `GET`

<!-- **Auth required** : NO

**Permissions required** : None -->

## Success Response

**Code** : `200 OK`

**Content examples**

For a list of ranked players where there are only two users registered in the system, and only one series has been played between them:

```json
[
    {
        "Username": "212123456",
        "Shutouts": 0,
        "TotalGamesPlayed": 3,
        "Ranking": 1,
        "SeriesWins": 1,
        "GameWins": 2,
        "TotalPoints": 15,
        "SignupDate": "2018-01-05T15:04:32.825103",
        "Email": "sara.stiklickas@example.com",
        "Id": 1,
        "TotalTimePlayed": 900,
        "LastName": "Stiklickas",
        "FirstName": "Sara"
    },
    {
        "Username": "212123457",
        "Shutouts": 0,
        "TotalGamesPlayed": 3,
        "Ranking": 2,
        "SeriesWins": 0,
        "GameWins": 1,
        "TotalPoints": 13,
        "SignupDate": "2018-01-05T15:26:16.417546",
        "Email": "daniel.lerner@example.com",
        "Id": 11,
        "TotalTimePlayed": 900,
        "LastName": "Lerner",
        "FirstName": "Daniel"
    }
]
```