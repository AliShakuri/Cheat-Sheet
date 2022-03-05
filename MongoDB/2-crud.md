### insert --> create

Add one object to collection
```js
db.collectionName.insertOne({jsonObject})
```

Add multiple objects to the collection
```js
db.collectionName.insert([{jsonObjects}])
```
### find --> read
Show first object
```js
db.collectionName.findOne()
```

Show all objects
```js
db.collectionName.find().pretty()
```

### update
update one object
```js
db.collectionName.upadteOne(
    {x}, {$set: {example_new_field: "newName"}}
)
// x --> filter by this field 

// Example : 
{x} = {'id': 'userId'}
```

update multiple objects
```js
db.collectionName.updateMany(
    {x}, {$set: {example_new_field: 'newValue'}}
)
// x --> filter by this field 

// Example : 
{x} = {status: true}
```

### replace
Replace one field with another
```js
db.collectionName.replaceOne({x},{y})
// y replaces x

// Example : 
{x} = {first_name: 'Kaveh'}
{y} = {full_name: 'Kaveh Yaghmaei'}
```

### delete
delete first object
```js
db.collectionName.deleteOne({x})

// Example : 
{x} = {status: true}
```

delete multiple objects
```js
db.collectionName.deleteMany({x})

// Example : 
{x} = {status: true}
```