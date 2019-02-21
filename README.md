# Jukebox
A music player

Basically, the Jukebox is itself an object. The cover is the play and pasue button. When the song is playing, the cover picture will spin. When the song is paused, the cover picture will stop spinning. The other buttons include before, next, shuffle, and stop. When the song is stopped, the song will reload and cover will return to original position. The playlist is clickable and it will hightlight the current song you are playing with light blue.

When the user open the page, the setup() method is called immediately. It will establish the playlist, load the song, and setup the functions of the buttons. The functions of buttons of the Jukebox are class methods. Next corresponds to toNext() method, Before corresponds to toBefore() method, shuffle corresponds to shuffle() method, stop corresponds to stop() method, and play and pause button corresponds to play() method. Each time these methods are called will call the update() and updateList() methods, which will update the information of song and the playlist.

For the play list, I put a method outside of the object because I need to access the event object, which affects the scope of this inside the object. I haven't thought of any great way to improve this problem. Eventually, I want to incoporate the click method also inside the object instead of outside in the global scope.
