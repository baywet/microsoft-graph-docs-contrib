---
description: "Automatically generated file. DO NOT MODIFY"
---

```bash


mgc device-management imported-windows-autopilot-device-identities import post --body '{\
  "importedWindowsAutopilotDeviceIdentities": [\
    {\
      "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentity",\
      "id": "985b4f49-4f49-985b-494f-5b98494f5b98",\
      "groupTag": "Group Tag value",\
      "serialNumber": "Serial Number value",\
      "productKey": "Product Key value",\
      "importId": "Import Id value",\
      "hardwareIdentifier": "aGFyZHdhcmVJZGVudGlmaWVy",\
      "state": {\
        "@odata.type": "microsoft.graph.importedWindowsAutopilotDeviceIdentityState",\
        "deviceImportStatus": "pending",\
        "deviceRegistrationId": "Device Registration Id value",\
        "deviceErrorCode": 15,\
        "deviceErrorName": "Device Error Name value"\
      },\
      "assignedUserPrincipalName": "Assigned User Principal Name value"\
    }\
  ]\
}\
'

```