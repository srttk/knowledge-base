# MongoDB


### Set DB path
```
mongod --dbpath F:\org\mongo\data
```


## Install Service D:\Program Files\MongoDB\Server\3.4
mongod --config f:\org\mongo\mongod.cfg --install
### Create user and assign permissions

```Shell
db.createUser(user, writeConcern)

```

Creates a new user for the database where the method runs. db.createUser() returns a duplicate user error if the user already exists on the database.


#### Example

```json
db.createUser(
   {
     user: "mynewuser",
     pwd: "myuser123",
     roles: [ "readWrite", "dbAdmin" ]
   }
);

```



## Reference

+ [Mongo Shell Reference ](https://docs.mongodb.com/manual/reference/mongo-shell/)
