# HTML-CSS-project
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>OTT Flatform</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha3/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-KK94CHFLLe+nY2dmCWGMq91rCGa5gtU4mk92HdvYe+M/SXH301p5ILy+dN9+nJOZ" crossorigin="anonymous">
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha3/dist/js/bootstrap.bundle.min.js" integrity="sha384-ENjdO4Dr2bkBIFxQpeoTz1HIcje39Wm4jDKdf19U8gI4ddQ3GYNS7NTKfAdVQSZe" crossorigin="anonymous"></script>
    <script src="https://cdn.jsdelivr.net/npm/@popperjs/core@2.11.7/dist/umd/popper.min.js" integrity="sha384-zYPOMqeu1DAVkHiLqWBUTcbYfZ8osu1Nd6Z89ify25QV9guujx43ITvfi12/QExE" crossorigin="anonymous"></script>
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha3/dist/js/bootstrap.min.js" integrity="sha384-Y4oOpwW3duJdCWv5ly8SCFYWqFDsfob/3GkgExXKV4idmbt98QcxXYs9UoXAB7BZ" crossorigin="anonymous"></script>


    <style>
      body{
        background-color:black;
      }
        *{
            margin: 0;
        }
        .nav-bar{
            height: 100px;
            width: 100%;
            border: solid;
            flex-wrap: nowrap;
            display: flex;
            background-color: black;
            position: fixed;
            top: 0;
            z-index: 1000;
        }
        .nav-logo{
          height: 20px;
          width: 20px;
        }
        .nav-items a{
            text-decoration:none;
        }
        .nav-items ul{
            display: flex;
            height: 100px;
            justify-content:space-around;
            /* align-items: center; */
            width: 1000px;
            flex-wrap: wrap;
            position: relative;
            left: 69%;
            font-size: 30px;
            top: 20px;
            margin-left: 0px;
        }        
        .nav-items a:hover{
          color:crimson;
        }
        .home{
          padding-top: 160px;
        }
        #recent{
          padding-top: 130px;
        }
        .mostly{
          padding-top: 130px;
        }
        
        
        .carousel-control-prev-icon{
            
         margin-top: 0px;
         margin-left: 0px;

        }      
        
        .carousel-inner img{
          height: 700px;
          width: 100%;
        }
        .corousel-slide{
          margin: 50px;
        }
        .recent h2{
          color: cyan;
          display: inline;
        }
        h2:hover{
          text-decoration: underline;
        }


        .recent-images img{
          width: 18%;
          height: 400px;
        }
        
        .recent-images{
          height: 850px;        
          display: flex;
          flex-wrap: wrap;
          align-items: center;
          justify-content: space-evenly;
        }   


        .recent-images img:hover{
          scale:1.2;
          transition: all .2s ease-in;
          border-radius: 10px;
        }

        .mostly-images img{
          width: 18%;
          height: 400px;
        }
        
       .mostly-images{
          height: 850px;        
          display: flex;
          flex-wrap: wrap;
          align-items: center;
          justify-content: space-evenly;
        }  
        .mostly-images img:hover{
          scale:1.2;
          transition: all .2s ease-in;
          border-radius: 10px;
        }
        .mostly h2{
          color: cyan;
          display: inline;
        }
        h2:hover{
          text-decoration: underline;
        }
        .trending-images img{
          width: 18%;
          height: 400px;
        }
        
       .trending-images{
          height: 850px;        
          display: flex;
          flex-wrap: wrap;
          align-items: center;
          justify-content: space-evenly;
        }  
        .trending-images img:hover{
          scale:1.2;
          transition: all .2s ease-in;
          border-radius: 10px;
        }
        .trending h2{
          color: cyan;
          display: inline;
        }
        h2:hover{
          text-decoration: underline;
        }

        .abt{
          border: solid;
          height: 200px;
          width: 100%;
          background-color: rgb(36, 40, 40);
          display: flex;
          align-items:start;
        }
        .company{
          height: 200px;
          width: 25%;
          position: relative;
        /* background-color: aliceblue; */
        }
        .company h3{
          font-size: 20px;
          color: rgb(104, 108, 112);
        }
        .company p{
          color: rgb(104, 108, 112);
        }
        .viewin{
          height: 200px;
          width: 25%;
          position: relative;
        }
        .viewin h3{
          font-size: 20px;
          color: rgb(104, 108, 112);
        }
        .viewin p{
          color: rgb(104, 108, 112);
        }
        .needhelp{
          height: 200px;
          width: 25%;
          position: relative;
        }
        .needhelp h3{
          font-size: 20px;
          color: rgb(104, 108, 112);
        }
        .needhelp p{
          color: rgb(104, 108, 112);
        }
        .contact{
          height: 200px;
          width: 25%;
          position: relative;
        }
        .contact h3{
          font-size: 21px;
          color: rgb(104, 108, 112);
        }
        .contact img{
          height: 40px;
          width: 40px;
          margin-left: 50px;
        }
        .contact img:hover{
          scale: 1.2;
          transition: all .1ms ease-in;
        }
    </style>
