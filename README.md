# 
<html>
    <head>
    <meta name="viewport" content="width=device-width, initial-scale=1">
    </head>
    <style>
        body{
            margin:0;
            font-family: 'Lato',sans-serif;
        }
        .zemin{
            height: 100vh;
            width: 100vw;
            position: fixed;
            z-index:1;
            top:0;
            left:-100vw;
            background: rgba(0,0,0,.9);
            overflow-x: hidden;
            transition: .5s;
        }
        .zemin-icerik{
            position: relative;
            top:25%;
            width: 100%;
            text-align: center;
        }
        
        .zemin a{
            display: block;
            padding:8px;
            text-decoration: none;
            color:#818181;
            transition: .4s;
            font-size:36px;
            border-top:solid 2px rgba(241,241,241,0);
            border-bottom:solid 2px rgba(241,241,241,0);
        }
        
        .zemin-icerik a:hover, .zemin-icerik a:focus{
            color:#f1f1f1;
            border-top:solid 2px #f1f1f1;
            border-bottom:solid 2px #f1f1f1;
            background: #b71540;
        }
        .zemin .kapatBtn{
            position: absolute;
            top:40px;
            right: 40px;
            font-size:60px;
        }
    </style>
    <title>MyWorld</title>

    <body bgcolor="#000000">
    <div id="menu" class="zemin">
        <a href="#" class="kapatBtn" id="kapatBtn"> <font color="#FF0000">&times</font></a><font color="#FF0000">
		</font>
        <div class="zemin-icerik">
            <a href="index.htm"><font color="#FFFFFF" size="5">
			<a href="index.htm"><font size="5" color="#FFFFFF">Anasayfa</font></a></font></a><font color="#FFFFFF" size="5">
			<a href="index2.htm"><font size="5" color="#FFFFFF">Haber </font>
			</a><a href="index3.htm"><font size="5" color="#FFFFFF">Sohbet</font></a>
			<a href="index4.htm"><font size="5" color="#FFFFFF">İndir</font></a>
			<a href="index5.htm"><font size="5" color="#FFFFFF">Hakkımda</font></a>
			</font>
        </div>
    </div>    
    <span id="menuAc"> <b><font size="4" color="#FFFFFF">&#9776;</font></b><font color="#FFFFFF">
	</font> <font size="4" color="#FFFFFF">Menü</font></span>
        
    <p></p>
        <script>
         var menuAc=document.querySelector("#menuAc");
         var menu=document.querySelector("#menu");
         var kapatBtn=document.querySelector("#kapatBtn");
            
            menuAc.addEventListener("click",function(){
               menu.style.left="0vw"; 
            });
            
            kapatBtn.addEventListener("click",function(){
                menu.style.left="-100vw"; 
            });
            
        </script>
    </body>
</html>
