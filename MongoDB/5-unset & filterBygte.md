### unset

delete one field of objects
```js
db.collectionName.updateMany({}, {$unset: {field_to_be_cleared: 0}})
// {} --> means All 
```

### filter by gte or lte

```js
db.collectionName.find({your_field: {$gte: 150}})
db.collectionName.find({your_field: {$lte: 20}})
```