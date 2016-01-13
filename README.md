# Learning MongoDB

## Commands
- mongod
- mongo
- show dbs
- mongoimport -d [???] -c users --file [FILE_NAME]
- mongoexport -d [???] -c users --out [FILE_NAME]
    - export db in json
- mongodump
    - binary export
- mongorestore
    - restore binary export
- bsondump
- mongostat
- use [DB_NAME]
    - change/switch DB
    - there is NO command to create DB
- db
    - set variable as DB (after *user [DB_NAME]*)
- db.[COLLECTIONS]
    - e.g. db.links
    - don't have to create collections (similar to DB)
- db.[COLLECTIONS].count()
    - to check number of documents
    - e.g. db.links.count()
- db.[COLLECTIONS].insert({[JSON_DATA]})
    - e.g. db.links.insert({title: "google search", url:"www.google.com", comment:"top search engine", tags:["default","main page"], saved_on: new Date()})
- db.[COLLECTIONS].save({[JSON_DATA]})
    - e.g. db.links.save({title: "yahoo search", url: "www.yahoo.com", saved_on: new Date()})
- db.[COLLECTIONS].find()
    - e.g. db.links.find()
    - query the database to find the documents

### Notes
- bson: binary JSON
- Collection: Like an RDBMS table; but collection has no schemas.
- Document: Like an RDBMS record or row. There are bson documents.
- Field: Like an RDBMS column; {key: value}
- 

------------------

http://code.tutsplus.com/courses/learning-mongodb

## Contents

1. Getting Started 4 lessons, 12:45

    1.1 Introduction 01:05

    1.2 Installing MongoDB 05:41

    1.3 MongoDB Tools 03:35

    1.4 NoSQL Database Terms 02:24

2. Getting Practical3 lessons, 24:34

    2.1 Creating Databases, Collections, and Documents 08:20

    2.2 ObjectIDs 07:42

    2.3 Relating Documents 08:32

3. Querying Your Database9 lessons, 1:35:29

    3.1 Finding Documents and Choosing Fields 14:25

    3.2 Operators, part 1 07:57

    3.3 Operators, part 2 15:30

    3.4 Grouping and Regular Expression 08:40

    3.5 Cursor Methods, Sorting, and Paging 06:59

    3.6 Updating Documents, part 1 14:08

    3.7 Updating Documents, part 2 11:21

    3.8 Deleting Documents, Collections, and Database 03:51

    3.9 Indexes 12:38

4. Digging Deeper3 lessons, 39:37

    4.1 The PHP Driver 21:05

    4.2 The Node.js Driver 14:51

    4.3 NoSQL vs. SQL 03:41

5. Conclusion1 lesson, 01:17

    5.1 Conclusion 01:17