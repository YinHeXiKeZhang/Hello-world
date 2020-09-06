# Hello-world
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>MY GAME</title>
    <style>
         body{background-image:url(../素材/timg.jpg);
            background-attachment: fixed;
            background-repeat: no-repeat;
            background-size: cover;
         }
         .fr0{
             height: 120px;
             margin: 0px auto;
         }
        .fr{
            height: 120px;
            width: 100%;
            margin: 0px auto;
            box-shadow: 0px 8px 16px 0px rgba(0, 0, 0, 0.63);
        }

        .fr1{
            width: 200px;
            height: 100px;
            position: relative;
            top: 10px;
            left: 400px;
        }
        .fr2 {
        position: relative;
            top: -50px;
            left: 700px;
        display: inline-block;
        }
        .fr3 {
        display: none;
        position: absolute;
        background-color: #f9f9f9;
        min-width: 160px;
        box-shadow: 0px 8px 16px 0px rgb(0, 0, 0);
        padding: 12px 16px;
        cursor:hand;
        }
        .fr2:hover .fr3 {
         display: block;
        }

        .fr4 {
        position: relative;
            top: -50px;
            left: 750px;
        display: inline-block;
        }
        .fr5 {
        display: none;
        position: absolute;
        background-color: #f9f9f9;
        min-width: 160px;
        box-shadow: 0px 8px 16px 0px rgb(0, 0, 0);
        padding: 12px 16px;
        }
        .fr4:hover .fr5 {
         display: block;
        }

        .fr6{
            font-size: 15px;
            height: 30px;
            width: 100px;
            position: relative;
            top: -110px;
            left: 1100px;
            background-color: rgba(65, 109, 22, 0.521);
        }
        .fr7{
            margin: 5px 20px;
        }

        .fr8{
            color: white;
            position: relative;
            top: 5px;
        }
        .tw{
            height:500px ;
            width: 1600px;
            margin: 0px auto;
            display: none;
        }
        .tw2{
            height: 500px;
            width: 1600px;
        }
        .th{
            height: 400px;   
        }
        .th0{
            height: 400px;
            width: 1600px;
        }
        .th1{
            height: 200px;
            width: 300px;
        }
        .th1{
            float: left;
            margin: 70px 100px;
        }
        .img1{
            display: block;
            height: 250px;
            width: 350px;
            box-shadow: 0px 8px 16px 0px rgb(0, 0, 0);
        }
        .img2{
            display: none;
            height: 250px;
            width: 350px;
            box-shadow: 0px 8px 16px 0px rgb(0, 0, 0);
            position: relative;
        }
        .for{
            height: 250px;
            width: 1400px;
            box-shadow: 0px 8px 16px 0px rgb(0, 0, 0);
            margin:70px auto;
        }
        .six{
            height: 150px;
        }
        .six1{
            font-size: 50px;
            color: white;
        }
        .fif{
            height: 800px;
            width: 100%;
            position: relative; 
        }
        .fif1{
            margin: 5% auto;
            width: 100%;
            overflow: hidden; 
            height:600px;
            width: 1200px; 
            display: block; 
            line-height: 1; 
            z-index: 1;
            box-shadow: 0px 8px 16px 0px rgb(0, 0, 0);

        }
        .pic0{
            position: absolute;
            bottom:10px;
            left:44%;
            z-index: 2;
            list-style-type: none;
        }
        .pic0 li{
            display:inline-block;
            padding: 0 15px;
            font-size: 24px;
            color:#999; 
            cursor: pointer;
            z-index: 2;
        }
        .active1{
            font-size: 28px;
            color:#fff;
        }   
        
       .img3{
           display: block;
       }
       .img4{
           display: none;
       }
       .img5{
           display: none;
       }
       #img6{
           display: none;
       }
       
    </style>
</head>
<script src="../jq.min.js"></script>
<script>
      $(document).ready(function(){
        $('.tw').fadeIn(2000)
    })
</script>

