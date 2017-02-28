---
title: Data at the Table
author: Pat Meehan | PS Analytics Consulting
mode : selfcontained
framework: revealjs
hitheme : tomorrow
revealjs:
  theme: default
  transition: linear
  center: "true"
url: {lib: "."}
# bootstrap:
#   theme: amelia
--- .custom1

<!-- try to create slides at https://slides.com/lajfe9/new - see if I can 
figure out code to customize transitions by slide -->
<!-- how to print pdf example:  http://lab.hakim.se/reveal-js/?print-pdf#/ -->
<link href="http://fonts.googleapis.com/css?family=Bebas Neue" rel="stylesheet" type="text/css">
<link href="http://fonts.googleapis.com/css?family=League Gothic" rel="stylesheet" type="text/css">
<link href='http://fonts.googleapis.com/css?family='Open Sans' rel='stylesheet' type='text/css'>


<style>
.reveal h1,
.reveal h2,
.reveal h3,
.reveal h4,
.reveal h5,
.reveal h6 {
  margin: 0 0 20px 0;
  color: white; /*#eee8d5;*/
  font-family: "League Gothic", Impact, sans-serif;
  line-height: 0.9em;
  letter-spacing: 0.02em;
  text-transform: uppercase;
  text-shadow: none; }
.reveal h3 {
  text-transform: none;
}
/* FROM frameworks/revealjs/css/theme/default.css  - can edit colors for links here*/
.reveal a:not(.image) {
  color: #13daec;
  text-decoration: none;
  -webkit-transition: color 0.15s ease;
  -moz-transition: color 0.15s ease;
  -ms-transition: color 0.15s ease;
  -o-transition: color 0.15s ease;
  transition: color 0.15s ease; }
.reveal a:not(.image):hover {
  color: #71e9f4;
  text-shadow: none;
  border: none; }
.reveal .roll span:after {
  color: #fff;
  background: #0d99a5; }
.reveal blockquote {
	display: block;
	position: relative;
	width: 85%;
	margin: 5px auto;
	padding: 5px;
	font-style: italic;
	background: rgba(255, 255, 255, 0.05);
	box-shadow: 0px 0px 2px rgba(0,0,0,0.2);
	color: #71e9f4;
	font-size: 1.3em;
}
.longer blockquote {
	display: block;
	position: relative;
	width: 85%;
	margin: 5px auto;
	padding: 5px;
	font-style: italic;
	background: rgba(255, 255, 255, 0.05);
	box-shadow: 0px 0px 2px rgba(0,0,0,0.2);
	color: #71e9f4;
	font-size: 1.35em;
}

<!-- .reveal h2 {  -->
<!--   font-size: 3em;  -->
<!--   font-family: 'Bebas Neue', sans-serif; -->
<!-- } -->
/* MY CUSTOMIZATIONS */
.custom1 h1 {
  margin: 0 0 20px 0;
  color: white; /*#eee8d5;*/
  font-family: "League Gothic", Impact, sans-serif;
  font-size: 2.5em;
  line-height: 0.9em;
  letter-spacing: 0.02em;
  text-transform: uppercase;
  text-shadow: none; 
  }
.custom2 {
  <!-- background-color: #777; -->
  font-family: 'Open Sans', Impact, sans-serif;
  font-weight: 700;
  }
.custom2 h1 {
  color: white;
  text-align: center;
  }
.custom2 h2 {
  text-transform: none;
  font-family: 'Open Sans Condensed', Impact, sans-serif;
  color: white;
  font-weight: 700;
  font-size: 70px;
  text-align: center;
  padding-top: 100px;
  }
.custom2 h3 {
  color: white;
  text-align: center;
  font-weight: 700;
  }
<!-- .custom2 ul { -->
<!--   padding-left: 100px; -->
<!-- } -->
.custom2 li {
  font-size: 120%;
  font-weight: 700;
  line-height: 175%;
}
.custom2 li::before {
  font-size: 1.5em;
  left: 2.5em;
  }
.custom3 h1 {
  color: white;
  text-align: center;
  }
.custom3 h2 {
  color: #71e9f4; /*maroon;*/
  font-weight: 700;
  font-size: 62px;
  text-align: center;
  text-transform: none;
  letter-spacing: 0.01em;
  font-family: 'Open Sans Condensed', sans-serif;
  }
.custom3 h3 {
  color: white; /*#333;*/
  font-family: 'Open Sans', Impact, sans-serif;
  font-size: 34px;
  font-weight: 700;
  text-align: center;
  <!-- margin-top: 100px; -->
} 
.custom3 p {
  color: #999;
  font-size: 70%;
}
<!-- .custom4 { -->
<!--   background-color: white; /*#777;*/ -->
<!--   font-weight: 700; -->
<!--   } -->
<!-- .custom4 h1 { -->
<!--   color: white; -->
<!--   text-align: center; -->
<!--   } -->
<!-- .custom4 h2 { -->
<!--   color: white; -->
<!--   font-weight: 700; -->
<!--   font-size: 70px; -->
<!--   text-align: center; -->
<!--   padding-top: 175px; -->
<!--   } -->
.custom4 ol {
  background-color:#777; 
  color:white; 
  font-weight:bold; 
  padding:40px;
  border-radius:1%;
}
.custom4 li {
  padding-bottom:10px;
  padding-left:10px;
  margin-left:40px;
  color:white;
  font-size:1em; 
}
.custom5 {
  <!-- background-color: #777; -->
  font-family: 'Open Sans', sans-serif;
  font-weight: 700;
  }
.custom5 h1 {
  color: white;
  text-align: center;
  }
.custom5 h2 {
  text-transform: none;
  font-family: 'Open Sans', Impact, sans-serif;
  letter-spacing: 0.01em;
  color: white;
  font-weight: 700;
  font-size: 120%;
  text-align: center;
  padding-top: 100px;
  }
.custom11 {
  color: white;
}
.thankyou {
  background: white;
}
.thankyou h1{
  text-align: center;
  text-transform: none;
  font-family: 'Open Sans', Impact, sans-serif;
  font-size:80px;
  font-weight: 700;
  padding-top: 3em;
}
.thankyou center {
  line-height: 20px;
}
.addvert {
  padding-top: 275px;
}
.remvert {
  padding-top: -100px;
}
.larger p{
  font-size: 200%;
}
.nobull {
  list-style: none;
}
.lightgrey { 
  color: lightgrey;
}
.darkgrey {
  color: #333;
}
.aqua {
   color: #71e9f4;
}
.lightblue {
  color:#B2DFEE;
}
/*flowchart layout*/
#flow {
  background-color: white;
  font-weight: 700;
  font-family: 'Open Sans';
  }
