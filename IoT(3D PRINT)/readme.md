<h1> ๐งฑ3D Modeling & Printing </h1>

๐ **IoT System์ ์ ํํ ์๊ณ ๋ฆฌ์ฆ ๋์์ ์ํ ํ๊ฒฝ ์กฐ์ฑ๊ณผ IoT(Raspberry Pi)๋ฅผ ๊ฑฐ์นํ  ๊ตฌ์กฐ๋ฌผ์ ๋ง๋ค๊ธฐ ์ํด 3D Print๊ธฐ์ ์ ์ฌ์ฉํ์ต๋๋ค.**

<table>
    <tr>
        <td width="30%">
            <img src="/IoT(3D PRINT)/asset/new_all2.png">
        </td>
        <td width="35%">
            <img src="/IoT(3D PRINT)/asset/3d_gif.gif">
        </td>
	       <td width="30%">
            <img src="/IoT(3D PRINT)/asset/modelreal.jpg">
        </td>
    </tr>
    <tr>
        <td align="center">
            3D Model
        </td>
        <td align="center">
            3D Model Flow GIF
        </td>
	<td align="center">
            Real 3D Print 
        </td>
    </tr>
</table>

                                                                      
                                                                      
                                                                      
<h2>๐ง3D Printing ์ค๊ณ ๋ฐ ์ถ๋ ฅ</h2>
<br>
                                                                    

โจ **์ค๊ณ๋ฅผ ํ ๋ ์ฃผ์ ๊ณ ๋ คํด๋ ์ฌํญ**
* ์ถ๋ ฅ์ ์๋๋ฅผ ๊ณ ๋ คํ ์ค๊ณ
* ๋น์ด ์ ํตํ๋ ๊ตฌ์กฐ
* ์ฅ๊ธฐ๊ฐ(24์๊ฐ ์ด์) ์ฌ์ฉ ์ ๋ธ์ฆ์ ์์์ผ๋ก ์ ์์ ์ธ ์ถ๋ ฅ์ด ๋ถ๊ฐํ ๊ฒฝ์ฐ ๊ณ ๋ ค
* ๋ถํ ๊ฒฐํฉ์ ๊ณ ๋ ค
* ์ ์ฉ ์นด๋ฉ๋ผ์ ๋ฐ๋ฅ์ ์์ง์ ๊ฑฐ๋ฆฌ    
                                                                    
๐จ **์ถ๋ ฅ์ ์ธ๋ถ ์ฌํญ**
* ์ฑ์์ ์ ๋ 0%
* ์ธ๋ฒฝ์ ๋๊นจ 1~0.5 mm
* ์ถ๋ ฅ ์๋๋ ํด๋น ๊ธฐ๊ณ์ ์ต๊ณ  ์๋
                                                                    
๐จ **์ถ๋ ฅ ํ๊ฒฝ**
* STL ์ ์ : Tinkercad ์ฌ์ฉ
* G-code์์ฑ : CURA ์ฌ์ฉ 
* 3D Printer : Ultimaker็คพ
* Total Time : 36h                                                                    




<h2>๐จ๋ถ์ํ ์๊ฐ</h2>
                                                                    
|์ข๋ฅ|์ธ๋ถ ๋ถ์๋ฌผ
|:-----:|:-----:|
|TOP(4ea)|TOP_center, TOP_center_front, TOP_left, TOP_right
|BOTTOM(3ea)|BOTTOM_center, BOTTOM_left, BOTTOM_right
|PILLAR(8ea)| PILLAR x 8


<br><br>
<h3>top_center.stl</h3>

>๋ผ์ฆ๋ฒ ๋ฆฌํ์ด์ ์นด๋ฉ๋ผ๊ฐ ์ฌ๋ผ๊ฐ๋ ๋ถ์ํ, <br>
>๊ตฌ์กฐ๋ฌผ์ ์ต์๋จ์ ์์นํด ์ง๋ถ์ ์ญํ <br>
<img src="/IoT(3D PRINT)/asset/new_top1.png">
 
  ___
 
<h3>bottom.stl</h3> 

>์ํ์ ๋๊ณ , ๊ตฌ์กฐ๋ฌผ์ ์งํฑํ๋ ๋ถ๋ถ <br>
>๊ตฌ์กฐ๋ฌผ์ ํ๋จ์ ์์นํด ๊ตฌ์กฐ๋ฌผ์ ์ฃผ์ถง๋ ์ญํ  <br>
<img src="/IoT(3D PRINT)/asset/new_bottom1.png">

 ___
 
<h3>pillar.stl</h3>

>์ด 6๊ฐ์ ๊ธฐ๋ฅ์ผ๋ก top์ bottom์ ์ด์ด์ฃผ๋ ์ญํ 
<br>
<img src="/IoT(3D PRINT)/asset/pill.png">
  
<h2>๐ฉ๋ถ์ํ์ ๊ฒฐํฉ ๋ฐ ๊ตฌ์กฐ๋ฌผ ์๊ฐ </h2>
<h3>Raspberry PI ์ top๋ถ๋ถ ๊ฒฐํฉ </h3>

>Top ๋ถ์ํ Center์ ์ ์ฉ ์นด๋ฉ๋ผ๋ฅผ ๋ถ์ฐฉํ  ์ ์๋ ๊ตฌ๋ฉ์ด ์๋ค. <br>
>์ด ๋ถ๋ถ์ ์ ์ฉ ์นด๋ฉ๋ผ๋ฅผ ๊ฒฐํฉํ๊ณ  ๋ผ์ฆ๋ฒ ๋ฆฌํ์ด์ ์ ์ฉ ์คํฌ๋ฆฐ์ Top๋ถ์ํ์ ๋ถ์ฐฉ์ํค๋ฉด ๋๋ค.<br>
>โป IoT ๋ถ๋ถ ๊ตฌ์ฑ : Raspberry Pi,์ ์ฉ ํฐ์น ์คํฌ๋ฆฐ,์ ์ฉ ์นด๋ฉ๋ผ <br>
<img src="/IoT(3D PRINT)/asset/rasp1.png">
  
 ___
 
<h3>Top & Bottom ๋ถ์ํ ๊ฒฐํฉ </h3>

>Top Center & Top Left & Top Right & Top Center2 ๊ฒฐํฉ <br>
>Top์ 4๊ฐ์ง ๋ถ์ํ์ ๊ฒฐํฉํ๋ ๊ณผ์ 
<img src="/IoT(3D PRINT)/asset/bottom_all.png" width="100%" height="100%">

>bottom Center & bottom Left & bottom Right ๊ฒฐํฉ <br>
>bottom์ 3๊ฐ์ง ๋ถ์ํ์ ๊ฒฐํฉํ๋ ๊ณผ์ 
<img src="/IoT(3D PRINT)/asset/top_all.png" width="100%" height="100%">

<h3> ๊ฒฐํฉ ์๋ฃ </h3>
<div align="center">
<img src="/IoT(3D PRINT)/asset/new_all2.png" width="40% height="40%">
<img src="/IoT(3D PRINT)/asset/3d_gif.gif" width="47% height="47%">
</div>                                                                     
                                                                      
