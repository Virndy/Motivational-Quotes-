<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Random Fun Facts</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            min-height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            padding: 20px;
        }

        .container {
            background: white;
            border-radius: 15px;
            box-shadow: 0 10px 40px rgba(0, 0, 0, 0.2);
            padding: 40px;
            max-width: 600px;
            text-align: center;
        }

        h1 {
            color: #333;
            margin-bottom: 30px;
            font-size: 2.5em;
        }

        .fact-box {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
            padding: 30px;
            border-radius: 10px;
            margin-bottom: 30px;
            min-height: 150px;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 1.2em;
            line-height: 1.6;
            box-shadow: 0 5px 15px rgba(102, 126, 234, 0.4);
        }

        button {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
            border: none;
            padding: 15px 40px;
            font-size: 1.1em;
            border-radius: 50px;
            cursor: pointer;
            transition: transform 0.2s, box-shadow 0.2s;
            font-weight: bold;
        }

        button:hover {
            transform: translateY(-2px);
            box-shadow: 0 5px 20px rgba(102, 126, 234, 0.4);
        }

        button:active {
            transform: translateY(0);
        }

        .fact-counter {
            margin-top: 20px;
            color: #666;
            font-size: 0.9em;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>🎉 Fun Facts</h1>
        <div class="fact-box" id="factDisplay">
            Click the button to get a random fun fact!
        </div>
        <button onclick="getNewFact()">Get New Fact</button>
        <div class="fact-counter">
            Fact <span id="factCount">0</span> of <span id="totalFacts">0</span>
        </div>
    </div>

    <script>
        const facts = [
            "🐌 Snails have 14,000 teeth!",
            "🍯 Honey never spoils. Archaeologists have found 3,000-year-old honey in Egyptian tombs that was still edible.",
            "🧠 Your brain uses 20% of your body's energy, despite being only 2% of your body's weight.",
            "🦑 Octopuses have three hearts and blue blood!",
            "🌍 A day on Venus is longer than its year.",
            "👅 Your tongue has unique prints, just like your fingerprints.",
            "🦆 Ducks sleep with one eye open.",
            "☕ Caffeine takes 10 minutes to enter your bloodstream.",
            "🎸 A guitar string vibrates about 100 times per second.",
            "🐘 Elephants are the only animals that can recognize themselves in a mirror.",
            "🌙 The Moon is moving away from Earth at about 1.5 inches per year.",
            "🍕 Americans eat approximately 100 acres of pizza per day!",
            "🧲 Your body contains about 0.2% of the Earth's magnetic iron.",
            "🐦 Hummingbirds are the only birds that can fly backwards.",
            "🌟 Light from the Sun takes 8 minutes and 20 seconds to reach Earth."
        ];

        let currentFactIndex = 0;

        function getNewFact() {
            currentFactIndex = Math.floor(Math.random() * facts.length);
            document.getElementById('factDisplay').textContent = facts[currentFactIndex];
            document.getElementById('factCount').textContent = currentFactIndex + 1;
            document.getElementById('totalFacts').textContent = facts.length;
        }

        // Display first fact on page load
        window.addEventListener('load', getNewFact);
    </script>
</body>
</html>            font-size: 1.2em;
            line-height: 1.6;
            box-shadow: 0 5px 15px rgba(102, 126, 234, 0.4);
        }

        button {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
            border: none;
            padding: 15px 40px;
            font-size: 1.1em;
            border-radius: 50px;
            cursor: pointer;
            transition: transform 0.2s, box-shadow 0.2s;
            font-weight: bold;
        }

        button:hover {
            transform: translateY(-2px);
            box-shadow: 0 5px 20px rgba(102, 126, 234, 0.4);
        }

        button:active {
            transform: translateY(0);
        }

        .fact-counter {
            margin-top: 20px;
            color: #666;
            font-size: 0.9em;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>🎉 Fun Facts</h1>
        <div class="fact-box" id="factDisplay">
            Click the button to get a random fun fact!
        </div>
        <button onclick="getNewFact()">Get New Fact</button>
        <div class="fact-counter">
            Fact <span id="factCount">0</span> of <span id="totalFacts">0</span>
        </div>
    </div>

    <script>
        const facts = [
            "🐌 Snails have 14,000 teeth!",
            "🍯 Honey never spoils. Archaeologists have found 3,000-year-old honey in Egyptian tombs that was still edible.",
            "🧠 Your brain uses 20% of your body's energy, despite being only 2% of your body's weight.",
            "🦑 Octopuses have three hearts and blue blood!",
            "🌍 A day on Venus is longer than its year.",
            "👅 Your tongue has unique prints, just like your fingerprints.",
            "🦆 Ducks sleep with one eye open.",
            "☕ Caffeine takes 10 minutes to enter your bloodstream.",
            "🎸 A guitar string vibrates about 100 times per second.",
            "🐘 Elephants are the only animals that can recognize themselves in a mirror.",
            "🌙 The Moon is moving away from Earth at about 1.5 inches per year.",
            "🍕 Americans eat approximately 100 acres of pizza per day!",
            "🧲 Your body contains about 0.2% of the Earth's magnetic iron.",
            "🐦 Hummingbirds are the only birds that can fly backwards.",
            "🌟 Light from the Sun takes 8 minutes and 20 seconds to reach Earth."
        ];

        let currentFactIndex = 0;

        function getNewFact() {
            currentFactIndex = Math.floor(Math.random() * facts.length);
            document.getElementById('factDisplay').textContent = facts[currentFactIndex];
            document.getElementById('factCount').textContent = currentFactIndex + 1;
            document.getElementById('totalFacts').textContent = facts.length;
        }

        // Display first fact on page load
        window.addEventListener('load', getNewFact);
    </script>
</body>
</html>
