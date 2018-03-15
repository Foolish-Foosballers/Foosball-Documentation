# Get Series

Get a full list of all the series in the database and all their associated information.

**URL** : `/series`

**Method** : `GET`

<!-- **Auth required** : NO

**Permissions required** : None -->

## Success Response

**Code** : `200 OK`

**Content examples**

For a list of series where only one series has been played in the system, and the player on the left side won two out of three games:

```json
[
    {
        "RightWins": 1,
        "Id": 1,
        "LeftWins": 2,
        "NumGames": 3
    }
]
```