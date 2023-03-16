![video]()

make a function to group together all the drawing functions (`ellipse` and `fill`'s) into 1 reusable function

```js
var xPosition = -200;
var yPosition = 0;

function setup() {
  createCanvas(400, 400);
}

function draw() {
  background(220);
  
  drawFatty(xPosition, yPosition);

  xPosition = xPosition + 1;
}

function drawFatty(xPos, yPos) {
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
}
```