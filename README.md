GGMusic
============

GGMusic allows you to play a list of background music tracks in linear or random order in your Corona SDK powered apps.

Basic Usage
-------------------------

##### Require The Code
```lua
local GGMusic = require( "GGMusic" )
```

##### Create your music library
```lua
local music = GGMusic:new()
```

##### Add some tracks
```lua
music:add( "track1.mp3" ) -- An unnamed track.
music:add( "track2.mp3", "MainMenuMusic" ) -- A named track.
music:add( audio.loadStream( "track3.mp3" ), "Track3" ) -- A preloaded stream with a name.
```

##### Set the volume
```lua
music:setVolume( 0.8 )
```

##### Make it play!
```lua
music:play()
```

##### Control playback
```lua
music:stop() -- Stop the current track immediately.
music:play( "MainMenuMusic" ) -- Play the track named 'MainMenuMusic'.
music:next() -- Play the next track.
music:fadeOut( 1000 ) -- Fade out the current track over 1 second.
```

##### Add some randomness
```lua
music.random = true
```

Update History
-------------------------

##### 0.1
Initial release