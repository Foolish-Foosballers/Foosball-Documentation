# Create History

Create a history entry in the database. A history entry is created per player per game.

**URL** : `/history`

**Method** : `POST`

<!-- **Auth required** : YES

**Permissions required** : None -->

**Data constraints**

Provide the ID of the game, the ID of the player, the ID of the series, and the side that the provided player was on. All IDs must exist in their respective tables and correspond to the primary keys for their rows. `Side` must be either `Left` or `Right`. 

**Data example** All fields must be sent.

```json
{
	"GameId": "1",
	"PlayerId": "1", 
	"SeriesId": "1",
	"Side": "Left"
}
```

## Success Response

**Condition** : If everything is OK and the history entry doesn't already exist.

**Code** : `201 CREATED`

**Content example**

```json
{
    "Side": "Left",
    "SeriesId": 3,
    "GameId": 4,
    "PlayerId": 12
}
```

## Error Responses

**Condition** : If the history entry already exists.

**Code** : `303 SEE OTHER`

**Or**

**Condition** : If fields are missed.

**Code** : `400 BAD REQUEST`
