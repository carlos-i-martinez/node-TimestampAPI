
# API Project: Timestamp Microservice
  Timestamp microservice app that is build on the Glitch platform using Node.js and Express.js

## Project 1 of 5 for [freeCodeCamp's](https://www.freecodecamp.com) Api and Microservices Developer Certification.

App Webpage: [Timestamp API](https://fcc-timestamp-apiproject.glitch.me "Timestamp App") 

Glitch Project: [Timestamp API](https://glitch.com/~fcc-timestamp-apiproject)
 
Completed API and Microservices Certification: [Certificate](https://www.freecodecamp.org/certification/carlitos/data-visualization "FreeCodeCamp.Com").

## Technologies Used:
> * HTML, JavaScript, CSS, Node.js and Express.js   

## Some requirements to complete project:
1. The API endpoint is `GET https://fcc-timestamp-apiproject.glitch.me/api/timestamp/:date_string?`
2. A date string is valid if can be successfully parsed by `new Date(date_string)` (JS) . Note that the unix timestamp needs to be an **integer** (not a string) specifying **milliseconds**. In our test we will use date strings compliant with ISO-8601 (e.g. `"2016-11-20"`) because this will ensure an UTC timestamp.
3. If the date string is **empty** it should be equivalent to trigger `new Date()`, i.e. the service uses the current timestamp.
4. If the date string is **valid** the api returns a JSON having the structure 
`{"unix": <date.getTime()>, "utc" : <date.toUTCString()> }`
e.g. `{"unix": 1479663089000 ,"utc": "Sun, 20 Nov 2016 17:31:29 GMT"}`.
5. If the date string is **invalid** the api returns a JSON having the structure `{"unix": null, "utc" : "Invalid Date" }`. It is what you get from the date manipulation functions used above.

#### Example usage:
* https://fcc-timestamp-apiproject.glitch.me/api/timestamp/2015-12-15
* https://fcc-timestamp-apiproject.glitch.me/api/timestamp/1450137600000

#### Example output:
* { "unix": 1450137600, "natural": "December 15, 2015" }
