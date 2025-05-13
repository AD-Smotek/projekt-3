webovka pro mobilní zařízení 

tuto část projektu jsem si chtěl zkusit něco pro mobilní zařízení,
takže jsem dělal hodně s tutoriálama a taky trošku s Chatem kvůli opravě chyb.
tato část projektu trvala o mnoho dýl než šachy a to do list, ale hlavně mi šlo 
o to aby to měnilo tvar nebo spíš aby to vypadalo dobře na mobilním zařízením.
vím že to není hotovo ale jak říkám nebylo to ani záměrem.

Kod:














<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>clothing-test-shop</title>
    <style>
        body{
            font-family: sans-serif;
        }
        nav{
            width: 100%;
            display: flex;
            align-items: center;
            justify-content: space-between;
            background-color: lightgray;
        }
        .navbar{
            grid-area: navbar;
        }
        .logo-nav{
            width: 50px;
            margin: 0;
            margin-left: 30px;
        }
        nav ul li{
            list-style: none;
            display: inline-block;
            margin-right: 30px;
        }
        nav ul li a{
            text-decoration: none;
            color: #000;
            font-size: 14px;
        }
        nav ul li a:hover{
            color: #ff5ea2;
        }
        .container{
            display: grid;
            grid-template-columns: repeat(6, 1fr);
            grid-template-rows: 0.1fr 0.1fr 0.3fr 0.3fr 0.1fr;
            grid-template-areas: 
                "navbar navbar navbar"
                "main main main"
                "clothing1 clothing2 clothing3"
                "clothing4 clothing5 clothing6"
                "footer footer footer"
            ;
        }


        main{
            text-align: center;
            grid-area: main;
        }


        .clothing-column1{
            grid-area: clothing1;
        }
        .clothing-column2{
            grid-area: clothing2;
        }
        .clothing-column3{
            grid-area: clothing3;
        }
        .clothing-column4{
            grid-area: clothing4;
        }
        .clothing-column5{
            grid-area: clothing5;
        }
        .clothing-column6{
            grid-area: clothing6;
        }
        .clothing-column7{
            grid-area: clothing7;
        }
        .clothing-column8{
            grid-area: clothing8;
        }
        .clothing-column9{
            grid-area: clothing9;
        }
        .clothing-column10{
            grid-area: clothing10;
        }
        .clothing-column11{
            grid-area: clothing11;
        }
        .clothing-column12{
            grid-area: clothing12;
        }
        .clothing-column13{
            grid-area: clothing13;
        }
        .clothing-column14{
            grid-area: clothing14;
        }
        .clothing-column15{
            grid-area: clothing15;
        }
        .clothing-column16{
            grid-area: clothing16;
        }
        .clothing-column17{
            grid-area: clothing17;
            height: fit-content;
        }
        .clothing-column18{
            grid-area: clothing18;
        }
        #menu-img{
            width: 20px;
            margin-right: 20px;
            display: none;
        }

        .clothing-column1, 
        .clothing-column2, 
        .clothing-column3, 
        .clothing-column4,
        .clothing-column5, 
        .clothing-column6,
        .clothing-column7,
        .clothing-column8,
        .clothing-column9,
        .clothing-column10,
        .clothing-column11,
        .clothing-column12,
        .clothing-column13,
        .clothing-column14,
        .clothing-column15,
        .clothing-column16,
        .clothing-column17,
        .clothing-column18{
            -webkit-user-select: none;
            -ms-user-select: none;
            user-select: none;
            box-sizing: border-box;
            margin: 0 auto;
            background-color: lightgray;
            padding: 5px;
            width: fit-content;
            box-shadow: 0px 0px 10px gray;
            transition: 0.15s;
            cursor: pointer;
            margin-bottom: 10%;
        }

        .clothing-column1:hover, 
        .clothing-column2:hover, 
        .clothing-column3:hover, 
        .clothing-column4:hover,
        .clothing-column5:hover, 
        .clothing-column6:hover,
        .clothing-column7:hover,
        .clothing-column8:hover,
        .clothing-column9:hover,
        .clothing-column10:hover,
        .clothing-column11:hover,
        .clothing-column12:hover,
        .clothing-column13:hover,
        .clothing-column14:hover,
        .clothing-column15:hover,
        .clothing-column16:hover,
        .clothing-column17:hover,
        .clothing-column18:hover{
            padding: 7px 7px 0 7px;
            margin-bottom: 5%;
        }

        
        @media only screen and (max-width:500000px){
            .container{
                display: grid;
                grid-template-columns: 1fr 1fr 1fr 1fr;
                grid-template-rows: 0.1fr 0.1fr 0.3fr 0.3fr 0.1fr;
                grid-template-areas: 
                    "navbar navbar navbar navbar"
                    "main main main main"
                    "clothing1 clothing2 clothing3 clothing4"
                    "clothing5 clothing6 clothing7 clothing8"
                    "clothing9 clothing10 clothing11 clothing12"
                    " clothing13 clothing14 clothing15 clothing16"
                    " clothing17 clothing18 clothing18 clothing18"
                    "footer footer footer footer"
                ;
            }
        }
        @media only screen and (max-width:992px){
            .container{
                display: grid;
                grid-template-columns: 1fr 1fr 1fr;
                grid-template-rows: 0.1fr 0.1fr 0.3fr 0.3fr 0.1fr;
                grid-template-areas: 
                    "navbar navbar navbar"
                    "main main main"
                    "clothing1 clothing2 clothing3"
                    "clothing4 clothing5 clothing6"
                    "clothing7 clothing8 clothing9"
                    "clothing10 clothing11 clothing12"
                    "clothing13 clothing14 clothing15"
                    "clothing16 clothing17 clothing18"
                    "footer footer footer"
                ;
            }
        }
        @media only screen and (max-width:768px){
            .container{
                display: grid;
                grid-template-columns: 1fr 1fr;
                grid-template-rows: 0.1fr 0.1fr 0.3fr 0.3fr 0.1fr;
                grid-template-areas: 
                    "navbar navbar"
                    "main main"
                    "clothing1 clothing2"
                    "clothing3 clothing4"
                    "clothing5 clothing6"
                    "clothing7 clothing8"
                    "clothing9 clothing10"
                    "clothing11 clothing12"
                    "clothing13 clothing14"
                    "clothing15 clothing16"
                    "clothing17 clothing18"
                    "footer footer"
                ;
            }
        }
        @media only screen and (max-width:600px){
            .container{
                display: grid;
                grid-template-columns: 1fr;
                grid-template-rows: 0.1fr 0.1fr 0.3fr 0.3fr 0.1fr;
                grid-template-areas: 
                    "navbar"
                    "main"
                    "clothing1"
                    "clothing2"
                    "clothing3"
                    "clothing4"
                    "clothing5"
                    "clothing6"
                    "clothing7"
                    "clothing8"
                    "clothing9"
                    "clothing10"
                    "clothing11"
                    "clothing12"
                    "clothing13"
                    "clothing14"
                    "clothing15"
                    "clothing16"
                    "clothing17"
                    "clothing18"
                    "footer"
                ;
            }
        }
        
        
        @media only screen and (max-width:450px){
            #menu-img{
                display: block;
                float: left;
            }
            #menu-list{
                display: none;
            }
            #ul-list{
                display: none;
            }
        }
        

    </style>
