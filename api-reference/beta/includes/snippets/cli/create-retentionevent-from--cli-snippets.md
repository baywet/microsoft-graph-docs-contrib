---
description: "Automatically generated file. DO NOT MODIFY"
---

```bash


mgc-beta security triggers retention-events create --body '{\
  "@odata.type": "#microsoft.graph.security.retentionEvent",\
  "displayName": "String",\
  "description": "String",\
  "eventQueries": [\
    {\
      "@odata.type": "microsoft.graph.security.eventQuery"\
    }\
  ],\
  "eventTriggerDateTime": "String (timestamp)",\
  "createdBy": {\
    "@odata.type": "microsoft.graph.identitySet"\
  },\
  "eventPropagationResults": [\
    {\
      "@odata.type": "microsoft.graph.security.eventPropagationResult"\
    }\
  ],\
  "eventStatus": {\
    "@odata.type": "microsoft.graph.security.retentionEventStatus"\
  },\
  "lastStatusUpdateDateTime": "String (timestamp)"\
}\
'

```