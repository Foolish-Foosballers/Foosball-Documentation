# Create Series

Create a series entry in the database.

**URL** : `/series`

**Method** : `POST`

<!-- **Auth required** : YES

**Permissions required** : None -->

**Data constraints**

Provide number of games in the series, number of games won by the left player, and number of games won by the right player. All must be integers.

**Data example** All fields must be sent.

```json
{
	"NumGames": "3",
	"LeftWins": "2",
	"RightWins": "1"
}
```

## Success Response

**Condition** : If everything is OK.

**Code** : `201 CREATED`

**Content example**

```json
{
    "LeftWins": 2,
    "Id": 3,
    "NumGames": 3,
    "RightWins": 0
}
```

## Error Responses

**Condition** : If fields are missed.

**Code** : `400 BAD REQUEST`
