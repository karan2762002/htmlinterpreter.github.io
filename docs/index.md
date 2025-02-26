<html>
<head>
    <title>HTML Interpreter</title>
    <style>
        body {
            background-color: #f0f4f8;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            color: #333;
            margin: 0;
            padding: 0;
        }
        .container {
            max-width: 800px;
            margin: 50px auto;
            padding: 20px;
            text-align: center;
            background-color: #ffffff;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
            border-radius: 10px;
        }
        .output {
            background-color: #ffffff;
            border: 2px solid #00796b;
            padding: 20px;
            margin-bottom: 20px;
            border-radius: 10px;
            box-shadow: inset 0 2px 4px rgba(0, 0, 0, 0.1);
        }
        .output p {
            color: #d32f2f;
        }
        textarea {
            width: 100%;
            height: 150px;
            border: 2px solid #00796b;
            border-radius: 10px;
            padding: 10px;
            font-size: 16px;
            box-shadow: inset 0 2px 4px rgba(0, 0, 0, 0.1);
            resize: none;
        }
        button, input[type="reset"] {
            background-color: #00796b;
            color: #ffffff;
            border: none;
            padding: 10px 20px;
            margin: 10px;
            border-radius: 5px;
            cursor: pointer;
            font-size: 16px;
            transition: background-color 0.3s ease;
        }
        button:hover, input[type="reset"]:hover {
            background-color: #004d4d;
        }
        footer {
            margin-top: 20px;
            color: #777;
            font-size: 14px;
        }
        h1 {
            color: #00796b;
        }
        p#d2 {
            margin: 20px 0;
        }
    </style>
    <script>
        function lw() {
            var x = document.getElementById("d1");
            var z = document.getElementById("d3");
            x.innerHTML = z.value;
        }
    </script>
</head>
<body>
    <div class="container">
        <h1>HTML Interpreter</h1>
        <div id="d1" class="output">
            <p>See your HTML render in real-time!</p>
        </div>
        <p id="d2">
            <u><b><font size="6" color="#00796b">Live HTML Preview</font></b></u>
        </p>
        <u><font size="3" color="red">Enter your code</font></u>
        <textarea id="d3" onkeyup="lw()"></textarea>
        <br/>
        <button type="button" onclick="window.location.href='https://in.linkedin.com/in/karan2762002'">Submit</button>
        <input type="reset" value="Reset" onclick="document.getElementById('d3').value=''; lw();">
        <footer>
            <p>| Copyright ©2022 | All Rights Reserved..</p>
        </footer>
    </div>
</body>
</html>
