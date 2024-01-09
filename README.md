# portfolio

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
  }
  
  header {
    width: 100%;
    height: 70px;
    background-color: #FFFAF6;
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 0 50px;
  }
  
  body {
    font-family: 'Cabinet Grotesk', sans-serif;
    background-color: #203A27;
    margin: 0;
  }
  
  .nav-bar ul {
    list-style: none;
    padding: 0;
    margin: 0;
    display: flex;

  }

  .nav-bar ul li {
    margin: 0 5px;
  }
  
  .nav-bar a {
    text-decoration: none;
  }

  .logo{
    font-family: 'General Sans', sans-serif;
  }

  .hamburger{
    display: none;
  }

  .nav-bar ul li a{
    display: block;
    font-size: 17px;
    margin: 0 5px;
    color: black;
    padding: 10px 25px;
    border-radius: 50px;
    transition: 0.2s;
  }

  .nav-bar ul li a:hover{
    color: #FFFAF6;
    background-color: black;
  }

  @media only screen and (max-width: 1320px) {
    header {
        padding: 0 50px;
    }
}

@media only screen and (max-width: 1100px) {
    header {
        padding: 0 30px;
    }
}

@media only screen and (max-width: 900px) {
    .hamburger{
        display: block;
        cursor: pointer;
    }

    .hamburger .line{
        width: 25px;
        height: 3px;
        background: black;
        margin: 5px 0;
    }

    .nav-bar{
        height: 0;
        position: absolute;
        top: 80px;
        left: 0;
        right: 0;
        width: 100vw;
        background: #FFFAF6;
        transition: 0.2s;
        overflow: hidden;
    }
    .nav-bar ul{
        display: block;
        width: fit-content;
        margin: 70px auto 0 auto; 
        text-align: center;
        transition: 0.5s;
        opacity: 0;
    }
    .nav-bar ul li a{
        margin-bottom: 12px
    }
}



<!DOCTYPE html>
    <html lang="en">
        <head>
            <!-- Required meta tags -->
            <meta charset="utf-8">
            <meta name="viewport" content="width=device-width, initial-scale=1">

            <!-- Bootstrap CSS -->
            <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3/dist/css/bootstrap.min.css" rel="stylesheet">
            
            <!-- style sheet -->
            <link rel="stylesheet" href="./style.css">

            <!-- Fonts     font-family: 'General Sans', sans-serif; -->
            <link href="https://api.fontshare.com/v2/css?f[]=general-sans@700&f[]=cabinet-grotesk@400&display=swap" rel="stylesheet">
        </head>

        <title>
            Samyuktha Pugalanthi
        </title>

        <body>
            <header>
                <div class="logo">Samyuktha</div>
                <div class="hamburger">
                    <div class="line"></div>
                    <div class="line"></div>
                    <div class="line"></div>
                </div>

                <div class="nav-bar">
                    <ul>
                        <li>
                            <a href="">about</a>
                        </li>
                        <li>
                            <a href="">skill</a>
                        </li>
                        <li>
                            <a href="">projects</a>
                        </li>
                        <li>
                            <a href="" >contact</a>
                        </li>
                    </ul>
                </div>
            </header>

            <script>
                document.addEventListener("DOMContentLoaded", function () {
  const hamburger = document.querySelector(".hamburger");
  const navBar = document.querySelector(".nav-bar");

  hamburger.addEventListener("click", function () {
    // Toggle the "active" class on the hamburger icon
    hamburger.classList.toggle("active");

    // Toggle the visibility of the navigation bar
    if (navBar.style.height === "0px" || navBar.style.height === "") {
      navBar.style.height = "200px"; // You can adjust the height as needed
    } else {
      navBar.style.height = "0px";
    }
  });
});

            </script>
        </body>

    </html>

  