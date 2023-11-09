# MongoDB_01
**1.Create a Database called movies**

test> use movies
switched to db movies

**2.Create a collection called moviedetails.**

movies> db.createCollection("movie_details")
{ ok: 1 }

**3.Create above 5 movie documents into a moviedetails collection.**

movies> db.movie_details.insertMany([{"movie_title":"jurassic park","type":"adventure","director":"steven spielber","release":"1993"},{"movie_title":"forrest gump","type":"darama","director":"robert zemeckies","release":"1994"},{"movie_title":"titanic","type":"romance","director":"james cameron","release":"1997"},{"movie_title":"the dark night","type":"action","director":"christopher","release":"2008"},{"movie_title":"avatar","type":"science fiction","director":"james cameron","release year":"2009"}])
{
  acknowledged: true,
  insertedIds: {
    '0': ObjectId("654cb0aea645cb7638ba417a"),
    '1': ObjectId("654cb0aea645cb7638ba417b"),
    '2': ObjectId("654cb0aea645cb7638ba417c"),
    '3': ObjectId("654cb0aea645cb7638ba417d"),
    '4': ObjectId("654cb0aea645cb7638ba417e")
  }
}

**4. List all documents created.**
[
{
_id: ObjectId("654c7f5117597cba8b45c14f"),
Movie Title: 'Jurassic Park',
Type: 'Adventure',
Director: 'steven Spielberg',
Release year: 1993
},
{
_id: ObjectId("654c7f5117597cba8b45c150"),
Movie Title: 'Forrest Gump',
Type: 'drama',
Director: 'Robert Zemeckies',
Release year: 1994
},
{
_id: ObjectId("654c7f5117597cba8b45c151"),
Movie Title: 'Titanic',
Type: 'Romance',
Director: 'James Cameron',
Release Year: 1997
},
{
_id: ObjectId("654c7f5117597cba8b45c152"),
Movie Tile: 'The Dark Knight',
Type: 'Action',
Director: 'Christopher Nolan',
Release Year: 2008
},
{
_id: ObjectId("654c7f5117597cba8b45c153"),
Movie Title: 'Avatar',
Type: 'Science Fiction',
Director: 'James Cameron',
Release Year: 2009
}
]



