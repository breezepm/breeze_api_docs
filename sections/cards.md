#Cards

##Add tags

You can add and update tags with the card POST/PUT methods. Add an array of tags to the json. 

Example:

```
POST /projects/:project_id/cards.json
{
  "name": "new task from API",
  "tags": ["tag1","tag2"]
  
}
```

When you update the card then all the tags are overwritten, not appended. 

Example:

```
PUT /projects/:project_id/cards/:card_id.json 
{
  "tags": ["tag3"]
  
}
Now the task only has 1 tag "tag3".
```
##Errors

###Move a card
Error in the documentation, to move a card use PUT not POST.

```
~~POST~~ PUT /projects/:project_id/cards/:card_id.json move a card

Request
{
  "stage_id": 9,
  "prev_id": 9
}
```

