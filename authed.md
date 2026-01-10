---
permalink: /authed
title: Authed API endpoints
---
# Authed API endpoints
**All API andpoints that require a auth header or login**
Authing information [here](/#authing)

### GET /verify
Verifies you api key.
Successful status code: 204

[try](https://thenamelessdev.com/projects/request?url=https://thenamelessdev.com/api/v1/verify&method=GET)

### GET /clicks
Gets the currect clicks in the cookie clicker project
Succesful response: 200 {clicks: CLICK_COUNT}

[try](https://thenamelessdev.com/projects/request?url=https://thenamelessdev.com/api/v1/clicks&method=GET)

### GET /ttt/rooms?room=
Gets the room. Use the required room query to specify the room name
Successful response: 200 {room: name: ROOM_NAME, host: ROOM_HOST, player: PLAYYER}
Error responses:
- 400: missing room query
- 404: room not found

[try](https://thenamelessdev.com/projects/request?url=https://thenamelessdev.com/api/v1/rooms?room=&method=GET)

### POST /encode
Encodes a text x times in Base64
Request body: {"text": TEXT TO ENCODE, "times": ENCODE THIS MANY TIMES}
Succesful response: 200 {output: ENCODED OUTPUT}
Errors: 400 times in NaN, 500 error while encoding

[try](https://thenamelessdev.com/projects/request?url=https://thenamelessdev.com/api/v1/encode&method=POST)

### POST /decode
Decodes a text x times in Base64
Request body: {"text": TEXT TO DECODE, "times": DECODE THIS MANY TIMES}
Succesful response: 200 {output: ENCODED OUTPUT}
Errors: 400 times in NaN, 500 error while decoding

[try](https://thenamelessdev.com/projects/request?url=https://thenamelessdev.com/api/v1/decode&method=POST)
