### increment

increment values of one object
```js
db.collectionName.updateOne({x}, {$inc: {y}})
// x --> filter by this field 

// Example : 
{x} = {'id': 'userId'}
{y} = {likes: -1}
```

### rename

rename field of objects
```js
db.collectionName.updateMany({}, {$rename: {old_field: 'new_field'}})
// {} --> means All 
```