#flow p {
  font-size: 22px;
}
#flow h2 {
  color: maroon;
  font-weight: 700;
  font-size: 52px;
  text-align: center;
  padding-top: 50px;
  }
#flow h1{
  <!-- border: solid 7px #333; -->
  width: 225px;
  height: 225px;
  border-radius: 50%;
  text-align: center;
  line-height: 30px;
  font-size:36px;
  color: maroon;
  font-family: 'Open Sans', sans serif;
}
#flow h5{
  border: dotted 3px maroon;
  width: 225px;
  height: 225px;
  border-radius: 10%;
  text-align: center;
  line-height: 30px;
  font-size:26px;
  font-weight:bold;
}
#flow table {
  border: none;
  width: 100%;
  border-collapse: collapse;
  font-size: 24px;
  line-height: 32px;
  font-family: 'Open Sans'; /*'Bebas Neue';*/
  font-weight: bolder;
  color: maroon;   /*rgb(102, 102, 102);*/
}
#flow table thead {
  border-top: 1px solid #BFBEAD;
  border-bottom: 1px solid #BFBEAD;
}
#flow table th, table td, table caption {
  margin: 0;
  padding: 2pt 6pt;
  text-align: left;
  vertical-align: top;
}
#flow table th {
  background:  #333;  /*#CFCEBD; not nec*/
  color: #575400;
  text-transform: uppercase;
}
#flow table td {
  border-bottom: 1px solid #CFCEBD;
}
#flow table tr:nth-child(2n+1) {
/*  background: #E8F2FF; */
  background: lightgrey;/*soft red #F9EBEE;*/   /*#EFEEDD;*/
}
#flow h3 {
  color: #333;/*maroon;*//*#333;*/
  font-weight: 700;
  text-align: center;
  margin-top: -60px;
 }
 <!-- #flow p { -->
 <!--  color: white; -->
 <!--  font-weight: 700; -->
 <!--  font-size:20px; -->
 <!--  text-align: center; -->
 <!--  font-family: 'Open Sans'; -->
 <!-- } -->
 #flow h4 {
  border: solid 7px #333;
  width: 225px;
  height: 225px;
  border-radius: 50%;
  text-align: center;
  line-height: 30px;
  font-size:18px;
  font-family: 'Open Sans', sans serif;
  color: white;
 }
 #flow h1 {
   font-family: 'Open Sans', sans serif;
}
</style>

