# pangram-test

In the framework of your choice, please create automated tests for the pangram-api.  A pangram is a sentence or a verse that contains all the letters of the alphabet.

Here's a quick description of the pangram-api.

## POST /pangram

### Header:

Content-Type: application/json

Body:  {'string':'Some String;}

### Response

Content-Type: application/json
  
200:  {"pangram":"true"} if string is a pangram

200: {"pangram":"false"} if string is not a pangram

404: {"message":"Not Enough Characters In String"} if string is less than 26 characters