</head>
<body>
    

    <header class="nav-bar">
        <div class=".nav-logo">
            <img src="C:\Users\Kushi\Desktop\web\Project\OTT\images\navlogo.png" alt="" height="100px">
        </div>
        <div class="nav-items">
            <ul type="none">
                <li><a href="#home">Home</a></li>
                <li><a href="#recent">Recently added</a></li>
                <li><a href="#mostly">Most Watched</a></li>
                <li><a href="#trending">Trending Movies</a></li>
                <li><a href="#sign-in">Sign-in</a></li>
                <li><a href="#about">About</a></li>
            </ul>
        </div>
    </header>

    <!-- Home page stars -->
    <div class="home" id="home">
      <div id="carouselExampleAutoplaying" class="carousel slide" data-bs-ride="carousel">
        <div class="carousel-inner" >
          <div class="carousel-item active">
            <img src="C:\Users\Kushi\Desktop\web\Project\OTT\images\vampire-diaries-main-poster-1024x576.jpg"  class="d-block " alt="...">
          </div>
          <div class="carousel-item">
            <img src="C:\Users\Kushi\Desktop\web\Project\OTT\images\download (2)home.jpeg"  class="d-block" alt="..." >
          </div>
          <div class="carousel-item">
            <img src="C:\Users\Kushi\Desktop\web\Project\OTT\images\home3.jpeg"  class="d-block" alt="..." >
          </div>
        </div>
        <button class="carousel-control-prev" type="button" data-bs-target="#carouselExampleAutoplaying" data-bs-slide="prev">
          <span class="carousel-control-prev-icon" aria-hidden="true"></span>
          <span class="visually-hidden">Previous</span>
        </button>
        <button class="carousel-control-next" type="button" data-bs-target="#carouselExampleAutoplaying" data-bs-slide="next">
          <span class="carousel-control-next-icon" aria-hidden="true"></span>
          <span class="visually-hidden">Next</span>
        </button>
      </div>

    </div>
    
      
    <!-- Home page ends -->

      <!-- Recently added starts -->
      <div class="recent" id="recent">
        <div class="recent-title">
          <h2>Recently added</h2>
        </div>
        <div class="recent-images">
          <img src="C:\Users\Kushi\Desktop\web\Project\OTT\images\recentlyimg1.jpg" alt="" >
          <img src="C:\Users\Kushi\Desktop\web\Project\OTT\images\recentlyimg2.jpeg" alt="" >
          <img src="C:\Users\Kushi\Desktop\web\Project\OTT\images\recentlyimg3.jpeg" alt="" >
          <img src="C:\Users\Kushi\Desktop\web\Project\OTT\images\recentlyimg4.jpeg" alt="" >
          <img src="C:\Users\Kushi\Desktop\web\Project\OTT\images\recentlyimg5.jpeg" alt="" >
          <img src="C:\Users\Kushi\Desktop\web\Project\OTT\images\recentlyimg6.jpeg" alt="" >
          <img src="C:\Users\Kushi\Desktop\web\Project\OTT\images\recentlyimg7.jpeg" alt="" >
          <img src="C:\Users\Kushi\Desktop\web\Project\OTT\images\recentlyimg8.jpeg" alt="" >
          <img src="C:\Users\Kushi\Desktop\web\Project\OTT\images\recentlyimg9.jpeg" alt="" >
          <img src="C:\Users\Kushi\Desktop\web\Project\OTT\images\recentlyimg11.jpeg" alt="">
        </div>
      </div>
      <!-- Recently added ends -->

      <!-- Mostly Watched movies starts -->
      <div class="mostly" id="mostly">
        <div class="mostly-title">
          <h2>Mostly watched</h2>
        </div>
        <div class="mostly-images">
         <img src="C:\Users\Kushi\Desktop\web\Project\OTT\images\mostlyimg1.jpeg" alt="">
         <img src="C:\Users\Kushi\Desktop\web\Project\OTT\images\mostlyimg2.jpeg" alt="">
         <img src="C:\Users\Kushi\Desktop\web\Project\OTT\images\mostlyimg3.jpeg" alt="">
         <img src="C:\Users\Kushi\Desktop\web\Project\OTT\images\mostlyimg4.jpeg" alt="">
         <img src="C:\Users\Kushi\Desktop\web\Project\OTT\images\mostlyimg5.jpeg" alt="">
         <img src="C:\Users\Kushi\Desktop\web\Project\OTT\images\mostlyimg6.jpeg" alt="">
         <img src="C:\Users\Kushi\Desktop\web\Project\OTT\images\mostlyimg7.jpeg" alt="">
         <img src="C:\Users\Kushi\Desktop\web\Project\OTT\images\mostlyimg8.jpeg" alt="">
         <img src="C:\Users\Kushi\Desktop\web\Project\OTT\images\mostlyimg9.jpeg" alt="">
         <img src="C:\Users\Kushi\Desktop\web\Project\OTT\images\mostlyimg10.jpeg" alt="">
         
        </div>
      </div>
      <!-- Mostly watched movies ends -->
      

      <!-- Trending movies starts-->
      <div class="trending" id="trending">
        <div class="trending-title"><br><br><br><br><br>
          <h2>Trending Movies</h2>
        </div>
        <div class="trending-images">
         <img src="C:\Users\Kushi\Desktop\web\Project\OTT\images\trending10.jpeg" alt="">
         <img src="C:\Users\Kushi\Desktop\web\Project\OTT\images\trending(1).jpeg" alt="">
         <img src="C:\Users\Kushi\Desktop\web\Project\OTT\images\trending2.jpeg" alt="">
         <img src="C:\Users\Kushi\Desktop\web\Project\OTT\images\trending3.jpeg" alt="">
         <img src="C:\Users\Kushi\Desktop\web\Project\OTT\images\trending4.jpeg" alt="">
         <img src="C:\Users\Kushi\Desktop\web\Project\OTT\images\trending5.jpeg" alt="">
         <img src="C:\Users\Kushi\Desktop\web\Project\OTT\images\trending6.jpeg" alt="">
         <img src="C:\Users\Kushi\Desktop\web\Project\OTT\images\trending7.jpeg" alt="">
         <img src="C:\Users\Kushi\Desktop\web\Project\OTT\images\trending8.jpeg" alt="">
         <img src="C:\Users\Kushi\Desktop\web\Project\OTT\images\trending9.jpeg" alt="">
        </div>
      </div>

      <!-- Trending movies ends -->

      <!-- about starts -->
      <div class="abt" id="abt">
        <div class="company">
            <h3 align="center">Company</h3>
            <p align="center">
                About us <br>
                Careers <br>
                <br>
                All rights reserved <br><br>
  
                Terms of use &nbsp;&nbsp;Privacy policy&nbsp;&nbsp;FAQ
            </p>
        </div>
        <div class="viewin"> 
            <h3 align="center">View In</h3>
            <p align="center">English</p>
        </div>
        <div class="needhelp">
            <h3 align="center">
                Need help ?
            </h3>
            <p align="center">
                visit help center <br>
                share feedback
            </p>
        </div>
        <div class="contact"> 
            <h3 align="center">Contact us</h3><br>
            <a href="https://www.facebook.com/"></a><img src="C:\Users\Kushi\Desktop\web\Project\OTT\images\download.png" alt="">   
            <a href="https://twitter.com/"></a><img src="C:\Users\Kushi\Desktop\web\Project\OTT\images\download (1).png"alt="">
            <a href="https://www.instagram.com/"></a><img src=C:\Users\Kushi\Desktop\web\Project\OTT\images\download.jpeg alt="">
            <br><br>
            <a href=""></a><img src="C:\Users\Kushi\Desktop\web\Project\OTT\images\download (2).png" alt=""  style="margin-left: 100px;">
            <a href=""></a><img src="C:\Users\Kushi\Desktop\web\Project\OTT\images\download (3).png" alt="">
        </div>
    </div>
</body>
</html>
