# myvalentinesluer
Asking m girlfriend for Valentines
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Will you be My Valentines?</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #fefefe;
            text-align: center;
            margin-top: 50px;
        }
        h1 {
            color: #ff69b4;
        }
        .button-yes, .button-no {
            display: inline-block;
            margin: 10px;
            padding: 15px 30px;
            font-size: 18px;
            color: white;
            border: none;
            border-radius: 8px;
            cursor: pointer;
            transition: background-color 0.3s, transform 0.3s;
        }
        .button-yes {
            background-color: #ff69b4;
        }
        .button-no {
            background-color: #ff6f69;
        }
        .button-yes:hover {
            background-color: #ff4081;
        }
        .button-no:hover {
            background-color: #ff4945;
        }
    </style>
    <script>
        let yesButton = null;
        let initialSize = 1;

        function sayYes() {
            alert("Yay! I knew you'd say yes!");
        }

        function sayNo() {
            if (yesButton) {
                initialSize += 0.1;
                yesButton.style.transform = "scale(" + initialSize + ")";
            }
        }

        window.onload = function() {
            yesButton = document.getElementById('yesButton');
        }
    </script>
</head>
<body>
    <h1>Will you be my Valentine?</h1>
    <button id="yesButton" class="button-yes" onclick="sayYes()">Yes!</button>
    <button class="button-no" onclick="sayNo()">No</button>
</body>
</html>
