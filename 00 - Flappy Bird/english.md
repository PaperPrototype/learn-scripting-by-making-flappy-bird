Are you a complete beginner? You probably SUCK at coding... well, so did I. 

In this guide I'm going to teach how to code by making a derailed flappy bird! Are you ready?!

![]()

Here is the final code for drawing Mr. Fatty Bird (that's what I'm calling him from now on).

```js
function setup() {
    createCanvas(400, 400);
}

function draw() {
    background(220);

    // body
    fill(240, 240, 0);
    ellipse(200, 200, 90, 90); 
    
    // eye 
    fill(255, 255, 255); 
    ellipse(230, 185, 40, 40);
    
    // pupil
    fill(0);
    ellipse(240, 185, 15, 20);
    
    // wing
    fill(255, 255, 0);
    ellipse(170, 200, 50, 40);
    
    // lips
    fill(255, 0, 0);
    ellipse(230, 220, 40, 30);
}
```