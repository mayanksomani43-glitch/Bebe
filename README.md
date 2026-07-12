<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>For Bebe ❤️</title>

<style>
*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    font-family:Arial,Helvetica,sans-serif;
}

body{
    height:100vh;
    display:flex;
    justify-content:center;
    align-items:center;
    background:url("background.jpg") center/cover no-repeat;
}

.overlay{
    position:fixed;
    inset:0;
    background:rgba(0,0,0,0.45);
}

.container{
    position:relative;
    z-index:2;
    width:350px;
    padding:35px;
    border-radius:15px;
    background:rgba(255,255,255,0.15);
    backdrop-filter:blur(10px);
    text-align:center;
    color:white;
}

h1{
    margin-bottom:20px;
}

input{
    width:100%;
    padding:12px;
    margin:10px 0;
    border:none;
    border-radius:8px;
    outline:none;
}

button{
    width:100%;
    padding:12px;
    margin-top:10px;
    border:none;
    border-radius:8px;
    background:#ff4d6d;
    color:white;
    font-size:16px;
    cursor:pointer;
}

button:hover{
    background:#ff2f56;
}

#message{
    display:none;
    max-width:700px;
    padding:40px;
    text-align:center;
    color:white;
    background:rgba(0,0,0,0.45);
    backdrop-filter:blur(8px);
    border-radius:15px;
}

#message h1{
    font-size:40px;
    margin-bottom:20px;
}

#message p{
    font-size:20px;
    line-height:1.8;
}
</style>

</head>
<body>

<div class="overlay"></div>

<div class="container" id="loginBox">
    <h1>❤️ Welcome ❤️</h1>

    <input type="text" id="username" placeholder="Name">

    <input type="password" id="password" placeholder="Password">

    <button onclick="login()">Login</button>
</div>

<div id="message">
    <h1>Dear Bebe ❤️</h1>

    <p>
        I know that words alone cannot erase the hurt I may have caused,
        but they can carry the truth from my heart.
        <br><br>

        I'm truly sorry.
        Every moment without your smile reminds me how precious you are to me.
        You deserve love, respect, patience, and kindness every single day.
        <br><br>

        If I have disappointed you, I promise to learn from my mistakes and become a better person.
        You are one of the most beautiful parts of my life, and I never want to lose what we have.
        <br><br>

        Thank you for every memory, every smile, and every moment we've shared.
        I hope you can forgive me when you're ready.
        <br><br>

        ❤️ I love you, Bebe. ❤️
    </p>
</div>

<script>

const correctName = "bebe";
const correctPassword = "love123";

function login(){

    let name = document.getElementById("username").value.toLowerCase();
    let pass = document.getElementById("password").value;

    if(name===correctName && pass===correctPassword){

        document.getElementById("loginBox").style.display="none";
        document.getElementById("message").style.display="block";

    }else{

        alert("Wrong name or password.");
    }

}

</script>

</body>
</html>
