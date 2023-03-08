# API Documentation

* json data only
* basic parameters
  * fn: always required, decides which api function is used
all requests via POST to "exampledomain.eu/api.php"
## Features

* get the serverstatus
  * parameters
    * fn
      * serverstatus
  * response
    * status
      * should be "ok", if not there is an error
    * serveronline
      * returns 1 in case the server is online, otherwise 0
    * playersonline
      * returns amount of online players
    * motd
      * returns the message of the day
  * **examples**
    * request: {"fn":"serverstatus"}
    * response: {"status":"ok","serveronline":"1","playersonline":"250","motd":"meow"}
