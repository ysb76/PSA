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
---

<!-- try to create slides at https://slides.com/lajfe9/new - see if I can 
figure out code to customize transitions by slide -->
<!-- how to print pdf example:  http://lab.hakim.se/reveal-js/?print-pdf#/ -->
<!-- <link href="http://fonts.googleapis.com/css?family=Bebas Neue" rel="stylesheet" type="text/css"> -->
<!-- <link href="http://fonts.googleapis.com/css?family=League Gothic" rel="stylesheet" type="text/css"> -->
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
.aqua {
   color: #71e9f4;
}
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
.larger p{
  font-size: 200%;
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

# Data on the Table

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

--- {id: custom5, bg: "#007777", bt: zoom}

## The Same Message for All

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

--- #custom1

</br></br>
<center>
<img src="./assets/img/digital-capability.png" height=400 class="imgframe"/>
</center>

.fragment domain knowledge &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; personal beliefs &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; teaching background

.fragment <h3 style="padding-bottom:5em; color:#71e9f4">prior experiences</h3>

*** =pnotes
<h3 style="font-size:36px; color:darkslategrey; font-weight:700">How do leadership teams create strategic plans?</h3>

<!-- --- #custom3 -->

--- {id: custom3, bg: "#007777", dt: zoom}
 
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
<img src="./assets/img/MA MCAS table.png" height=600 />
</center>

*** =pnotes
Add a graph - 
Sample data and/or dashboard.  Not longitudinal, without clear anchor (g4 math MA).

---

## Buddha

> Nothing ever exists entirely alone. Everything is in relation to everything else.

</br></br>
<!-- .fragment Agree:  Tufte, Cleveland, Tukey, Few, Kahneman -->
.fragment <span style="text-transform: none; font-size:24; color:#999;">Agree:  Tufte, Cleveland, Tukey, Few, Kahneman</span>


*** =pnotes
Others who agree:  Edward Tufte, William Cleveland, John Tukey, Stephen Few, Daniel Kahneman

Few - perceptualedge.com


--- .longer

> I cannot define the real problem, therefore I suspect there's no real problem, but I'm not sure there's no real problem.

<span style="padding-left:10em">Richard Feynman, physicist


*** =pnotes
Feynman was speaking about quantum mechanics (short defn).  A recent BBC article questioned whether the same might be true of consciousness.  I suggest that could also be true of leaders on the precipice of an analysis plan. 

http://www.bbc.com/earth/story/20170215-the-strange-link-between-the-human-mind-and-quantum-physics

--- {class: custom5, bg: "#007777", bt: zoom}

## Heads Up

reveal.js is a framework for easily creating beautiful presentations using HTML. You'll need a browser with support for CSS 3D transforms to see it in its full glory.

<section>

---

## Slide 1

---

## Slide 2

</section>

--- &vertical

## Vertical Slides

Slides can be nested inside of other slides, try pressing <a href="#" class="navigate-down">down</a>

<a href="#" class="image navigate-down">
  <img width="178" height="238" src="https://s3.amazonaws.com/hakim-static/reveal-js/arrow.png" alt="Down arrow">
</a>

***

## Basement Level 1

Press down or up to navigate.

***

## Basement Level 2

Cornify

<a class="test" href="http://cornify.com">
 <img width="280" height="326" src="https://s3.amazonaws.com/hakim-static/reveal-js/cornify.gif" alt="Unicorn">
</a>

***

## Basement Level 3

That's it, time to go back up.

<a href="#/2" class="image">
  <img width="178" height="238" src="https://s3.amazonaws.com/hakim-static/reveal-js/arrow.png" alt="Up arrow" style="-webkit-transform: rotate(180deg);">
</a>

--- &vertical

## Vertical Slides

Slides can be nested inside of other slides, try pressing <a href="#" class="navigate-down">down</a>

<a href="#" class="image navigate-down">
  <img width="178" height="238" src="https://s3.amazonaws.com/hakim-static/reveal-js/arrow.png" alt="Down arrow">
</a>

***

## Basement Level 1

Press down or up to navigate.

***

## Basement Level 2

Cornify

---

## Point of View

Press ESC to enter the slide overview. Hold down alt and click on any element to zoom in on it using [zoom.js](http://lab.hakim.se/zoom-js). Alt + click anywhere to zoom back out.

---

## RVL.IO

If you don't like writing slides in HTML you can use the online editor [rvl.io](http://rvl.io).

---

## Works in Mobile Safari

Try it out! You can swipe through the slides and pinch your way to the overview.

---

## Marvolous Unordered List

- No order here
- Or here
- Or here
- Or here

---

## Fantastic Ordered List

1. One is smaller than...
2. Two is smaller than...
3. Three!

--- #transitions

## TRANSITION STYLES
You can select from different transitions, like: 

[Cube](?transition=cube#/transitions) - [Page](?transition=page#/transitions) - [Concave](?transition=concave#/transitions) - [Zoom](?transition=zoom#/transitions) - [Linear](?transition=linear#/transitions) - [Fade](?transition=fade#/transitions) - [None](?transition=none#/transitions) - [Default](?transition=default#/transitions)

--- #themes

## Themes

Reveal.js comes with a few themes built in: 

[Sky](?theme=sky#/themes) - [Beige](?theme=beige#/themes) - [Simple](?theme=simple#/themes) - [Serif](?theme=serif#/themes) - [Night](?theme=night#/themes) - [Default](?theme=default#/themes) - [Solarized](?theme=solarized#/themes) - [Moon](?theme=moon#/themes)

<small>* Theme demos are loaded after the presentation which leads to flicker. In production you should load your theme in the `<head>` using a `<link>`.</small>

--- ds:alert &vertical

## Global State
Set `data-state="something"` on a slide and "something" will be added as a class to the document element when the slide is open. This lets you apply broader style changes, like switching the background.

<a href="#" class="image navigate-down">
  <img width="178" height="238" 
    src="https://s3.amazonaws.com/hakim-static/reveal-js/arrow.png" alt="Down arrow">
</a>

*** ds:blackout

## Blackout

<a href="#" class="image navigate-down">
  <img width="178" height="238" 
    src="https://s3.amazonaws.com/hakim-static/reveal-js/arrow.png" alt="Down arrow">
</a>

*** ds:soothe

## Soothe

<a href="#" class="image navigate-next">
  <img width="178" height="238" alt="Up arrow" style="-webkit-transform: rotate(-90deg);"
    src="https://s3.amazonaws.com/hakim-static/reveal-js/arrow.png" >
</a>

--- ds:red &vertical

## Custom Soothe Styles

*** ds:orange

## Orange

*** ds:yellow

## Yellow

*** ds:green

## Green

*** ds:blue

## Blue

*** ds:indigo

## Indigo

*** ds:violet

## Violet

*** ds:brown

## Brown

---

## Custom Events

Additionally custom events can be triggered on a per slide basis by binding to the data-state name.

```
Reveal.addEventListener( 'customevent', function() {
  console.log( '"customevent" has fired' );
} );
```

---

## Clever Quotes

These guys come in two forms, inline:  <q>The nice thing about standards is that there are so many to choose from and block:</q>

> For years there has been a theory that millions of monkeys typing at random on millions of typewriters would reproduce the entire works of Shakespeare. The Internet has proven this theory to be untrue.

---

## Pretty Code

```
function linkify( selector ) {
  if( supports3DTransforms ) {

    var nodes = document.querySelectorAll( selector );

    for( var i = 0, len = nodes.length; i < len; i++ ) {
      var node = nodes[i];

      if( !node.className ) ) {
        node.className += ' roll';
      }
    };
  }
}
```

Courtesy of [highlight.js](http://softwaremaniacs.org/soft/highlight/en/description/)

---

## Intergalactic Interconnections

You can link between slides internally, [like this](#/2/3).

---

## Fragmented Views

Hit the next arrow...

.fragment ... to step through ...

> - any type
> - of view
> - __fragments__

---

## Take a Moment

Press b or period on your keyboard to enter the 'paused' mode. This mode is helpful when you want to take distracting slides off the screen during a presentation.


---

## Incremental Paragraphs

.fragment This is paragraph 1 and should appear on first click.

.fragment This is paragraph 2 and should appear on second click.

.small [Back to the Beginning](#/0)


---

## Title

This is a slide

- point 1
- point 2
- point 3

---

## Incremental Reveal

These points should be animated

> - Point 1
> - .highlight-red Point 2
> - .grow Point 3

<script>
$('ul.incremental li').addClass('fragment')
</script>


---

## Code with slide


```r
library(ggplot2)
qplot(wt, mpg, data = mtcars)
```

![plot of chunk unnamed-chunk-3](figure/unnamed-chunk-3-1.png)

--- &vertical ds:soothe

## Vertical Slides

The next set of slides will be vertical slides.

***

## Slide 1

This is slide 1

***

## Slide 2

<iframe src='http://www.statdistributions.com' width = '960px' height = '600px'></iframe>

