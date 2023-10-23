#Node #Code #Backend #JavaScript 
# Przyjmowanie [[request|requestów]]:
`app.METHOD(PATH, HANDLER);`
METHOD - get, post, …
PATH - "/"
HANDLER - `function(req, res){}`

np:
```js
app.get("/", function(req, res) {
  res.sendFile(__dirname + "/views/index.html")
  console.log("Sent response");
});

app.get("/json", function(req, res){
  res.json({"message": "Hello json"});
  console.log("Sent JSON");
})
```

# [[Middleware]]
app.use(PATH, MIDDLEWARE

PATH - opcjonalne, gdy się go nie poda funkcja będzie wykonywana każdego requestu.
MIDDLEWARE - funkcja wykonywana dla requestu

np:
```js
app.use("/public", express.static(__dirname + "/public"));
```