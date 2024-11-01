<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Quiz Game</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <div class="quiz-container">
        <!-- Real-time Score Display -->
        <div id="score-bar">
            Score: <span id="current-score">0</span>
        </div>

        <h1>Quiz Game</h1>
        
        <!-- Quiz Level Selection -->
        <div id="level-selection">
            <h2>Select your level</h2>
            <button class="level-button" onclick="startQuiz('std10')">Standard 10</button>
            <button class="level-button" onclick="startQuiz('std11')">Standard 11 (JEE Mains & Advanced)</button>
            <button class="level-button" onclick="startQuiz('std12')">Standard 12 (JEE Mains & Advanced)</button>
        </div>
        
        <!-- Quiz Content -->
        <div id="quiz-content" style="display: none;">
            <p id="question"></p>
            <div id="options"></div>
            <button class="submit-button" onclick="submitAnswer()">Submit Answer</button>
        </div>
        
        <!-- Result Display -->
        <div id="result" style="display: none;">
            <h2>Quiz Completed</h2>
            <p id="final-score"></p>
            <button class="reset-button" onclick="resetQuiz()">Try Again</button>
        </div>

        <!-- Footer Line -->
        <footer>
            <p>This app developed by Bhavy Lukhi</p>
        </footer>
    </div>

    <script src="script.js"></script>
</body>
</html>

