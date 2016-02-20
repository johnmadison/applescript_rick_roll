1. Install "Play Sound" from here: goo.gl/V0XHbN

2. Open Up "Applescript Editor" (every mac has it by default)

3. Copy and Paste the Following Into the editor:

tell application "Play Sound"

activate

--here is where we load in all of our 13 chromatic notes
-- "x" means sharp since # and as are reserved
set a to ((path to me as text) & "Contents:A.wav") as alias
set ax to ((path to me as text) & "Contents:A#.wav") as alias
set b to ((path to me as text) & "Contents:B.wav") as alias
set c to ((path to me as text) & "Contents:C.wav") as alias
set c2 to ((path to me as text) & "Contents:C2.wav") as alias
set cx to ((path to me as text) & "Contents:C#.wav") as alias
set d to ((path to me as text) & "Contents:D.wav") as alias
set dx to ((path to me as text) & "Contents:D#.wav") as alias
set e to ((path to me as text) & "Contents:E.wav") as alias
set f to ((path to me as text) & "Contents:F.wav") as alias
set fx to ((path to me as text) & "Contents:F#.wav") as alias
set g to ((path to me as text) & "Contents:G.wav") as alias
set gx to ((path to me as text) & "Contents:G#.wav") as alias

set k to ((path to me as text) & "Contents:kick.wav") as alias
set s to ((path to me as text) & "Contents:snare.wav") as alias

--then we open up "Play Sound" NOTE: make sure to install Play Sound

tell application "Play Sound"
--heres where you can write the music
play a

end tell
quit "Play Sound"
end tell

step 4:

Click compile and save it as an application. Right click on where you saved it and open the package contents. Inside the folder named "Contents" put your desired samples.

Once you've added enough sounds you should be able to make some sounds happening by typing "play a" or whatever note or sound you've loaded.