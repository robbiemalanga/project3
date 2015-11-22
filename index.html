<!doctype html>
<html>
<head>
<style>
h1   {font-size:30px;
		color:#6600FF;
		text-align:center;
		font-family: Arial, Helvetica, sans-serif;}
</style>
<title>Canvas</title>
<script>
    window.onload = function() {

      var canvas = document.createElement("canvas");
      var context = canvas.getContext("2d");
      canvas.width = window.innerWidth * 0.9;
      canvas.height = window.innerHeight * 0.9;
      document.body.appendChild(canvas);

      var posX = 50,
      posY = canvas.height / 2;

	  var num2=Math.floor((Math.random() * 20) + 1);

      var particles = {},
          particleIndex = 0,
          settings = {
            density: 1,
            particleSize: num2,
            particleSize2: 20,
            startingX: canvas.width / 2,
            startingY: canvas.height / 4,
            gravity: 0.1,
            maxLife: 300,
            groundLevel: canvas.height,
            leftWall: canvas.width * 0.1,
            rightWall: canvas.width
          };
          
      var seedsX = [];
      var seedsY = [];
      var maxAngles = 100;
      var currentAngle = 0;

      function seedAngles() {
        seedsX = [];
        seedsY = [];
        for (var i = 0; i < maxAngles; i++) {
          seedsX.push(Math.random() * 20 - 10);
          seedsY.push(Math.random() * 30 - 10);
        }
      }
      seedAngles();

      function Particle() {
        if (currentAngle !== maxAngles) {
          this.x = settings.startingX;
          this.y = settings.startingY;
          this.vx = seedsX[currentAngle];
          this.vy = seedsY[currentAngle];
          currentAngle++;

          particleIndex ++;
          particles[particleIndex] = this;
          this.id = particleIndex;
          this.life = 0;
          this.maxLife = settings.maxLife;

          seedAngles();
          currentAngle = 0;
        }
      }

      Particle.prototype.draw = function() {
        this.x += this.vx;
        this.y += this.vy;
        
        if ((this.y + settings.particleSize) > settings.groundLevel) {
          this.vy *= -0.6;
          this.vx *= 0.75;
          this.y = settings.groundLevel - settings.particleSize;
        }

        if (this.x - (settings.particleSize) <= settings.leftWall) {
          this.vx *= -1;
          this.x = settings.leftWall + (settings.particleSize);
        }

        if (this.x + (settings.particleSize) >= settings.rightWall) {
          this.vx *= -1;
          this.x = settings.rightWall - settings.particleSize;
        }
        this.vy += settings.gravity;
        this.life++;

        if (this.life >= this.maxLife) {
          delete particles[this.id];
        }


        context.fillStyle = "#6600FF";
        context.fillRect(this.x, this.y, 20, 20);
        context.clearRect(settings.leftWall, settings.groundLevel, canvas.width, canvas.height);
        context.beginPath();
        context.fillStyle="#6600FF";

        context.arc(this.x, this.y, settings.particleSize, 0, Math.PI*2, true); 
        context.closePath();
        context.fill();
        
        
        context.beginPath();
        context.moveTo(170, 80);
        context.bezierCurveTo(130, 100, 130, 150, 230, 150);
        context.bezierCurveTo(250, 180, 320, 180, 340, 150);
        context.bezierCurveTo(420, 150, 420, 120, 390, 100);
        context.bezierCurveTo(430, 40, 370, 30, 340, 50);
        context.bezierCurveTo(320, 5, 250, 20, 250, 50);
        context.bezierCurveTo(200, 5, 150, 20, 170, 80);
        context.closePath();
        context.lineWidth = 5;
        context.strokeStyle = 'white';
        context.stroke();
        }

      setInterval(function() {
        context.fillStyle = "rgba(10,10,10,0.8)";
        context.fillRect(0, 0, canvas.width, canvas.height);

        context.fillStyle = "white";
        context.fillRect(0, 0, settings.leftWall, canvas.height);
        context.fillRect(settings.rightWall, 0, canvas.width, canvas.height);
        context.fillRect(0, settings.groundLevel, canvas.width, canvas.height);

        // Draw the particles
        for (var i = 0; i < settings.density; i++) {
          new Particle();
        }

        for (var i in particles) {
          particles[i].draw();
        }
      }, 30);

    };
</script>
</head>
<body>
<h1 id="fade">RANDOM SIZED FALLING SHAPES</h1>
</body>	  
</html>
