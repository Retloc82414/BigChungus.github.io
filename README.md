# BigChungus.github.io
<!DOCTYPE html>
<html>
<head>
    <title>Login</title>
    <style>
        body {
            margin: 0;
            padding: 0;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background-color: #333; /* Dark gray background color */
            color: #fff; /* Text color */
        }
        .login-container {
            max-width: 400px;
            padding: 20px;
            background-color: #444; /* Slightly lighter gray for the login box */
            border-radius: 8px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.3);
        }
        .login-container h2 {
            text-align: center;
            margin-bottom: 20px;
        }
        .login-form input[type="text"],
        .login-form input[type="password"] {
            width: 100%;
            padding: 10px;
            margin-bottom: 15px;
            background-color: #555; /* Input background color */
            border: none;
            border-radius: 4px;
            color: #fff;
        }
        .login-form input[type="submit"] {
            width: 100%;
            padding: 10px;
            background-color: #007bff; /* Blue submit button */
            border: none;
            border-radius: 4px;
            color: #fff;
            cursor: pointer;
        }
        .login-form input[type="submit"]:hover {
            background-color: #0056b3; /* Darker blue on hover */
        }
    </style>
</head>
<body>
    <div class="login-container">
        <h2>Login</h2>
        <form class="login-form" onsubmit="checkLogin(event)">
            <input type="text" placeholder="Username" required>
            <input type="password" placeholder="Password" required>
            <input type="submit" value="Login">
        </form>
    </div>

    <script>
        function checkLogin(event) {
            event.preventDefault();
            
            // Retrieve the username and password entered by the user
            const usernameInput = document.querySelector('input[type="text"]');
            const passwordInput = document.querySelector('input[type="password"]');
            const enteredUsername = usernameInput.value;
            const enteredPassword = passwordInput.value;

            // Replace these lines with your own validation logic
            const correctUsername = "Admin";
            const correctPassword = "theyearis2023";

            if (enteredUsername === correctUsername && enteredPassword === correctPassword) {
                // Replace this line with the desired action upon successful login
                alert("Login successful!");
            } else {
                alert("Incorrect username or password. Please try again.");
            }
        }
    </script>
</body>
</html>
