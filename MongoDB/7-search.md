### search
Search by a field

- First by createIndex we specify in which field to search 

```js
db.collectionName.createIndex({title: "text"})
// here title is an example

db.collectionName.find({$text: {$search: "TV"}}).pretty()
```