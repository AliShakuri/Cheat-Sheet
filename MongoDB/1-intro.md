## intro

show all database
```sh
show dbs   
```

create and switch to new database
```sh
use databaseName
```

Show active database
```sh
db
```

create new collection
```sh
db.createCollection('newCollectionName')
```

show all collections
```sh
show collections
```

rename a collection
```sh
db.collectionName.renameCollection('newCollectionName')
```

delete a collection
```sh
db.collectionName.drop()
```

delete a database
```sh
db.dropDatabase()
```