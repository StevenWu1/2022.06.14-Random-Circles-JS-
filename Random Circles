const cx = 600;
const cy = 600;
let circleMin = 50;
let circleMax = 300;

function setup() {
  createCanvas(cx, cy);
  frameRate(2);
}

let circleCount = 0;

function draw() {
  background("rgba(0, 0, 0, 0.7)");
  NumOfCircleDraw(10);
  circleCount = circleCount + 1;
}

function randomColor() {
  const r = round(random(0, 256));
  const g = round(random(0, 256));
  const b = round(random(0, 256));
  const c = color(r, g, b);
  console.log(c);
  return c;
}

function randomCircle() {
  fill(randomColor());
  let d = random(circleMin, circleMax);
  let x = random(d/2, cx - d/2);
  let y = random(d/2, cy - d/2);
  circle(x, y, d);
}

function NumOfCircleDraw(num) {
  if (num > 0) {
    randomCircle();
    NumOfCircleDraw(num-1);
  }
}
