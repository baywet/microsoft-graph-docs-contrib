---
description: "Automatically generated file. DO NOT MODIFY"
---

```bash


mgc-beta sites lists items create-link post --site-id {site-id} --list-id {list-id} --list-item-id {listItem-id} --body '{\
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