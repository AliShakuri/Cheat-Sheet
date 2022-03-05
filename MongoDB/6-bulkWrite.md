# bulkWrite


### insertOne & updateMany{$set} 
inserting one object and update multiple objects by bulkrite
```js
db.collectionName.bulkWrite(
	[
		{
			insertOne: {
				'document': {
					title: "Radio",
					price: 20,
					likes: 0
				}
			}
		},
		{
			insertOne: {
				'document': {
					title: "Brush",
					price: 8,
					likes: 0
				}
			}
		},
		{
			updateMany: {
				filter: {
					likes: {
						$gte: 12
					}
				},
				update: {
					$set: {
						popular: true
					}
				}
			}
		}
	] 
)
```

### deleteOne & updateMany{$unset}
deleting one object and update multiple objects by bulkrite
```js
db.collectionName.bulkWrite(
	[
		{
			deleteOne: {
				filter: {
					title: "Radio"
				}
			}
		},
		{
			deleteOne: {
				filter: {
					title: "Brush"
				}
			}
		},
		{
			updateMany: {
				filter: {
					likes: {
						$gte: 12
					}
				},
				update: {
					$unset: {
						popular: 0
					}
				}
			}
		}
	] 
)
```