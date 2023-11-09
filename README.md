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