</head>
<body>
    <div class="container">
        <div class="navbar">
            <nav>
                <img src="Playstation_Img/logo.png" class="logo-nav">
                <div id="ul-list">
                    <ul id="menuList">
                        <li><a href="">Home</a></li>
                        <li><a href="">About</a></li>
                        <li><a href="">Services</a></li>
                        <li><a href="">Contact</a></li>
                        <li><a href="">Cart</a></li>
                    </ul>
                </div>
                
                <img src="Playstation_Img/menu.png" id="menu-img">
                <div class="navbar-btnned">
                    
                </div>
            </nav>
        </div>
        <main>
            <h1>This is a clothing brand</h1><br>
            <h2>Pick the best style that fits you</h2>
        </main>

            <div class="clothing-column1">
                <img src="t-shirt.jpg" class="tshirt-img">
                <p class="shirt-text">T-shirt</p>
                <p clas="price">10$</p>
            </div>
            <div class="clothing-column2">
                <img src="t-shirt.jpg" class="tshirt-img">
                <p class="shirt-text">T-shirt</p>
                <p clas="price">10$</p>
            </div>
            <div class="clothing-column3">
                <img src="t-shirt.jpg" class="tshirt-img">
                <p class="shirt-text">T-shirt</p>
                <p clas="price">10$</p>
            </div>
            <div class="clothing-column4">
                <img src="t-shirt.jpg" class="tshirt-img">
                <p class="shirt-text">T-shirt</p>
                <p clas="price">10$</p>
            </div>
            <div class="clothing-column5">
                <img src="t-shirt.jpg" class="tshirt-img">
                <p class="shirt-text">T-shirt</p>
                <p clas="price">10$</p>
            </div>
            <div class="clothing-column6">
                <img src="t-shirt.jpg" class="tshirt-img">
                <p class="shirt-text">T-shirt</p>
                <p clas="price">10$</p>
            </div>
            <div class="clothing-column7">
                <img src="t-shirt.jpg" class="tshirt-img">
                <p class="shirt-text">T-shirt</p>
                <p clas="price">10$</p>
            </div>
            <div class="clothing-column8">
                <img src="t-shirt.jpg" class="tshirt-img">
                <p class="shirt-text">T-shirt</p>
                <p clas="price">10$</p>
            </div>
            <div class="clothing-column9">
                <img src="t-shirt.jpg" class="tshirt-img">
                <p class="shirt-text">T-shirt</p>
                <p clas="price">10$</p>
            </div>
            <div class="clothing-column10">
                <img src="t-shirt.jpg" class="tshirt-img">
                <p class="shirt-text">T-shirt</p>
                <p clas="price">10$</p>
            </div>
            <div class="clothing-column11">
                <img src="t-shirt.jpg" class="tshirt-img">
                <p class="shirt-text">T-shirt</p>
                <p clas="price">10$</p>
            </div>
            <div class="clothing-column12">
                <img src="t-shirt.jpg" class="tshirt-img">
                <p class="shirt-text">T-shirt</p>
                <p clas="price">10$</p>
            </div>
            <div class="clothing-column13">
                <img src="t-shirt.jpg" class="tshirt-img">
                <p class="shirt-text">T-shirt</p>
                <p clas="price">10$</p>
            </div>
            <div class="clothing-column14">
                <img src="t-shirt.jpg" class="tshirt-img">
                <p class="shirt-text">T-shirt</p>
                <p clas="price">10$</p>
            </div>
            <div class="clothing-column15">
                <img src="t-shirt.jpg" class="tshirt-img">
                <p class="shirt-text">T-shirt</p>
                <p clas="price">10$</p>
            </div>
            <div class="clothing-column16">
                <img src="t-shirt.jpg" class="tshirt-img">
                <p class="shirt-text">T-shirt</p>
                <p clas="price">10$</p>
            </div>
            <!-- <div class="clothing-column17">
                <img src="t-shirt.jpg" class="tshirt-img">
                <p class="shirt-text">T-shirt</p>
                <p clas="price">10$</p>
            </div>
            <div class="clothing-column18">
                <img src="t-shirt.jpg" class="tshirt-img">
                <p class="shirt-text">T-shirt</p>
                <p clas="price">10$</p>
            </div> -->
    </div>

    <script>



    </script>

</body>
</html>
