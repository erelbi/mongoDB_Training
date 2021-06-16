---
description: BSON&JSON
---

# Mongo Shell



![](.gitbook/assets/sorucevap.png)

| JSON | BSON |
| :--- | :--- |
| mongoimport | mongorestore |
| mongoexport | mongodump |

![](.gitbook/assets/bson-json.png)

### Sample Data Restore

{% embed url="https://erelbi.github.io/mongodb\_sample\_data/" %}

```text
show dbs;
```

![](.gitbook/assets/showdbs.png)

```text
use sample_airbnb
show collections;
```

![](.gitbook/assets/show-collections.png)

### Find & FindOne

```text
use sample_mflix
show collections
db.movies.findOne()
```

![](.gitbook/assets/find.png)

```text
db.movies.find()
```

![](.gitbook/assets/find2.png)

**Type "it" for more**

```text
it
```

#### Pretty\(\)

```text
db.movies.find().pretty()
```

#### Count\(\)

```text
db.movies.find().count()
```

### Find\({'filed':'value'}\)

```text
db.movies.find({'year':1983})
```

### Subdocument Find

```text
db.movies.find({'year':1983, 'imdb.rating':6.2})
```

![](.gitbook/assets/find3.png)

```text
db.movies.find({'year':1983, 'imdb.rating':6.2,'countries':['Italy']}).pretty()
```

![](.gitbook/assets/find4.png)

### Find Filter Filed \(3F\) \( Böyle bir Tabir Yok :\)\)

```text
db.movies.find({'year':1983, 'imdb.rating':6.2},{'cast':1}).pretty()
```

![](.gitbook/assets/find5.png)

### MongoDB Quiz-1

[https://forms.gle/8M3PBmYM5vT5mybr8](https://forms.gle/8M3PBmYM5vT5mybr8)

