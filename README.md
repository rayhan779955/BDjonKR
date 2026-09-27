<!DOCTYPE html>
<html>
<head>
<title>Admin Login</title>
<style>
body{
    font-family: Arial;
    background:#f2f2f2;
}
.box{
    width:300px;
    margin:100px auto;
    background:white;
    padding:20px;
    border-radius:10px;
    box-shadow:0 0 10px #aaa;
}
input,button{
    width:100%;
    padding:10px;
    margin-top:10px;
}
button{
    background:#007bff;
    color:white;
    border:0;
    cursor:pointer;
}
</style>
</head>

<body>

<div class="box">
<h2>Admin Login</h2>

<input type="text" id="user" placeholder="Username">

<input type="password" id="pass" placeholder="Password">

<button onclick="login()">Login</button>

<p id="msg"></p>

</div>


<script>
function login(){

let username = document.getElementById("user").value;
let password = document.getElementById("pass").value;

if(username=="admin" && password=="12345"){
    alert("Login Success");
    window.location="dashboard.html";
}
else{
    document.getElementById("msg").innerHTML="ভুল তথ্য!";
}

}
</script>

</body>
</html>
