use xPosition and yPosition variables to decide where to put Mr. Flappy on the screen

in draw increase the xPosition to make Mr. Fatty move across the screen!

```js
var xPos = -200;
var yPos = 0;

function setup() {
    createCanvas(400, 400);
}

function draw() {
    background(220);

    // body
    fill(240, 240, 0);
    ellipse(200 + xPos, 200 + yPos, 90, 90); 
    
    // eye 
    fill(255, 255, 255); 
    ellipse(230 + xPos, 185 + yPos, 40, 40);
    
    // pupil
    fill(0);
    ellipse(240 + xPos, 185 + yPos, 15, 20);
    
    // wing
    fill(255, 255, 0);
    ellipse(170 + xPos, 200 + yPos, 50, 40);
    
    // lips
    fill(255, 0, 0);
    ellipse(230 + xPos, 220 + yPos, 40, 30);
  
    xPos = xPos + 1;
}
```