# Day 11

## npm code things

npm install express to install the server and start.
npm init to get the setup and license and author name on you server.
npm install for installing things.

## express
```js
let express = require("express")
let app = express()
```
to get express in your file and make life easier.

```js
app.get("/", (request, response)=>{
  response.send("howdy")
})
```

```js
app.get("/greet/:fname/:lname", (request, response)=>{
  let {fname, lname} = request.params;
  response.send([`Hellp ${fname} ${lname}`])
})
```

to start your server listening on a port
```js
app.listen(port number);
```
