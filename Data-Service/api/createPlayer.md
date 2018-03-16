# Create Player

Create a player entry in the database, effectively registering them in the system.

**URL** : `/players`

**Method** : `POST`

<!-- **Auth required** : YES

**Permissions required** : None -->

**Data constraints**

Provide first name, last name, username, and email of player to be created. Username must be 9 characters, all numbers.

**Data example** All fields must be sent.

```json
{
	"FirstName": "Sara",
	"LastName": "Stiklickas",
	"Username": "212570174",
	"Email": "sara.stiklickas@ge.com"
}
```

## Success Response

**Condition** : If everything is OK and an account didn't exist for this player.

**Code** : `201 CREATED`

**Content example**

```json
{
    "GameWins": 0,
    "TotalGamesPlayed": 0,
    "Shutouts": 0,
    "TotalTimePlayed": 0,
    "LastName": "Stiklickas",
    "SignupDate": "2018-03-15T23:44:59.159643",
    "FirstName": "Sara",
    "Email": "sara.stiklickas@example.com",
    "Ranking": 0,
    "TotalPoints": 0,
    "Id": 1,
    "Username": "212123456",
    "SeriesWins": 0
}
```

## Error Responses

**Condition** : If Account already exists for User.

**Code** : `303 SEE OTHER`

### Or

**Condition** : If fields are missed.

**Code** : `400 BAD REQUEST`