<script>
    window.onload = function(){init();wheel()}
    

    function init(){
        var img1 = document.getElementById("img1");
        var img2 = document.getElementById("img2");
        var img3 = document.getElementById("img3");
        var img4 = document.getElementById("img4");
        var img5 = document.getElementById("img5");
        var img6 = document.getElementById("img6");
        var doclick1 = document.getElementById("doclick1");
        var doclick2 = document.getElementById("doclick2");
        var doclick3= document.getElementById("doclick3");
        var doclick4= document.getElementById("doclick4");
        
      
        
        img1.onmouseenter = seenter;
        img2.onmouseleave = seleave;
        img3.onmouseenter = seentertw;
        img4.onmouseleave = seleavetw;
        img5.onmouseenter = seenterth;
        img6.onmouseleave = seleaveth;
        doclick1.onclick = into1;
        doclick2.onclick = into2;
        doclick3.onclick = into3;
        doclick4.onclick = into8;
        img2.onclick = into4;
        img4.onclick = into6;
        img6.onclick = into7;
        
    }

    
    function seenter(){
        img1.style.display = 'none';
        img2.style.display = 'block';
    }

    function seleave(){
        img1.style.display = 'block';
        img2.style.display = 'none';
    }

    function seentertw(){
        img3.style.display = 'none';
        img4.style.display = 'block';
    }

    function seleavetw(){
        img3.style.display = 'block';
        img4.style.display = 'none';
    }

    function seenterth(){
        img5.style.display = 'none';
        img6.style.display = 'block';
    }

    function seleaveth(){
        img5.style.display = 'block';
        img6.style.display = 'none';
    }

    function into1(){
        window.location.href = "../实训/NEWS.html";
    }
  
    function into2(){
        window.location.href = "../实训/game.html";
    }
    function into3(){
        window.location.href = "../实训/install.html";
    }
  
    function into4(){
        window.location.href = "../实训/ZHILANG.html";
    }   
   
    function into6(){
        window.location.href = "../实训/CKXT.html";
    }   
    function into7(){
        window.location.href = "../实训/GMLY.html";
    }
    function into8(){
        window.location.href = "../实训/batter.html";
    }
   
       
       function wheel(){
        var lunbo = document.getElementById('fif');
        var imgs = lunbo.getElementsByTagName('img'); 
        var uls = lunbo.getElementsByTagName('ul');
        var lis = lunbo.getElementsByTagName('li');
        lis[0].style.fontSize = '26px';
        lis[0].style.color = '#fff';
        var pic_index = 1;
        var pic_time = setInterval(autobofang,3000);
        for(var i=0;i<lis.length;i++){ 
        lis[i].addEventListener("mouseover",change,false);
        }
    function change(event){ 
        var event=event||window.event;
        var target=event.target||event.srcElement; 
        var children = target.parentNode.children; 
        for(var i=0;i<children.length;i++){
        if(target == children[i]){ 
            picChange(i); 
            } 
        }
    } 
    function picChange(i){ 
        for(var j=0;j<imgs.length;j++){
            imgs[j].style.display = 'none'; lis[j].style.fontSize = '24px';
            lis[j].style.color = '#999';
        }
            imgs[i].style.display = 'block'; 
            lis[i].style.fontSize = '26px';
            lis[i].style.color = '#fff'; 
        }
    function autobofang(){
            if(pic_index >= lis.length){
            pic_index = 0;
        }
            change1(pic_index);
            pic_index++;
        }
    function change1(index){ 
        picChange(index);
        uls[0].addEventListener("mouseover",pause,false);
        uls[0].addEventListener("mouseout",go,false);
    }
    function pause(event){
        var event=event||window.event;
        var target=event.target||event.srcElement;

        switch(target.id){
        case "pic1":
        clearInterval(pic_time); 
        break;
        case "pic2":
        clearInterval(pic_time);
        break;
        case "pic3":
        clearInterval(pic_time);
        break;
        }
        }

function go(event){
var event=event||window.event;
var target=event.target||event.srcElement; 
switch(target.id){
case "pic1":
pic_index = 1; 
pic_time = setInterval(autobofang,3000);
break;
case "pic2":
pic_index = 2; 
pic_time = setInterval(autobofang,3000);
break;
case "pic3":
pic_index = 3; 
pic_time = setInterval(autobofang,3000); 
break;
}
}
}
</script>
<body>
    <div class="fr0">
    <div class="fr" style="background-color: rgba(197, 197, 196, 0.39);">
        <div class="fr1"><img src="../素材/6.png" style="width: 200px; height: 100px;"></div>
        <div class="fr2">
            <span>商店</span>
            <div class="fr3">
              <p>精选</p>
              <p id="doclick1" >新闻</p>
              
              <p id="doclick2">游戏</p>
            </div>
          </div>
        <div class="fr4">
            <span>社区</span>
            <div class="fr5">
              <p id="doclick4">推广</p>
              <p>设置</p>
              <p>创意工坊</p>
            </div>
        </div>
        <div class="fr6">
            <div class="fr7" align = center>
            <span class="fr8" id="doclick3">安装软件</span>
            </div>
        </div>
        </div>
    <div class="tw">
        <img src="../素材/促销2.png" class="tw2" id="doclick5">
    </div>
    <div class="th" align = 'center' >
        <div class="th0" align = 'center'>
        <div class="th1">
            <img src="../素材/只狼主1.jpg" id="img1" class="img1">
            <img src="../素材/只狼主2.png" id="img2" class="img2">
        </div>
        <div class="th1"> 
            <img src="../素材/刺客信条主1.jpg" id="img3" class="img1">
            <img src="../素材/刺客信条主2.jpg" id="img4" class="img2">
        </div>
        <div class="th1">
            <img src="../素材/古墓丽影主1.jpg" id="img5" class="img1">
            <img src="../素材/古墓丽影主2.jpg" id="img6" class="img2">
        </div>
    </div>
    </div>
    <div class="for">
        <img src="../素材/领贴纸.jpg" style="width: 1400px;height: 250px;" >
    </div>
    <div class="six" align = 'center'>
        <p class="six1">精选游戏</p>
    </div>
    <div class="fif" id="fif">
       <div class="fif1">
           <div class="fif2"><img src="../素材/CSGO轮播.jpg" alt="第一张图片"  style="width: 1200px;height: 600px;"></div>
           <div class="fif3"><img src="../素材/守望先锋轮播.jpg" alt="第二张图片" style="width: 1200px;height: 600px;"></div>
           <div class="fif4"><img src="../素材/求生之路轮播.jpg" alt="第三张图片" style="width: 1200px;height: 600px;"></div>
       </div>
       <ul class="pic0">
        <li id='pic1'>●</li>
        <li id='pic2'>●</li>
        <li id='pic3'>●</li>
        </ul>
    </div>
</body>
</html>
