---
description: "Automatically generated file. DO NOT MODIFY"
---

```javascript

const options = {
	authProvider,
};

const client = Client.init(options);

const domain = {
  isDefault: true,
  supportedServices: [
    'Email',
    'OfficeCommunicationsOnline',
    'CustomUrlDomain'
  ]
};

await client.api('/domains/contoso.com')
	.version('beta')
	.update(domain);

```