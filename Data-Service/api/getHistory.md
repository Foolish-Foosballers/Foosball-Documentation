# Get History

Get a full list of all the history entries in the database and all their associated information.

**URL** : `/history`

**Method** : `GET`

<!-- **Auth required** : NO

**Permissions required** : None -->

## Success Response

**Code** : `200 OK`

**Content examples**

For a list of history entries where 3 singles games have been played, so there is one entry per player per game:

```json
[
    {
        "SeriesId": 1,
        "GameId": 1,
        "PlayerId": 1,
        "Side": "Left"
    },
    {
        "SeriesId": 1,
        "GameId": 1,
        "PlayerId": 2,
        "Side": "Right"
    },
    {
        "SeriesId": 1,
        "GameId": 2,
        "PlayerId": 2,
        "Side": "Right"
    },
    {
        "SeriesId": 1,
        "GameId": 2,
        "PlayerId": 1,
        "Side": "Left"
    },
    {
        "SeriesId": 1,
        "GameId": 3,
        "PlayerId": 1,
        "Side": "Left"
    },
    {
        "SeriesId": 1,
        "GameId": 3,
        "PlayerId": 2,
        "Side": "Right"
    }
]
```