# Data at the Table

<small> Pat Meehan | [PS Analytics Consulting](http://psanalyticsconsulting.com) </small>

<script src="http://ajax.googleapis.com/ajax/libs/jquery/1.9.1/jquery.min.js"></script>

*** =pnotes

Some notes on the first slide

--- .larger

# QUEM 

.fragment Quality Evidence Matters

*** =pnotes
Did you know that there is a new debate about how to survive a riptide?  My 
husband is from Hawaii and I (have to) visit regularly to see all of my in-laws.  I've learned a lot about local perspectives on the ocean. 

---  #flow

<!-- ## <span style="padding-bottom:-50px">PS Analytics Consulting</span> -->
<span style="font-family:'Open Sans'; font-size:2em; color:maroon">PS Analytics Consulting</span>

<span style="font-family:'Open Sans'; color:#333"><i>Supporting leadership teams with 
custom analytics</i></span>

<!-- ### *Supporting leadership teams with custom analytics* -->

</br></br></br>
<table>
<tr>
<td style="padding-left:50px;"><h4>3294839</br> JFRghl9LJO#%YES</br> (D*GDVLDJOFIJgrade<br> yr2016ES4Mathplan </br> MF83PA#&SWD89ADV</br> ELAjo74398lang </br> SIP3>4873 </h4></td>
<td style="font-size:36px;"></br></br></br>&#8594</td>
<td><h5></br></br>
<span style="color:maroon;">Statistician</br>&</br>Developer</span></h5></td>
<td style="font-size:36px;"></br></br></br>&#8594</td>
<td><p style="font-size:24px"><h4></br></br></br>Custom Tools</h4></p></td>
</tr>
</table>

--- {class: custom2, bg: "#007777", bt: zoom}

<h2 style="margin-top:-100px;">The Same Message for All</h2>

<center>
<img src="./assets/img/heads with data.png" height=400 width=400 class="imgframe"/>
</center>

*** =pnotes
### Causes of Data Misinformation

Difference in domain expertise, aggregation obscures truth

9 Causes of Data Misinterpretation (Information Week article)
1. Insufficient domain expertise
2. Important variables are ommitted (gender - is it that boys show lower reading performance or kids who sit in the back of the class?)
3. Aggegation obscures truth
4. Inferences are off base  (all are conditional on the group studied)
5. Sources of variation overlooked (after or before-school programs; desk neighbors in classroom; scheduling conflicts for services that interfere with, say, library time)
6. Statistical thinking trumps thinking (testing many hypothesis in search of *significance)
7. Numerical analysis missed something.  (Data visualizations can reveal anomalies that could be overlooked in numerical analysis.  Outliers are immediately obvious visually.  Nonlinear relationships result in a small correlation coefficient but are easy to recognize visually.)
8. Correlation is mistaken for causation.  (Journal stated: eye color a potential indicator of alcohol dependence among European Americans.  
9. Explanation adds distortion.  (Jargon may sound scientific but may also confuse the audience.)

---

</br>
<center>
<img src="./assets/img/digital-capability.png" height=400 class="imgframe"/>
</center>

<p class="fragment" style="font-size:.8em"> domain knowledge &nbsp;&nbsp;&nbsp; personal beliefs &nbsp;&nbsp;&nbsp;teaching background</p>

<h3 class="fragment" style="padding-bottom:5em; color:#71e9f4">prior experiences</h3>

*** =pnotes
<h3 style="font-size:36px; color:darkslategrey; font-weight:700">How do leadership teams create strategic plans?</h3>

---
 
##  Decision Neuroscience

.fragment <span class="aqua" style="text-transform: none;">Not just what but how</span>

</br>
<center>
<img src="./assets/img/emoji_hmm2.png" height=200 width=200/>
</center>

</br>

&bull; Perception &nbsp;&nbsp;&nbsp; &bull; Cognition &nbsp;&nbsp;&nbsp; &bull; Time to Decision

--- 
### What's your takeaway?

</br>
<center>
<img src="./assets/img/MA MCAS table.png" height=500 />
</center>

*** =pnotes
Add a graph - 
Sample data and/or dashboard.  Not longitudinal, without clear anchor (g4 math MA).

---

## Buddha

</br></br>
> Nothing ever exists entirely alone. Everything is in relation to everything else.

</br></br></br>
<!-- .fragment Agree:  Tufte, Cleveland, Tukey, Few, Kahneman -->
.fragment <span style="text-transform: none; font-size:30px; color:#999;">Agree:  Tufte, Cleveland, Tukey, Few, Kahneman</span>


*** =pnotes
Others who agree:  Edward Tufte, William Cleveland, John Tukey, Stephen Few, Daniel Kahneman

Few - perceptualedge.com

--- .custom3

</br>
## Interactive Visuals 

</br></br></br></br></br>
<em>
<h3 style="font-size:1.4em; color:white;">Overview first, </h3>
<h3 style="font-size:1.8em; color:white;">zoom and filter, </h3>
<span style="font-size:1.2em; color:white;">then details on demand</span>
</em>

<!-- </br></br> -->
<!-- <span style="font-size:32px; color:white; text-align:center">*Overview first, zoom and filter, then details on demand*</span> -->

</br></br></br></br></br></br></br>
*Ben Schneiderman, University of Maryland Human-Computer Interaction Lab

--- .custom2

## Graphical Principles of PSA

</br></br>
<center style="color:#71e9f4; font-weight:700;">
Focused &nbsp; | &nbsp; Clear &nbsp; | &nbsp; Anchored &nbsp; | &nbsp; Layered
</center>

*** psnotes
Can't just build.  Need to understand something about how humans perceive information depending on presentation choices and how anchors help them make sense of it.  Now we have a philosophy of graphical design that provides focus, clarity, and anchors so that key information is nonignorable.  And details are persuable.  

--- {class: custom4, bg: white}

<!-- <i class="fa fa-cog" style="color:#333; font-size:84px;"></i> -->
<!-- <i class="fa fa-cog" style="color:darkslategrey; font-size:42px;"></i> -->
<!-- <i class="fa fa-cog" style="color:#444; font-size:54px;"></i> -->

<ol> 
<li class="odd">No software purchase - open source R </li>
<li class="even">Easily reproducible & updatable - script-based </li>
<li class="odd">Extendable - modularized </li>
<li class="even">Hosted locally or web-based </li>
<li style="color:#71e9f4">Informed by a statistics perspective </li>
</ol>

</br>
<center style="color:maroon; font-style:italic;">**Visual, interactive, and easy to share**</center>

*** pnotes
<center style="color:darkslategrey; font-style:italic;">**Not just a tool, not just data ... a scientific approach to insight.**</center>

*"Provide a product that is scientific and data-driven and can help people" (Julie Woo, Chief Data Scientist, pymetrics) [WIDS, Stanford, 2017]

--- .custom5

## Ongoing communication and guidance ...

</br>
<center>
<img src="./assets/img/Ed Leadship Data issue - 2009.jpg" height=250/></br>
**2009**
</center>

*** pnotes
List titles of articles; what's been done since?


--- {class: custom2, bg: "#777"}

## Ready for analytics by design?

</br>
> - .darkgrey Do you know your questions?
> - .lightgrey Do you have relevant data?
> - .darkgrey Committed to data at the table?


--- {class: thankyou, bg: white}

<h1 style="color:#333">thank<span style="color:lightslategrey">you</span></h1>

</br></br></br></br></br>
<center>
<span style="color:darkslategrey; font-size: 20px; font-family="Open Sans;">
Pat Meehan | PS Analytics Consulting </span> </br>
<span style="color:darkslategrey; font-size: 20px; font-family="Open Sans; 
display:none;">
meehanpm@psanalyticsconsulting<span>.</span>com
</span>
</center>

--- .longer

> I cannot define the real problem, therefore I suspect there's no real problem, but I'm not sure there's no real problem.

<span style="padding-left:10em">Richard Feynman, physicist


*** =pnotes
Feynman was speaking about quantum mechanics (short defn).  A recent BBC article questioned whether the same might be true of consciousness.  I suggest that could also be true of leaders on the precipice of an analysis plan. 

http://www.bbc.com/earth/story/20170215-the-strange-link-between-the-human-mind-and-quantum-physics

