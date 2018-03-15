# Get Player by ID

Get a single player from the database and all of his associated information.

**URL** : `/players/<id>`

**URL Parameters** : `<id>` where `id` is the integer ID of the player in the database.

**Method** : `GET`

<!-- **Auth required** : NO

**Permissions required** : None -->

## Success Response

**Code** : `200 OK`

**Content examples**

For a user with ID 1 on the database who has played and won one series of three games, and is currently the top-ranked player:

```json
{
    "Username": "212123456",
    "Id": 1,
    "Email": "sara.stiklickas@example.com",
    "SeriesWins": 1,
    "TotalTimePlayed": 900,
    "Ranking": 1,
    "Shutouts": 0,
    "LastName": "Stiklickas",
    "TotalGamesPlayed": 3,
    "FirstName": "Sara",
    "TotalPoints": 15,
    "SignupDate": "2018-01-05T15:04:32.825103",
    "GameWins": 2
}
```

## Error Response

**Condition** : If player does not exist with `Id` of provided `id` parameter.

**Code** : `404 NOT FOUND`

**Content** : `{}`