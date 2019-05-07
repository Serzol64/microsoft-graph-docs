
```Javascript

const options = {
	authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/messages')
	.version('beta')
	.select('sender,subject')
	.get();

```