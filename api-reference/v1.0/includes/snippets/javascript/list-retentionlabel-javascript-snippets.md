---
description: "Automatically generated file. DO NOT MODIFY"
---

```javascript

const options = {
	authProvider,
};

const client = Client.init(options);

let retentionLabels = await client.api('/security/labels/retentionLabels')
	.get();

```