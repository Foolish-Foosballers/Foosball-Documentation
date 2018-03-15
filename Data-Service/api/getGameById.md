# Get Game by ID

Get a single game from the database and all of its associated information.

**URL** : `/games/<id>`

**URL Parameters** : `<id>` where `id` is the integer ID of the game in the database.

**Method** : `GET`

<!-- **Auth required** : NO

**Permissions required** : None -->

## Success Response

**Code** : `200 OK`

**Content examples**

For a game with ID 1 on the database lasting 300 seconds where the player on the left side of the table won with a score of 5 to 3:

```json
{
    "Single": true,
    "StartTime": "2018-01-05T15:21:51.611419",
    "RightScore": 3,
    "LeftScore": 5,
    "WinMargin": 2,
    "Winner": "Left",
    "Duration": 300,
    "Id": 1
}
```

## Error Response

**Condition** : If game does not exist with `Id` of provided `id` parameter.

**Code** : `404 NOT FOUND`

**Content** : `{}`