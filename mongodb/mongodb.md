MongoDB is mostly used with Express.JS

The Shell-

1. mongosh {to start mongodb sever}
2. use db_name {to create & use a new database called db_name }
3. cmd+k to clear shell
4. help {get all mongodb commands}
5. show dbs {show all the databases in the system }
6. quit {to exit the shell/server}

it is a type of a javascript shell. It reconizes the javascript shell. In short we can run the javascrip commands here not all but few

test is a temporary database created for us
if we use any database then the name will change to the database in use instead of use

to save any database in the server we should save some data in it all the database are temproray in mongodb if data not stored

db gives us the current database in use

BSON data - binary JSON

JSON has some drawbacks -

1. its a text based format
2. its space ineffeicient
3. less datatypes

check JSON and bson page of mongobd.com

Collection -
Data is stored in the fromat of Document
and multiple documents together are called the collection

    Document - Mongo stores data in the form of documents
    Collection - MongoDB stores the documents in collections

    database can have multiple collections and collection can include multiple documents

Insert in DB

insertOne() - inserts a single document
insertMany() - inserts multiple documents

show collections - show the collection in the database

db.collection_name.insertOne({}) - insert data

db.collection_name.find() - show all data in the database

if the collection does not exit mongo creates one while inserting data

db.collection_name.insertMany({},{},{},{})

Finding in database -

db.collection.find()

for specific quries

db.collection.find({key:value, key:value})
db.collection.findone({key.value}) - only one data will be showed

curser - refernce to orignal- given by find
findone - gives us the actual document

Ouery operators in Find :
$gt = greater than
$gte = greater than equal to
//check website mongodb resourses

Update in Database :
db.collection.updateOne(<filter>,<update>,<optons>)
update = $set (an update operators)

Nesting : an object inside an object
to find:
db.collection.find({"key.value" : value})

DELETE in database
db.collection.deleteOne({key:value})
db.collection.deleteMany({key:value})
deleteMany with empty condition delete all collections
