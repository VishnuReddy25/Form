# Form
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Teacher Feedback Form</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f2f2f2;
            margin: 0;
            padding: 0;
        }

        .header {
            background-color: #4caf50;
            color: white;
            text-align: center;
            padding: 20px;
        }

        .feedback-form {
            background-color: #ffffff;
            padding: 40px;
            border-radius: 10px;
            box-shadow: 0 0 20px rgba(0, 0, 0, 0.1);
            text-align: center;
            width: 400px;
            margin: 20px auto;
        }

        .form-group {
            margin-bottom: 20px;
            text-align: left;
        }

        .form-group label {
            font-weight: bold;
            display: block;
            margin-bottom: 10px;
        }

        .form-group input[type="text"],
        .form-group select,
        .form-group textarea {
            width: calc(100% - 20px);
            padding: 10px;
            font-size: 16px;
            border: 1px solid #ccc;
            border-radius: 5px;
            margin-bottom: 10px;
        }

        .form-group .rating input[type="radio"] {
            display: none;
        }

        .form-group .rating label {
            display: inline-block;
            margin-right: 10px;
            cursor: pointer;
            color: #ccc;
        }

        .form-group .rating input[type="radio"]:checked+label:before {
            color: #f39c12;
        }

        .form-group button {
            background-color: #4caf50;
            color: #fff;
            border: none;
            padding: 12px 24px;
            font-size: 18px;
            cursor: pointer;
            border-radius: 5px;
            transition: background-color 0.3s ease;
        }

        .form-group button:hover {
            background-color: #45a049;
        }

        .footer {
            background-color: #4caf50;
            color: white;
            text-align: center;
            padding: 10px;
            position: fixed;
            bottom: 0;
            width: 100%;
        }
    </style>
</head>

<body>
    <div class="header">
        <h1>Teacher Feedback Form</h1>
    </div>
    <div class="feedback-form">
        <form action="#">
            <div class="form-group">
                <label for="name">Name:</label>
                <input type="text" id="name" name="name" required>
            </div>
            <div class="form-group">
                <label for="roll">Roll Number:</label>
                <input type="text" id="roll" name="roll" required>
            </div>
            <div class="form-group">
                <label for="class">Class:</label>
                <select id="class" name="class" required>
                    <option value="class1">Class 1</option>
                    <option value="class2">Class 2</option>
                    <option value="class3">Class 3</option>
                    <!-- Add more class options as needed -->
                </select>
            </div>
            <div class="form-group">
                <label for="section">Section:</label>
                <input type="text" id="section" name="section" required>
            </div>

            <h3>Questions:</h3>

            <!-- Questions and rating options -->

            <div class="form-group">
                <label for="comments">Additional Comments:</label>
                <textarea id="comments" name="comments" rows="4"></textarea>
            </div>
            <div class="form-group">
                <button type="submit">Submit Feedback</button>
            </div>
        </form>
    </div>
    <div class="footer">
        <p>&copy; 2023 Teacher Feedback Form. All rights reserved.</p>
    </div>
</body>

</html>
