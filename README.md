<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Random Task Generator</title>
    <style>
        body {
            font-family: 'Arial', sans-serif;
            text-align: center;
            margin: 50px;
        }
        button {
            padding: 10px 20px;
            font-size: 16px;
            margin-bottom: 20px;
        }
        #task-display {
            font-size: 18px;
            margin-top: 20px;
        }
    </style>
</head>
<body>
    <h1>Random Task Generator</h1>
    <button onclick="generateRandomTask()">Generate Task</button>
    <div id="task-display"></div>

    <script>
        const taskCategories = {
            work: ["Complete a small work task.", "Organize your workspace.", "Write down your goals for the day."],
            selfCare: ["Take a 10-minute break.", "Practice deep breathing.", "Stretch your muscles."],
            fitness: ["Go for a 15-minute walk.", "Do 10 push-ups.", "Try a quick yoga session."],
            creativity: ["Draw something for 5 minutes.", "Write a short poem.", "Start a small DIY project."],
            relaxation: ["Read a chapter of a book.", "Listen to calming music.", "Take a power nap."],
        };

        function generateRandomTask() {
            const categories = Object.keys(taskCategories);
            const randomCategory = categories[Math.floor(Math.random() * categories.length)];
            const tasksInCategory = taskCategories[randomCategory];
            const randomTask = tasksInCategory[Math.floor(Math.random() * tasksInCategory.length)];

            displayTask(randomTask);
        }

        function displayTask(task) {
            const taskDisplay = document.getElementById('task-display');
            taskDisplay.textContent = `Task: ${task}`;
        }
    </script>
</body>
</html>
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Random Task Generator</title>
    <style>
        body {
            font-family: 'Arial', sans-serif;
            text-align: center;
            margin: 50px;
        }
        button {
            padding: 10px 20px;
            font-size: 16px;
            margin-bottom: 20px;
        }
        #task-display {
            font-size: 18px;
            margin-top: 20px;
        }
    </style>
</head>
<body>
    <h1>Random Task Generator</h1>
    <button onclick="generateRandomTask()">Generate Task</button>
    <div id="task-display"></div>

    <script>
        const taskCategories = {
            work: ["Complete a small work task.", "Organize your workspace.", "Write down your goals for the day."],
            selfCare: ["Take a 10-minute break.", "Practice deep breathing.", "Stretch your muscles."],
            fitness: ["Go for a 15-minute walk.", "Do 10 push-ups.", "Try a quick yoga session."],
            creativity: ["Draw something for 5 minutes.", "Write a short poem.", "Start a small DIY project."],
            relaxation: ["Read a chapter of a book.", "Listen to calming music.", "Take a power nap."],
        };

        function generateRandomTask() {
            const categories = Object.keys(taskCategories);
            const randomCategory = categories[Math.floor(Math.random() * categories.length)];
            const tasksInCategory = taskCategories[randomCategory];
            const randomTask = tasksInCategory[Math.floor(Math.random() * tasksInCategory.length)];

            displayTask(randomTask);
        }

        function displayTask(task) {
            const taskDisplay = document.getElementById('task-display');
            taskDisplay.textContent = `Task: ${task}`;
        }
    </script>
</body>
</html>
