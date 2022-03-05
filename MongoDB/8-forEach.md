### forEach
use the forEach loop for shows objects
```js
db.collectionName.find().forEach((d) => {print(d.title)})

db.collectionName.find().forEach((d) => {print(`${d.title} is ${d.price}$`)})
```