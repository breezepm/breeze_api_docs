##Activity and audit log

All activity responses are paginated 50 items per page. To get the next page append **?page=XX** to the query.

### Get activity from all projects
* `GET /activities.json` get all activity entries

Response
```json
[
  {
    "id": 4160,
    "created_at": "2013-03-01T09:07:43Z",
    "user": "Jake",
    "project_id": 1723,
    "card_id": 324785,
    "message": "logged <b>9h</b> of work for <a href="https://app.breeze.pm/projects/4186-name-the-project/cards/71399-asd-asd">Task name</a>",
  },
  {
   "id": 1040,
   "created_at": "2013-03-01T02:07:43Z",
   "user": "John",
   "project_id": 123,
   "card_id": 16485,
   "message": "<b>tagged</b> <a href="https://app.breeze.pm/projects/4186-aaaaaname-the-project/cards/70327-asdasd">Task name</a> with <b> bugs</b>",
  }
] 
```

###Get activity from all projects by a user
* `GET /activities/:user_id.json` get activity entries

Response is same as for all activities query.

###Get activity from a project
* `GET /projects/:project_id/activities.json` get all activity entries

Response is same as for all activities query.

###Get activity from a projects by a user
* `GET /projects/:project_id/activities/:user_id.json` get activity entries

Response is same as for all activities query.
