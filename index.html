<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Snake Game</title>
    <style>
        canvas {
            display: block;
            margin: auto;
            background-color: #f0f0f0;
            border: 1px solid black;
        }
    </style>
</head>
<body>
    <canvas id="gameCanvas" width="400" height="400"></canvas>
    <script>
        const canvas = document.getElementById('gameCanvas');
        const ctx = canvas.getContext('2d');

        const gridSize = 20;
        const tileCount = canvas.width / gridSize;

        let snake = [{ x: 10, y: 10 }];
        let food = { x: 5, y: 5 };
        let direction = { x: 0, y: 0 };
        let score = 0;

        function gameLoop() {
            update();
            draw();
            setTimeout(gameLoop, 100);
        }

        function update() {
            const head = { x: snake[0].x + direction.x, y: snake[0].y + direction.y };

            // Check for collisions
            if (
                head.x < 0 || head.x >= tileCount ||
                head.y < 0 || head.y >= tileCount ||
                snake.some(segment => segment.x === head.x && segment.y === head.y)
            ) {
                resetGame();
                return;
            }

            snake.unshift(head);

            // Check if food is eaten
            if (head.x === food.x && head.y === food.y) {
                score++;
                placeFood();
            } else {
                snake.pop();
            }
        }

        function draw() {
            ctx.clearRect(0, 0, canvas.width, canvas.height);

            // Draw snake
            ctx.fillStyle = 'green';
            snake.forEach(segment => ctx.fillRect(segment.x * gridSize, segment.y * gridSize, gridSize, gridSize));

            // Draw food
            ctx.fillStyle = 'red';
            ctx.fillRect(food.x * gridSize, food.y * gridSize, gridSize, gridSize);

            // Draw score
            ctx.fillStyle = 'black';
            ctx.font = '20px Arial';
            ctx.fillText(`Score: ${score}`, 10, 20);
        }

        function placeFood() {
            food.x = Math.floor(Math.random() * tileCount);
            food.y = Math.floor(Math.random() * tileCount);

            // Ensure food doesn't spawn on the snake
            while (snake.some(segment => segment.x === food.x && segment.y === food.y)) {
                food.x = Math.floor(Math.random() * tileCount);
                food.y = Math.floor(Math.random() * tileCount);
            }
        }

        function resetGame() {
            snake = [{ x: 10, y: 10 }];
            direction = { x: 0, y: 0 };
            score = 0;
            placeFood();
        }

        window.addEventListener('keydown', event => {
            switch (event.key) {
                case 'ArrowUp': if (direction.y === 0) direction = { x: 0, y: -1 }; break;
                case 'ArrowDown': if (direction.y === 0) direction = { x: 0, y: 1 }; break;
                case 'ArrowLeft': if (direction.x === 0) direction = { x: -1, y: 0 }; break;
                case 'ArrowRight': if (direction.x === 0) direction = { x: 1, y: 0 }; break;
            }
        });

        placeFood();
        gameLoop();
    </script>
</body>
</html>
