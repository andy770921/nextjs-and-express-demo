# Node Server Deployed in Vercel

## Demo Link

- Home Page: [https://node-server-in-vercel.vercel.app/](https://node-server-in-vercel.vercel.app/)
- About Page: [https://node-server-in-vercel.vercel.app/about](https://node-server-in-vercel.vercel.app/about)

## Node Server Example

```js
const express = require('express');

const app = express();

app.get('/', (req, res) => res.send('Home Page Route'));

app.get('/about', (req, res) => res.send('About Page Route'));

app.get('/portfolio', (req, res) => res.send('Portfolio Page Route'));

app.get('/contact', (req, res) => res.send('Contact Page Route'));

const port = process.env.PORT || 3000;

app.listen(port, () => console.log(`Server running on ${port}, http://localhost:${port}`));
```

## Reference Tutorial

[How to deploy a Node/Express App to Vercel](https://dev.to/andrewbaisden/how-to-deploy-a-node-express-app-to-vercel-2aa)

## Development

1. `npm install`

2. `npm run start`: start running local server

## Deployment

1. `npm i -g vercel`

2. `vercel`: init vercel setting. auto-generate `.vercel` folder

3. Add `vercel.json` file: define node.js file path and root route path

## Features

- After linking the corresponding GitHub repo to Vercel project, the deployment will be executed automatically

- [Price is for Free](https://vercel.com/pricing), pay as you grow
