# hellow-world
1st repository
testing how commit works


<!DOCTYPE html>
<html>
<head>
    <meta charset="utf-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <title>Test</title>
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/4.1.3/css/bootstrap.min.css">


<!-- Latest compiled JavaScript -->
<script src="https://maxcdn.bootstrapcdn.com/bootstrap/4.1.3/js/bootstrap.min.js"></script>
    <script src="https://ajax.googleapis.com/ajax/libs/angularjs/1.6.9/angular.min.js"></script>
  
        <style>
      
        body, html {
        height: 100%;
        width:100%;
        margin: 0;
        }

        .bg {
        /* The image used */
        height: 100%;
        width:100%;

        background-image: url("DesktopExample.jpg");
        background-position: center;
        background-repeat:no-repeat;
        background-size: contain;        
        }

        .absolute {
        position: absolute;
        top: 30%;
        right: 63%;
        width: 400px;
        height: 200px;       
        }

        .absolute1 {
        position: absolute;
        top: 30%;
        right: 54%;
        width: 400px;
        height: 200px;       
        }
        
        .absolute2 {
        position: absolute;
        top: 30%;
        right: 45%;
        width: 400px;
        height: 200px;       
        }
        
        .absolute3 {
        position: absolute;
        top: 30%;
        right: 36%;
        width: 400px;
        height: 200px;     
        }

        .absolute4 {
        position: absolute;
        top: 30%;
        right: 27%;
        width: 400px;
        height: 200px;      
        }

        .absolute5 {
        position: absolute;
        top: 50%;
        right: 57%;
        width: 400px;
        height: 200px;      
        }
        .absolute6 {
        position: absolute;
        top: 50%;
        right: 44%;
        width: 400px;
        height: 200px;       
        }

        .absolute7 {
        position: absolute;
        top: 50%;
        right: 29%;
        width: 400px;
        height: 200px;       
        }

        .absolute8 {
        position: absolute;
        top: 84%;
        right: 44%;
        width: 200px;
        height: 50px;             
        }

        div.gallery2 {        
        margin: 5px;       
        float: left;
        width: 200px;
        }

        div.gallery {              
        margin: 5px;        
        float: left;
        width: 140px;
        }

        .ctr {
        display: block;
        margin-left: auto;
        margin-right: auto;
        margin-top:23%;
        width: 20px;
        }
       
        div.gallery img {
            width: 100%;
            height: auto;
            opacity: 0.8;
        }
        
        </style>
   
    
</head>
<body class=" container bg" ng-app="myApp" ng-controller="myCtrl">

<!--CODE FOR THOSE 5 CIRCLES-->  
    
<div class="absolute gallery" ng-mousedown="myFunc()" ng-mouseup="nyFunc()" >
    <a  href="#">
      <img id="demo" src="never.png" alt="Cinque Terre" width="1000" height="1000">
    </a>
    
</div>  
<div class="absolute1 gallery" ng-mousedown="myFunc2()" ng-mouseup="nyFunc2()" >
    <a  href="#">
      <img id="demo2" src="occasionally.png" alt="Forest" width="300" height="200">
    </a>
    
</div>
  
<div class="absolute2 gallery" ng-mousedown="myFunc3()" ng-mouseup="nyFunc3()" >
    <a  href="#">
      <img id="demo3" src="4 hours.png" alt="Northern Lights" width="300" height="200">
    </a>
   
</div>
  
<div class=" absolute3 gallery" ng-mousedown="myFunc4()" ng-mouseup="nyFunc4()" >
    <a  href="#">
      <img  id="demo4" src="yearly.png" alt="Mountains" width="300" height="200">
    </a>
   
</div>
<div class="absolute4 gallery" ng-mousedown="myFunc5()" ng-mouseup="nyFunc5()"  >
    <a  href="#">
      <img id="demo5" src="never.png" alt="Cinque Terre" width="1000" height="1000">
    </a>
    
</div>

<!--CODE FOR THE ARROW-->

<div class="absolute5 gallery2" ng-click="hideIt()" >
      <img class ="ctr" id="img" src="arrow.png">       
</div>
<div class="absolute6 gallery2" ng-click="hideIt2()" >
      <img class= "ctr" id="img2" src="arrow.png" >      
</div>
<div class="absolute7 gallery2" ng-click="hideIt3()" >
      <img class= "ctr" id="img3" src="arrow.png">      
</div>

<!--CODE FOR THE TRY AGAIN BUTTON-->

<div class="absolute8 gallery3" ng-click="hideIt()" ></div>    
 
<script>
      var app=angular.module("myApp",[]);
      app.controller("myCtrl",function($scope){
        document.getElementById("img2").style.visibility="hidden";
        document.getElementById("img3").style.visibility="hidden";
        
        //FUNCTIONS FOR THE CIRCLES

          $scope.myFunc= function(){
               document.getElementById("demo").style.opacity=1;
               console.log("hello");
          }
          $scope.myFunc2= function(){
               document.getElementById("demo2").style.opacity=1;
          }
          $scope.myFunc3= function(){
               document.getElementById("demo3").style.opacity=1;
          }
          $scope.myFunc4= function(){
               document.getElementById("demo4").style.opacity=1;
          }
          $scope.myFunc5= function(){
               document.getElementById("demo5").style.opacity=1;
          }
          $scope.nyFunc=function(){
              document.getElementById("demo").style.opacity=0.8;
              console.log("sankar");
          }
          $scope.nyFunc2=function(){
              document.getElementById("demo2").style.opacity=0.8;
          }
          $scope.nyFunc3=function(){
              document.getElementById("demo3").style.opacity=0.8;
          }
          $scope.nyFunc4=function(){
              document.getElementById("demo4").style.opacity=0.8;
          }
          $scope.nyFunc5=function(){
              document.getElementById("demo5").style.opacity=0.8;
          }

//FUNCTIONS FOR THE ARROW & TRI AGAIN BUTTON

          $scope.hideIt=function(){
              document.getElementById("img").style.visibility="visible";
              document.getElementById("img2").style.visibility="hidden";
              document.getElementById("img3").style.visibility="hidden";
          }
          $scope.hideIt2=function(){
              document.getElementById("img").style.visibility="hidden";
              document.getElementById("img2").style.visibility="visible";
              document.getElementById("img3").style.visibility="hidden";
          }
          $scope.hideIt3=function(){
              document.getElementById("img").style.visibility="hidden";
              document.getElementById("img2").style.visibility="hidden";
              document.getElementById("img3").style.visibility="visible";
          }
          
      });
  </script>
</body>
</html>
