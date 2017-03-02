#Investigation in to Maze solving in JS#

index.html
-

index.html loads tiny.png 10x10 pixel maze  

getImageData produces a RGBA array  
black is 0,0,0,255 and white is 255,255,255,255   
R = G = B so only Red is read    
RGBA means length / 4 and i*4   
if 0 i.e. black pixel found then use fillRect() 
mod (%) used to go to next row  

debug.html
-

Zooming PNG is Blurry   
Following lines have been commented out in favour of redraw    
canvas set to image size    
zoom image to fit window height   
getImageData doesn't work after scale hence draw before and after scale 

pixels2Console() = pixels2Array() & array2Console()  
pixels2Array creates a simplified (getImageData) array, may be redundant  


References
-

https://preview.c9users.io/en10/maze/index.html

https://www.youtube.com/watch?v=rop0W4QDOUI

https://github.com/mikepound/mazesolving

https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Pixel_manipulation_with_canvas