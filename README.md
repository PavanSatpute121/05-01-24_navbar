<!-- Html code (nav-bar)  -->
<br>
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <link rel="stylesheet" href="style2.css">

</head>
<body>
    <header>
        <div class="logo">Rich</div>
        <div class="hamburger">
            <div class="line"></div>
            <div class="line"></div>
            <div class="line"></div>
        </div>

        <nav class="nav-bar">
            <ul>
                <li>
                 <a href="" class="active">Home</a>
                </li>
                <li>
                    <a href="" >About</a>
                </li>
                <li>
                    <a href="" >Career</a>
                </li>
                <li>
                    <a href="" >Feedback</a>
                </li>
                <li>
                    <a href="" >Contacts</a>
                </li>
                <li>
                    <a href="" >Services</a>
                </li>
                <li>
                    <a href="" >Comment</a>
                </li>
            </ul>
        </nav>
    </header>


    <script>
        hamburger = document.querySelector(".hamburger");
        hamburger.onclick = function(){  /* Function calling to nav-bar class  */
            navBar = document.querySelector(".nav-bar");
            navBar.classList.toggle("active");
        }
    </script>

    <!------------------------------------------------------- Header or Nav-bar End hare ------------------------------------------------->
</body>
</html>





//css code of navbar

*{
    margin: 0;
    padding: 0;
    list-style: none;
    text-decoration: none;
    box-sizing: border-box;
}
body{
    background: #fefefe;

}
header{
    width: 100%;
    height: 80px;
    background: #11101b;
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 0 100px;
}
.logo{
    font-size: 28px;
    font-weight: bold;
    color: #fefefe;
}


.hamburger{
    display: none;
}
.nav-bar ul{
    display: flex;
}
.nav-bar ul li a{
    display: block;
    color: #fefefe;
    font-size: 20px;
    padding: 10px 25px;
    border-radius: 50px;
    transition: 0.2s;
    margin: 0 5px;
    
}
.nav-bar ul li a:hover {
    color: #27215f;
    background: #fefefe;
    
}
.nav-bar ul li a.active{
    color: #11101b;
    background: #fefefe;

}

@media only screen and (max-width: 1320px){
    header{
        padding: 0 50px;
    }
}

@media only screen and (max-width: 1100px){
    header{
        padding: 0 30px;
    }
}

@media only screen and (max-width: 900px){
    .hamburger{
        display: block;
        cursor: pointer;
    }

    .hamburger .line{
        width: 30px;
        height: 3px;
        background: #fefefe;
        margin: 6px 0;
    }
    .nav-bar{
        height: 0;
        
        position: absolute;
        top: 80px;
        left: 0;
        right: 0;
        width: 100vw;
        background: #11101b;
        transition: 0.5s;
        overflow: hidden;
    }
    .nav-bar.active{
        height: 450px;
    }
    .nav-bar ul{
        display: block;
        width: fit-content;
        margin: 80px auto 0 auto;
        text-align: center;
        transition: 0.5s;
        opacity: 0;
    }
    .nav-bar.active ul{
        opacity: 1;
    }
    
    .nav-bar ul li a{
        margin-bottom: 12px;
        
    }
}

/* -----------------------------> NAV Bar End Hare <---------------------------------*/

