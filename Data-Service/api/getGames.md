# Get Games

Get a full list of all the games in the database and all their associated information.

**URL** : `/games`

**Method** : `GET`

<!-- **Auth required** : NO

**Permissions required** : None -->

## Success Response

**Code** : `200 OK`

**Content examples**

For a list of games where only one series has ever been played in the system, with the player on the left side of the table emerging victorious: 

```json
[
    {
        "RightScore": 3,
        "StartTime": "2018-01-05T15:21:51.611419",
        "Id": 1,
        "LeftScore": 5,
        "Winner": "Left",
        "Duration": 300,
        "Single": true,
        "WinMargin": 2
    },
    {
        "RightScore": 5,
        "StartTime": "2018-01-05T15:33:03.684154",
        "Id": 2,
        "LeftScore": 3,
        "Winner": "Right",
        "Duration": 300,
        "Single": true,
        "WinMargin": 2
    },
    {
        "RightScore": 5,
        "StartTime": "2018-01-05T15:33:46.472350",
        "Id": 3,
        "LeftScore": 7,
        "Winner": "Left",
        "Duration": 300,
        "Single": true,
        "WinMargin": 2
    }
]
```