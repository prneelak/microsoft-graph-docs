---
description: "Automatically generated file. DO NOT MODIFY"
---

```javascript

const options = {
	authProvider,
};

const client = Client.init(options);

const string = {
  securityEnabledOnly: true
};

let res = await client.api('/contacts/{id}/getMemberGroups')
	.version('beta')
	.post(string);

```