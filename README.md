# Html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>STEM Feedback Portal</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <!-- Navigation Bar -->
    <nav>
        <ul>
            <li><a href="#">Home</a></li>
            <li><a href="#feedback">Give Feedback</a></li>
            <li><a href="#learn">Learn</a></li>
            <li><a href="#stories">Success Stories</a></li>
            <li><a href="#timer">Study Timer</a></li>
            <li><a href="#teachers">Teachers' Ideas</a></li>
            <li><a href="#insights">Government Insights</a></li>
        </ul>
    </nav>

    <!-- Homepage Intro -->
    <section id="home">
        <h1>Welcome to the STEM Feedback Portal</h1>
        <p>Share your feedback and find helpful resources to enhance your STEM learning experience.</p>
        <button onclick="scrollToSection('feedback')">Share Your Feedback</button>
        <button onclick="scrollToSection('learn')">Find Helpful Resources</button>
    </section>

    <!-- Feedback Section -->
    <section id="feedback">
        <h2>Give Feedback</h2>
        <form id="feedbackForm">
            <label for="experience">Rate your experience:</label>
            <select id="experience">
                <option value="positive">Positive</option>
                <option value="negative">Negative</option>
            </select>

            <div id="difficultyReason" style="display:none;">
                <label for="difficulty">What is the reason?</label>
                <select id="difficulty">
                    <option value="difficulty">Subject Difficulty</option>
                    <option value="resources">Lack of Resources</option>
                    <option value="other">Other</option>
                </select>

                <div id="weaknessForm" style="display:none;">
                    <label for="subject">What subject are you struggling with?</label>
                    <select id="subject">
                        <option value="math">Math</option>
                        <option value="physics">Physics</option>
                        <option value="biology">Biology</option>
                        <option value="chemistry">Chemistry</option>
                    </select>
                </div>
            </div>
            <button type="submit">Submit Feedback</button>
        </form>
    </section>

    <!-- Video Library Section -->
    <section id="learn">
        <h2>Learn</h2>
        <p>We provide curated videos to help you improve your skills in various STEM subjects.</p>
        <div id="videoLibrary">
            <!-- Dynamically suggested videos will go here -->
        </div>
    </section>

    <!-- Success Stories Section -->
    <section id="stories">
        <h2>Success Stories</h2>
        <p>Read success stories from students who have overcome challenges in STEM education.</p>
    </section>

    <!-- Study Timer Section -->
    <section id="timer">
        <h2>Study Timer</h2>
        <button onclick="startTimer(30)">Start 30-Minute Timer</button>
        <button onclick="startTimer(60)">Start 1-Hour Timer</button>
        <p id="timerDisplay"></p>
    </section>

    <!-- Teachers' Ideas Section -->
    <section id="teachers">
        <h2>Teachers' Ideas</h2>
        <p>Teachers can share their ideas for improving STEM education here.</p>
    </section>

    <!-- Government Insights Section -->
    <section id="insights">
        <h2>Government Insights</h2>
        <p>The Department of Education can track data to improve the STEM curriculum.</p>
    </section>

    <script src="script.js"></script>
</body>
</html>
