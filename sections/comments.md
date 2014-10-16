##Comments

###Get comments
`GET /projects/1/cards/4160/comments.json` get all comments for a card

Response
```json
[
  {
    "card_id": 4160,
    "comment": "comment text",
    "created_at": "2013-03-01T09:07:43Z",
    "id": 466,
    "updated_at": "2013-03-01T09:07:43Z",
    "user_id": 5,
    "user": 
	    {
	    "id": 5,
	    "email": "john@breeze.pm",
	    "name": "John Doe"
	    "avatar": "https://avatarurl.com/avatar.jpg"
	   }
  },
  {
    "card_id": 4160,
    "comment": "second comment text",
    "created_at": "2013-02-01T08:07:13Z",
    "id": 467,
    "updated_at": "2013-02-01T08:07:13Z",
    "user_id": 5,
    "user": 
	    {
	    "id": 5,
	    "email": "john@breeze.pm",
	    "name": "John Doe"
	    "avatar": "https://avatarurl.com/avatar.jpg"
	   }
  }
]
```

###Create a comment

`POST /projects/1/cards/4160/comments.json` create a new comment for a card
Request
```json
{
  "comment": "comment text"
} 
```

###Update comment

`PUT /projects/1/cards/4160/comments/466.json` update specific comments for a card

Request
```json
{
  "comment": "comment text"
} 
```

###Remove comment


`DELETE /projects/1/cards/4160/comments/466.json` delete comment from card
