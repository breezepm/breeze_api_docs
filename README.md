Breeze API Documentation
====================



##The API Format##

The API accepts only JSON requests. Please make sure you're setting `Content-Type: application/json`in your request header. Each request returns a **JSON-encoded** body.

The result of each action is communicated via standard HTTP response codes.


###Example requests###

The example requests here are done using a command line tool called [cURL](http://en.wikipedia.org/wiki/CURL). If you want to try the requests out yourself, you can download cURL from [here](http://curl.haxx.se/download.html). It is available for all possible operating systems.

Under Ubuntu installing cURL is very easy:

```shell
sudo apt-get install curl
```

##API token##

Each user has an API token. You can find it under "Personal settings & password" in "API Token" section.

##Help us towards a better API##

If you have any requests or you found a bug, you can use Github issues to let us know. You can also fork the docs and send a pull request with improvements

