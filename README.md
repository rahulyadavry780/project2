<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Before and after pseudo selector</title>
    <link href="https://fonts.googleapis.com/css2?family=Unbounded:wght@300&display=swap" rel="stylesheet">
    <style>
 body{
    background-color: black;
    color: azure;
    margin: 0px;
    padding: 0px;
    
    
 }
 header::before{
   background: url(https://images.unsplash.com/photo-1675066097559-f8cae0f4e60a?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=387&q=80) no-repeat center center/cover;
   position: absolute;
   content: "";
   width:100%;
   height:100%;
   z-index: -1;
   top:0;
   left:0;
   opacity:0.5;

 }
 section{
    font-family: 'Unbounded', cursive;;
    display: flex;
    flex-direction: column;
    margin: 10px 35px;
    align-items: center;
    /* border: 2px solid red; */
    height:500px;
    justify-content: center;
 }
 .navigation{
    display: flex;
    font-size: large;
 }
 li{
    list-style: none;
    padding: 23px;
 }
 section::before{
    content:"This is my content";
 }
 section::after{
    content:"honesty is the best policy";
 }
 li:hover{
   cursor: pointer;
   color:rgb(127, 242, 255)
 }
    </style>
</head>
<body>
    
        <nav class="navbar">
            <ul class="navigation">
                <li class="item1">Home</li>
                <li class="item2">Services</li>
                <li class="item3">About</li>
                <li class="item4">Contact us</li>
            </ul>
        </nav>
        <header>
        <section>
            <h1>welcome to coding world</h1>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Repellat enim unde soluta perferendis molestias rem aperiam sapiente sunt doloremque, veritatis dolorum, porro ipsam.</p>
        </section>
        
    </header>
</body>
</html>
