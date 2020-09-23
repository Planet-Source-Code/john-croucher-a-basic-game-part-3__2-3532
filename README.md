<div align="center">

## A Basic Game \- Part 3


</div>

### Description

This is the 3rd section of my Basic Game Tutorial. This part shows how to put graphics into the game.
 
### More Info
 


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[John Croucher](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/john-croucher.md)
**Level**          |Beginner
**User Rating**    |4.3 (39 globes from 9 users)
**Compatibility**  |Java \(JDK 1\.2\)
**Category**       |[Games](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/games__2-72.md)
**World**          |[Java](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/java.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/john-croucher-a-basic-game-part-3__2-3532/archive/master.zip)





### Source Code

<CENTER></FONT>
<H1><font color="#0000CD">Java Game Tutorial - Part 3 </Font></H1>
</Center>
<font color="#000000" face="Comic Sans MS" size="2">
<BR>This tutorial is a small add on to part 2 of my Java Game Tutorial. I have had many requests by people for this so I finally decided to put this part 3 of my Java Game Tutorial together.
<BR>In this tutorial you will see how to change from using those boring shapes to using images.
<BR>
<BR>The first thing you will need is two 20x20 pixel gif or jpeg image. If you are using gif you must make sure you save it as 8bit Paletted. I have sometimes had problems if this is not done.
<BR>One image will be the alien type characters. I have smiley faces in my game.
<BR>Also you will need some sort of ship which does the shooting down the bottom.
<BR>These can be animated gif images if you would like to add some extra effect to them.
<BR>
<BR>Now to the coding
<BR>This is very simple and will not take very long at all.
<BR>
<BR>In the global variable section place the following:
</FONT><font color="#0000CD" face="Comic Sans MS" size="2">
<BR>      Image alien;
<BR>      Image ship;
<BR>
</FONT><font color="#000000" face="Comic Sans MS" size="2">
<BR>This will set up two image objects to store out images.
<BR>
<BR>Next is in the “public void init()” function. Place in the following code.
<BR>
</FONT><font color="#0000CD" face="Comic Sans MS" size="2">
<BR>      alien = getImage(getDocumentBase(), "img1.gif");
<BR>      ship = getImage(getDocumentBase(), "img2.gif");
<BR>
</FONT><font color="#000000" face="Comic Sans MS" size="2">
<BR>This will load the image files into the Image objects.
<BR>
<BR>The final part is to then draw the images to our buffer.
<BR>
<BR>The first one to draw are the aliens
<BR>We are currently drawing them with this line:
<BR>
</FONT><font color="#0000CD" face="Comic Sans MS" size="2">
<BR>      bufferdImgSurface.fillOval(currentX[i], currentY[i], 20,20);
<BR>
</FONT><font color="#000000" face="Comic Sans MS" size="2">
<BR>Replace that line with this line
<BR>
</FONT><font color="#0000CD" face="Comic Sans MS" size="2">
<BR>      bufferdImgSurface.drawImage(alien, currentX[i], currentY[i], this);
<BR>
</FONT><font color="#000000" face="Comic Sans MS" size="2">
<BR>This draws the image ‘alien’ to the current position in the buffer.
<BR>The same goes for the ship.
<BR>
<BR>Replace this line:
<BR>
</FONT><font color="#0000CD" face="Comic Sans MS" size="2">
<BR>      bufferdImgSurface.fillRect(shipX, shipY, 20, 20);
<BR>
</FONT><font color="#000000" face="Comic Sans MS" size="2">
<BR>With this line:
<BR>
</FONT><font color="#0000CD" face="Comic Sans MS" size="2">
<BR>      bufferdImgSurface.drawImage(ship, shipX, shipY, this);
<BR>
</FONT><font color="#000000" face="Comic Sans MS" size="2">
<BR>You should now be able to compile this code and run it. If you have any errors such as getting a white or grey java frame then check your paths for your images. Make sure they are in the same directory with your class file. You can put paths in if you want by doing the following.
<BR>
</FONT><font color="#0000CD" face="Comic Sans MS" size="2">
<BR>      alien = getImage(getDocumentBase(), "folder1/folder2/img1.gif");
<BR>
</FONT><font color="#000000" face="Comic Sans MS" size="2">
<BR>That is the end of my third tutorial for making games in Java.
<BR>I hope you like my tutorial. If you find any errors please email me, also if you have any comments please email me.
<BR>
<BR>Also if you have something you think I could put in a future tutorial like multi player or networking email me.
<BR> If you would like to see a working version go here http://www.jcroucher.com/javatutg3.html <BR>*Note: This tutorial has been compiled and tested with J2sdk 1.4.0_01 attempting to run or use this tutorial without this version JSDK or JRE can have bad effects. Use these at your own risk*
<BR>
<BR>Also check out my website for more tutorials and code samples www.jcroucher.com
<BR>
<BR>This code and tutorial is copyright 2003 John Croucher.
<BR>
<BR>
</Font>

