# Momb-music-app
This is a music app that allows users to search and play their favourite music
This code creates a music player that can play, pause, skip to the next song, and stop songs from a playlist.

Song class

The Song class represents a single song and has the following properties:

title (string): the title of the songartist (string): the name of the artist who performed the songalbum (string): the name of the album on which the song appearsduration (string): the duration of the song in the format of mm:ssurl (string): the URL where the song can be found online

Playlist class

The Playlist class represents a collection of songs and has the following properties:

name (string): the name of the playlistsongs (array of Song objects): an array of Song objects that make up the playlist

It also has the following methods:

addSong(song) : adds a Song object to the songs arrayremoveSong(song) : removes a Song object from the songs array

MusicPlayer class

The MusicPlayer class represents a music player and has the following properties:

playlist (a Playlist object): the playlist the player is currently usingcurrentSongIndex (integer): the index of the currently playing song in the playlistisPlaying (boolean): whether the player is currently playing a song or notcurrentSong (a Song object): the currently playing song

It also has the following methods:

play() : starts playing the current songpause() : pauses the current songnext() : skips to the next song in the playliststop() : stops playing the current song

Usage

Create Song objects with the title, artist, album, duration, and URL of the song.Create a Playlist object with a name and an array of Song objects.Create a MusicPlayer object with the Playlist object created in step 2.Call the play() method on the MusicPlayer object to start playing the first song in the playlist.Call the next() method to skip to the next song in the playlist.Call the pause() method to pause the current song.Call the stop() method to stop playing the current song.

Note: This code only supports playing a single playlist at a time. If you want to support multiple playlists, you will need to modify the MusicPlayer class to handle this.

