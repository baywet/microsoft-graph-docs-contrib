---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

from msgraph_beta import GraphServiceClient
from msgraph_beta.generated.models.identity_security_defaults_enforcement_policy import IdentitySecurityDefaultsEnforcementPolicy

graph_client = GraphServiceClient(credentials, scopes)

request_body = IdentitySecurityDefaultsEnforcementPolicy(
	is_enabled = False,
)

result = await graph_client.policies.identity_security_defaults_enforcement_policy.patch(request_body)


```