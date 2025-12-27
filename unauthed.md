---
permalink: /unauthed
title: Unauthed API endpoints
---
# Unauthed API endpoints
**The endpoints that doesn't require a auth header**

### GET /announcement
Gets the currect announcement.
Success response: 200 {announcement: ANNOUNCEMENT}
[try](https://thenamelessdev.com/projects/request?url=https://thenamelessdev.com/api/v1/announcement&method=GET)

### POST /request
A request proxy thing
Required body keys:
- method: the request method in all caps (example: GET)
- url: the url the request should be made on
- body: the request body. It expects a JSON body (optional)
- the request headers. It expects it in JSON (optional)
Successful response: 200 {status: RESPONSE_STATUS_CODE, body: RESPONSE_BODY, headers: RESPONSE_HEADERS}
Errors:
- 400: invalid method, invalid url or missing field (URL and/or method)
[try](https://thenamelessdev.com/projects/request?url=https://thenamelessdev.com/api/v1/request&method=POST)
