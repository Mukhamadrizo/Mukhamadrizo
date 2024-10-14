<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>JavaScript Simple Example</title>
</head>
<body>
    <h1>Welcome to My Website</h1>
    
    <p>Ismingizni kiriting:</p>
    <input type="text" id="nameInput" placeholder="Ismingizni kiriting">
    
    <button onclick="greeting()">Salom aytish</button>
    
    <p id="greetingMessage"></p>
    
    <script>
        function greeting() {
            var name = document.getElementById("nameInput").value;
            if(name) {
                document.getElementById("greetingMessage").innerHTML = "Salom, " + name + "!";
            } else {
                document.getElementById("greetingMessage").innerHTML = "Iltimos, ismingizni kiriting.";
            }
        }
    </script>
</body>
</html>
