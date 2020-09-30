# Playlist-API
Web service implementation that can create playlists from Swagger interface and has Couchbase as its datasource, created with Spring Boot.

*This project was given as a homework from Trendyol Tech Team, during the Kodluyoruz Trendyol Tech Talent Bootcamp.*

## Requirements:

  - should create a bucket called playlist and it should hold inside it documents for user's playlists. 
  - playlist should include
      id (can be generated with UUI)
      name,
      description,
      followersCount(int)
      tracks (list of track)
      trackCount(int),
      userId

  - track object should include: "name" , "length"(string) , artist(string)


Endpoints:

  - playlist create endpoint (save a playlist using a userId)

  - playlist findById endpoint (get playlist using playlistId)
  
  - playlist findAllByUserId endpoint (return all playlists of a user using userId) (used pagination)

  - playlist delete endpoint  (delete playlist using playlistId)

  - add track to playlist endpoint  (add track to a playlist using playlistId)

  - remove track to playlist endpoint  (delete track from a playlist using playlistId)
  
  - get track of playlist endpoint (get track from a playlist using playlistId and index of track) (was not required)
