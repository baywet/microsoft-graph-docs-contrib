---
description: "Automatically generated file. DO NOT MODIFY"
---

```bash


mgc-beta drives items create-link post --drive-id {drive-id} --drive-item-id {driveItem-id} --body '{\
  "type": "view",\
  "scope": "anonymous",\
  "password": "String",\
  "recipients": [\
    {\
      "@odata.type": "microsoft.graph.driveRecipient"\
    }\
  ],\
  "sendNotification": true,\
  "retainInheritedPermissions": false\
}\
'

```