group together many variables into 1 variable with sub variable's

```js
function setup() {
  createCanvas(400, 400);
}


function draw() {
  background(220);
  
  let fatty = new Fatty(0, 0);
  fatty.drawFatty();
}


class Fatty {
  constructor(x, y) {
    this.xPos = x;
    this.yPos = y;
    
    this.yVelocity = 0;
    this.xVelocity = 0;
  }
  
  drawFatty() {
    // body
    fill(240, 240, 0);
    ellipse(200 + this.xPos, 200 + this.yPos, 90, 90);

    // eye
    fill(255, 255, 255);
    ellipse(230 + this.xPos, 185 + this.yPos, 40, 40);

    // pupil
    fill(0);
    ellipse(240 + this.xPos, 185 + this.yPos, 15, 20);

    // wing
    fill(255, 255, 0);
    ellipse(170 + this.xPos, 200 + this.yPos, 50, 40);

    // lips
    fill(255, 0, 0);
    ellipse(230 + this.xPos, 220 + this.yPos, 40, 30);
  }
}
```