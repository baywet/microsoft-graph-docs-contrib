---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

from msgraph_beta import GraphServiceClient

graph_client = GraphServiceClient(credentials, scopes)


result = await graph_client.print.shares.by_printer_share_id('printerShare-id').allowed_groups.get()


```