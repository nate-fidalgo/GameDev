The stereo_surround.wav and stereo_surround.mp3 files are to test the illusion of 3d and surround sound like effects thru 2 channel stereo tricks.<br>
By using the pan all the way to the left for one channel and pan all the way to the right for the other channel you can achieve cool SFX coming from different speakers.<br>
Check it out download the files and listen  with two speakers or headphones!!!<br>
If you want to do the same one can use audicity or any decent audio editing software to achieve this thru creating two mono channels then merging them into stereo with pan to the left 
on one channel and pan to the right on the other channel <br>

<br>
Also wav files and mp3 are really container files that support compression as well like older but still very good in certain cases RLE (run length encoding) , a-law, mu-law ,...etc.
<br>
However most people as well as me have been fooled by everybody saying this is a audio file format , or a video file format...etc usually everything is in a container file that support
either 1 or more channels/sections of data having header fields that tell it what compression algorithm to encode/decode channels with.<br>
In the case of wav files its normally an uncompressed container file that just points to the raw linear PCM data that is usually 16bit 44khz endian little.<br>
In the case of mp3 files it normally is a container file format that has a lossy compression algorithm though one can support many different compression algorithms with a container 
file format <br>

<br>
So dont let the extensions fool you most of the time there all container file formats just with different extensions the extension sometimes are important though because the players
check the extensions to know what container file format there dealing with so they know how to parse the header sections.<br>
This is important for the player to figure out the codec it needs to uses and where the channel data is for each channel if it has multiple channels amongs other fields and features.
<br>

What differs from container files for video vs audio is that audio container files sometimes only have the capacity to store audio channel data not a good quality video channel.
<br>
And container file formats for video support usually multiple audio channels as well as multiple video channels its the images/quality of image data that wouldn't work well in a mp3 vs mp4.
<br>
Yet a mp4 could be used as a container for just audio file or just video making it really a file format for audio like an mp3 as well as a video file format like avi.
<br>

I hope i am not confusing the issue but there is really no such thing as audio file format and video file format but more container files used as audio storing only files or
video storing files.
<br>
<br>
We usually call the extensions of wav ,mp3,... an audio file format<br>
And m4k, avi ,mov ,mp4 ,mpeg,...etc an video file format <br>
However truely its all just container file formats which some support just audio , just video , multiple track audio ,....etc all depends on the header fields /file format choosen.
<br>
Goes container file ---> inside it fields telling the properties of all the channels/where they are in file (the compression algorithm/pointer to channel data)----> then its just 
the chuncks of channel data. Some times also called as streams, tracks  ,...etc

<br>
<br>
The more complicated aspect of these video /audio/container file formats is the compression/decompression algorithms choosen for each channel. <br>
Some people call them codec others call them encoding/decoders. Some codec even use encryption as well. <br>
While understanding LZ77 , LZW , LZxxx and all its variants like DEFLATE , what png uses , ...etc is pretty straight forward at a high level<br>
Basically associating <pointers | character length> to beable to just store pointers back to already seen data is the main trick for all of these variants. <br>
Its just the way they do it as well as what they choose for the pointer length vs the character length. A common choice is 10 bit address to 6 bit char length. <br>
<br>
Anyway compression/decompression algorithms i will be make a seperate code theory/information theory folder for this.
<br>
<br>
To sum up container files is everything audio file formats or video file formats are just a certain type of container file formats.<br>
So when we say audio file format or video file format for a given audio or video file extension we are just trying to figure out what the structure of that particular
<br> container file format is for that extension as well as what software can read/play/open it. <br>
Thats about it at the high level view :)
<br>
<br>
Enjoy the sample audio notice this effect is done in wav and mp3 both container formats for audio only. <br>
You could embedd very very shit quality of video images /thumbnail animation or stereographic data hiding <br>
After all there all just container file formats knowing this there like specific a folder of all the zip file channels interms of data compession zip files <br>
If your more familar with zip files / data compression for computer data :)
<br>
