### count
Show number of members of a collection 
```js
db.collectionName.find().count()
```

### sort
sort a collection 
```js
db.collectionName.find().sort({x})

// Example : 
{x} = {created: -1}
```

### pagination
Page pagination
```js
var paginated_by = 3
var page = 1
db.collectionName.find().sort({created: -1}).skip(paginated_by * (page - 1)).limit(paginated_by).pretty()

// and go to the next page :
var page = 2
db.collectionName.find().sort({created: -1}).skip(paginated_by * (page - 1)).limit(paginated_by).pretty()
‍‍```