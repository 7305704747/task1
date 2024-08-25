<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Login Form</title>
    <style>
        body {
            background-image: url("in.jpeg");
            background-repeat: no-repeat;
            background-size: cover;
        }

        form {
            width: 300px;
            margin: 0 auto;
            
            padding: 25px 50px 85px 100px;
           background: linear-gradient(to right, #4a90e2, #003366);
               color: #fff;
    padding: 40px 40px;
   text-align: center;
            opacity: 0.8;
            border: 2px solid black;
            border-radius: 10px;
        }

        label {
            margin-bottom: 5px;
            display: block;
        }

        input {
            width: 100%;
            padding: 10px;
            border: 1px solid #ccc;
        }

        button {
            padding: 10px 20px;
            background-color: #007bff;
            color: #fff;
            border: none;
            cursor: pointer;
        }
    </style>
</head>
<body>
    <center><h1>INTERNSHIP</h1></center>
    <h1>Hello Learners!</h1>
    <form id="loginForm">
        <h2>Login Form</h2>
        <b><label for="username">Username:</label></b>
        <input type="text" id="username" name="username" placeholder="Username or email"><br><br>

        <b><label for="password">Password:</label></b>
        <input type="password" id="password" name="password" placeholder="Password"><br><br>

        <button type="submit">Login</button>
    </form>

    <script>
        document.getElementById('loginForm').addEventListener('submit', function(event) { event.preventDefault();
            var username = document.getElementById('username').value;
            var password = document.getElementById('password').value;
          if (username&&password) {
 
          alert('Username or Email: ' + username + '\n' + 'Password: ' + password);
               
        document.getElementById('loginForm').reset();  } 
       else {
        alert('Please fill in all fields.');
    }
        });
</script>
</body>
</html>
