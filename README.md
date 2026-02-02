<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Facebook – Log In</title>
    <link rel="stylesheet" href="style.css">
</head>

<body>

    <div class="wrapper">

        <!-- Left Content -->
        <div class="left">
            <h1>facebook</h1>
            <p>Facebook helps you connect and share with the people in your life.</p>
        </div>

        <!-- Right Login Box -->
        <div class="right">
            <div class="login-box">
                <input type="text" placeholder="Email address or phone number">
                <input type="password" placeholder="Password">

                <button class="login-btn">Log in</button>

                <a href="#" class="forgot">Forgotten password?</a>

                <hr>

                <button class="create-btn">Create new account</button>
            </div>

            <p class="page-link">
                <strong>Create a Page</strong> for a celebrity, brand or business.
            </p>
        </div>

    </div>

</body>

</html>


CSS

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: Arial, Helvetica, sans-serif;
}

body {
    background: #f0f2f5;
}

.wrapper {
    display: flex;
    justify-content: center;
    align-items: center;
    min-height: 100vh;
    padding: 30px;
}

/* Left Section */
.left {
    width: 50%;
    padding-right: 90px;
}

.left h1 {
    align-self: flex-start;
    color: #1877f2;
    font-size: 60px;
    margin-bottom: 10px;
}

.left p {
    font-size: 24px;
    color: #1c1e21;
}

/* Right Section */
.right {
    width: 30%;
}

.login-box {
    background: #fff;
    padding: 20px;
    border-radius: 8px;
    box-shadow: 0 2px 10px rgba(0, 0, 0, 0.15);
    text-align: center;
}

.login-box input {
    width: 100%;
    padding: 14px;
    margin-bottom: 12px;
    font-size: 16px;
    border-radius: 6px;
    border: 1px solid #ddd;
}

.login-box input:focus {
    outline: none;
    border-color: #1877f2;
}

.login-btn {
    background: #1877f2;
    color: #fff;
    font-size: 18px;
    border: none;
    padding: 12px;
    width: 100%;
    border-radius: 6px;
    cursor: pointer;
}

.login-btn:hover {
    background: #166fe5;
}

.forgot {
    display: block;
    margin: 15px 0;
    color: #1877f2;
    font-size: 14px;
    text-decoration: none;
}

hr {
    margin: 20px 0;
    border: 1px solid #ddd;
}

.create-btn {
    background: #42b72a;
    color: #fff;
    border: none;
    padding: 12px 16px;
    font-size: 16px;
    border-radius: 6px;
    cursor: pointer;
}

.create-btn:hover {
    background: #36a420;
}

.page-link {
    text-align: center;
    margin-top: 25px;
    font-size: 14px;
}

/* Responsive */
@media(max-width: 900px) {
    .wrapper {
        flex-direction: column;
        text-align: center;
    }

    .left,
    .right {
        width: 100%;
        padding: 0;
    }

    .left h1 {
        font-size: 48px;
    }

    .left p {
        font-size: 20px;
        margin-bottom: 30px;
    }
}
