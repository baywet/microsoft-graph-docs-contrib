---
description: "Automatically generated file. DO NOT MODIFY"
---

```bash


mgc-beta drives items invite post --drive-id {drive-id} --drive-item-id {driveItem-id} --body '{\
  "recipients": [\
    {\
      "email": "robin@contoso.org"\
    }\
  ],\
  "message": "Here's the file that we're collaborating on.",\
  "requireSignIn": true,\
  "sendInvitation": true,\
  "roles": [ "write" ],\
  "password": "password123",\
  "expirationDateTime": "2018-07-15T14:00:00.000Z"\
}\
'

```