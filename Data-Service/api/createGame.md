# Create Game

Create a game entry in the database.

**URL** : `/games`

**Method** : `POST`

<!-- **Auth required** : YES

**Permissions required** : None -->

**Data constraints**

Provide duration, whether the game was singles or doubles, the left player's score, the right player's score, the win margin, and the winner. `Single` must be either `True` or `False`, and `Winner` must be either `Left` or `Right`. Duration is measured in seconds.

**Data example** All fields must be sent.

```json
{
	"Duration": "300",
	"Single": "True",
	"LeftScore": "5",
	"RightScore": "2",
	"WinMargin": "3",
	"Winner": "Left"
}
```

## Success Response

**Condition** : If everything is OK.

**Code** : `201 CREATED`

**Content example**

```json
{
    "Duration": 300,
    "Winner": "Left",
    "LeftScore": 5,
    "StartTime": "2018-03-15T23:52:52.602383",
    "WinMargin": 3,
    "RightScore": 2,
    "Id": 4,
    "Single": true
}
```

## Error Responses

**Condition** : If fields are missed.

**Code** : `400 BAD REQUEST`
