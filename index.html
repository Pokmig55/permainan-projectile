<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Projectile Motion Simulation</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            margin: 0;
            padding: 0;
        }

        canvas {
            border: 1px solid black;
            display: block;
            margin: 20px auto;
        }

        #controls {
            margin: 10px 0;
        }

        input[type="range"] {
            margin: 0 10px;
        }
    </style>
</head>
<body>
    <h1>Projectile Motion Simulation</h1>
    <div id="controls">
        <label for="angle">Angle (degrees): </label>
        <input type="range" id="angle" min="0" max="90" value="45"> <span id="angleValue">45</span>
        <br>
        <label for="velocity">Initial Velocity (m/s): </label>
        <input type="range" id="velocity" min="10" max="100" value="50"> <span id="velocityValue">50</span>
        <br>
        <button id="launch">Launch</button>
    </div>
    <canvas id="simulationCanvas" width="800" height="400"></canvas>

    <script>
        const canvas = document.getElementById("simulationCanvas");
        const ctx = canvas.getContext("2d");

        const angleInput = document.getElementById("angle");
        const velocityInput = document.getElementById("velocity");
        const angleValue = document.getElementById("angleValue");
        const velocityValue = document.getElementById("velocityValue");
        const launchButton = document.getElementById("launch");

        angleInput.addEventListener("input", () => {
            angleValue.textContent = angleInput.value;
        });

        velocityInput.addEventListener("input", () => {
            velocityValue.textContent = velocityInput.value;
        });

        let projectile = {
            x: 0,
            y: canvas.height,
            vx: 0,
            vy: 0,
            launched: false
        };

        const gravity = 9.8;
        let time = 0;

        function drawGround() {
            ctx.fillStyle = "green";
            ctx.fillRect(0, canvas.height - 10, canvas.width, 10);
        }

        function drawProjectile() {
            ctx.beginPath();
            ctx.arc(projectile.x, projectile.y, 5, 0, Math.PI * 2);
            ctx.fillStyle = "red";
            ctx.fill();
        }

        function resetCanvas() {
            ctx.clearRect(0, 0, canvas.width, canvas.height);
        }

        function updateProjectile() {
            if (!projectile.launched) return;

            time += 0.05;
            projectile.x = projectile.vx * time;
            projectile.y = canvas.height - (projectile.vy * time - 0.5 * gravity * time * time);

            if (projectile.y >= canvas.height) {
                projectile.launched = false;
            }
        }

        function render() {
            resetCanvas();
            drawGround();
            drawProjectile();
        }

        function gameLoop() {
            updateProjectile();
            render();
            requestAnimationFrame(gameLoop);
        }

        launchButton.addEventListener("click", () => {
            const angle = parseFloat(angleInput.value) * (Math.PI / 180);
            const velocity = parseFloat(velocityInput.value);

            projectile.x = 0;
            projectile.y = canvas.height;
            projectile.vx = velocity * Math.cos(angle);
            projectile.vy = velocity * Math.sin(angle);
            projectile.launched = true;
            time = 0;
        });

        gameLoop();
    </script>
</body>
</html>
