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

### GET /clicks
Gets the currect clicks in the cookie clicker project
Succesful response: 200 {clicks: CLICK_COUNT}

### GET /rooms?room=
Gets the room. Use the required room query to specify the room name
Successful response: 200 {room: name: ROOM_NAME, host: ROOM_HOST, player: PLAYYER}
Error responses:
- 400: missing room query
- 404: room not found

