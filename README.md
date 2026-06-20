# Motivational-Quotes-
A brief quote
<!DOCTYPE html>
<html>
<head> <style>
    body {
        font-family: Arial, sans-serif;
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        min-height: 100vh;
        background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
        color: white;
        margin: 0;
    }
    h1 { font-size: 2.5em; margin-bottom: 20px; }
    p { font-size: 1.2em; margin-bottom: 20px; }
    button {
        padding: 12px 30px;
        font-size: 1em;
        background-color: #ff6b6b;
        color: white;
        border: none;
        border-radius: 5px;
        cursor: pointer;
        transition: background-color 0.3s;
    }
    button:hover { background-color: #ff5252; }
    #quote {
        font-size: 1.5em;
        font-style: italic;
        text-align: center;
        max-width: 600px;
        margin-top: 30px;
        padding: 20px;
        background: rgba(255, 255, 255, 0.1);
        border-radius: 10px;
        min-height: 80px;
        display: flex;
        align-items: center;
    }
  </style>
    <title>Motivational Quote Generator</title>
</head>
<body>
    <h1>✨ Motivational Quote Generator ✨</h1>

    <p>Click the button for motivation!</p>

    <button onclick="showQuote()">Show Quote</button>

    <h2 id="quote"></h2>

    <script>
        const quotes = [
            "Believe in yourself and all that you are.",
            "Success begins with a single step.",
            "Your future is created by what you do today.",
            "Dream big, work hard, stay focused.",
            "Every expert was once a beginner.",
            "Don't watch the clock; do what it does. Keep going.",
            "Small progress is still progress.",
            "The best way to predict the future is to create it.",
            "You are stronger than you think.",
            "Never give up on a dream because of the time it will take."
        ];

        function showQuote() {
            const randomIndex = Math.floor(Math.random() * quotes.length);
            document.getElementById("quote").innerText = quotes[randomIndex];
        }
    </script>
</body>
</html>
