Breeze API Documentation
====================



## The API Format

The API accepts only JSON requests. Please make sure you're setting `Content-Type: application/json`in your request header. Each request returns a **JSON-encoded** body.

The result of each action is communicated via standard HTTP response codes.


## API token

Each user has an API token. You can find it under **"Personal settings & password"** in the **"API Token"** section.

## Accessing the API
Accessing the API uses the following URL schema:

```shell
https://api.breeze.pm/<resource>
```

Where resource is the resource you want to access (e.g. projects, cards, todos etc)

For example, getting a list of projects would result in the URL:
```shell
curl -u user:pass https://api.breeze.pm/projects.json 
```
To create or update something you also have to include the Content-Type header and the JSON data.
```shell
curl -u user:pass \
 -H 'Content-Type: application/json' \
 -d '{ "name": "New project" }' \
 http://api.breeze.pm/projects.json 
 ```


## Authentication
Breeze API supports HTTP Basic auth and token based authentication.

Basic auth
To get you started with Breeze API you can just use HTTP Basic authentication with your login info.
```shell
curl -u username:password http://api.breeze.pm/projects.json 
```
API token
You can also authenticate by providing your API token in the request. The token has to be sent for each request your application makes to the Breeze API. Remember that anyone who has your api token can see and change everything you have access to. Keep it safe ! You can manage your API token from your profile.
```shell
curl -u 6dasdg782: https://api.breeze.pm/projects.json 
```
You can also pass the api token as a query parameter in the url.
```shell
curl http://api.breeze.pm/projects.json?api_token=6dasdg782
```


## API ready for use
* [Projects](https://github.com/breezepm/breeze_api_docs/blob/master/sections/projects.md)
* [Cards](https://github.com/breezepm/breeze_api_docs/blob/master/sections/cards.md)
* [Lists](https://github.com/breezepm/breeze_api_docs/blob/master/sections/lists.md)
* [Comments](https://github.com/breezepm/breeze_api_docs/blob/master/sections/comments.md)
* [Todos](https://github.com/breezepm/breeze_api_docs/blob/master/sections/todos.md)
* [Time entries](https://github.com/breezepm/breeze_api_docs/blob/master/sections/time_entries.md)
* [Activities](https://github.com/breezepm/breeze_api_docs/blob/master/sections/activities.md)


## Help us make it better

If you have any requests or you found a bug, you can use Github issues to let us know. You can also fork the docs and send a pull request with improvements


