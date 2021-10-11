---
layout: default
title: 私の絵の記録　第4項
description: PCで描いた絵をここに記録します。
lang: ja_JP
---
<hedar>
<link rel="stylesheet" href="style.css">
<h1>4項目</h1>
<p>*献立
-<a href="https://itou332.github.io/">1項目</a>
-<a href="https://itou332.github.io/itou332a.github.io/">2項目</a>
-<a href="https://itou332.github.io/diary">3項目</a>
-<a href="http://itou33good.starfree.jp/?page_id=234">免責事項</a>
-<a href="https://github.com/itou332">my github</a>
-<a href="http://itou33good.starfree.jp/">itou</a>
</p>
</hedar>
<head>
<?xml version="1.0" encoding="UTF-8" standalone="no"?>
<!-- Created with Inkscape (http://www.inkscape.org/) -->
<!-- icon imge-->
<link rel="icon" href="img/favicon.svg" type=aoihata.svg"/svg+xml">
<meta http-equiv="Content-Type"content="text/html;charset=utf-8">
<body>
<hr>
<h2>-絵を記録します。</h2>

<h3>2021.10/8</h3>

<corde>
<canvas id="myCanvas" width="150" height="150"></canvas>
<script>
var canvas = document.getElementById('myCanvas');
var context = canvas.getContext('2d');


for(var x=0;x<700;x++)
{
        for(var y=0;y<600;y++)
        {
                var i= -4;
                var cx=-2+x/50;
                var cy=-2+y/50;
                var zx=0.06;
                var zy=0.04; 
                var z =zx*zy*i                       

                do
                {
                        var xt=zx*zy;
                        zx=zx*zx-zy*zy+cx;
                        zy=2*xt+cy;
                        i++;

                        
                }
                while(i<255&&(zx*zx+zy*zy)<4);

                var color=i.toString(8);
                context.beginPath();
                context.rect(zx*x*color,(i*y+(z*zy*zy*i))/(zx+zy),(z*zy*zy*i)*30,i*i);
                context.fillStyle ='#'+color+color+color;
                context.fill();
                
        }
        
}

</script>
</corde>

</body>
<footer>
*献立
-<a href="https://itou332.github.io/">1項目</a>
-<a href="https://itou332.github.io/itou332a.github.io/">2項目</a>
-<a href="https://itou332.github.io/diary">3項目</a>
-<a href="http://itou33good.starfree.jp/?page_id=234">免責事項</a>
-<a href="https://github.com/itou332">my github</a>
-<a href="http://itou33good.starfree.jp/">itou</a>
  <svg xmlns="http://www.w3.org/2000/svg" width="200" height="250">
                <text x="0" y="30" transform="rotate(45 40,40)">
                  Copyright © 2021 itou Inc. All Rights Reserved.
                </text>
</footer>
