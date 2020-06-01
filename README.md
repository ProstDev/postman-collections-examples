# postman-collections-examples
This is a repository to keep some examples of Postman Collections.

You can download a specific collection, or clone the entire repository, 
and then you can click "Import" from Postman, to be able to see the collection from there.

## Slack API collection
Contains 2 requests done to the Slack API, pointing to ProstDev's workspace.

First request performs 7 tests to the team.info method:

1. That the Content-Type header is present in the response.
2. That the Content-Type header in the response is of “application/json”.
3. That there is a response body.
4. That the response body is in a JSON format.
5. That the response body contains “ok”: true.
6. That the team.name in the response is “ProstDev”.
7. That the response status is 200 OK.

Second request is a negative scenario that calls an unexistent method and performs 7 tests 
to make sure it's sending the correct error in the response:

1. That the Content-Type header is present in the response.
2. That the Content-Type header in the response is of “application/json”.
3. That there is a response body.
4. That the response body is in a JSON format.
5. That the response body contains “ok”: false.
6. That the error in the response is “unknown_method”.
7. That the response status is 200 OK.
