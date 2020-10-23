# WEEK FOUR 
![180719110858-01-file-2000s-restricted-super-tease](https://user-images.githubusercontent.com/68723190/96998718-b1072f00-157f-11eb-93a4-4b6c28ffa32f.jpg)

## IN CLASS ACTIVITY 
Today's class saw us continue our experimentations on processing.
<img width="1680" alt="Screen Shot 2020-08-14 at 11 16 12 am" src="https://user-images.githubusercontent.com/68723190/96999692-5242b500-1581-11eb-94a0-9d4ad17c55a4.png">


[firend.mp4.zip](https://github.com/mabryson/slavetoalg/files/5429208/firend.mp4.zip)



### CODE: 
//sketch 14th august 2020
PImage photo;
int smallPoint, largePoint, x,y,dotSize,t;
color pix;
float pointillise;
void setup(){
size(1000,1000);
background (255);
imageMode(CENTER);
photo = loadImage("yeehaw1.jpg");
smallPoint=5;
largePoint=50;
frameRate(60);
}

void draw(){
//image (photo,240,240); //this loads the image to fill the sketch
x=int(random(photo.width)); // finds random() point across the sketch (x)
y=int(random(photo.height)); 
pointillise =map(mouseX, 0, width, smallPoint, largePoint); //map (input, lowest value in, highest value in, lowest value out, highest value out)
dotSize=int(pointillise);
pix=photo.get(x,y); //this gets the color value from where my mouse is
t=int(random(256));
strokeWeight(3);
//stroke (pix,t); // this updates the color of the fill() to the pixel values
fill(pix,t); 
noStroke(); // this removes the outline of the circle 
ellipse (x,y,dotSize,dotSize);
//line(x,y,x+dotSize,y+dotSize); // this draws the lines
}
## thought this processing sketch was cool 
https://www.openprocessing.org/sketch/838545
