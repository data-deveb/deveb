---
layout: default
permalink: 1.0/en/grid-system/partitioning-layout
lang: en
title: Partitioning Layout
description: 
---
<p class="girlik">
    The most used feature of the grid system is the piece layout. The piece layout is designed for you to create templates with stable percentage width. It offers use of all part layouts from 1 piece to 24 pieces. 
  </p>
  <div data-gnl="o" style="margin: 20px 0;">
    <div data-gnl="11 araları-aralık-1">
      <div data-gnl="4 araları-aralık-1">
        <div>
          <div style="background-color: #e0e0e0; min-height: 150px; height: 100%;"></div>
        </div>
        <div>
          <div style="background-color: #e0e0e0; min-height: 150px; height: 100%;"></div>
        </div>
      </div>
      <div data-gnl="4">
        <div style="background-color: #e0e0e0; min-height: 150px; height: 100%;"></div>
      </div>
      <div data-gnl="4">
        <div style="background-color: #e0e0e0; min-height: 150px; height: 100%;"></div>
      </div>
      <div data-gnl="8">
        <div style="background-color: #e0e0e0; min-height: 150px; height: 100%;"></div>
      </div>
      <div data-gnl="4">
        <div style="background-color: #e0e0e0; min-height: 150px; height: 100%;"></div>
      </div>
    </div>
  </div>
  <p>
    "NUMBER /NUMBER" values are used in the html file by writing to the desired display system. NUMBER can be between 1 and 24. For example, you want to divide the page into two and make the left side twice as wide as the right side. For this you can define the values data-gnl="2 /3" data-gnl="1 /3".
  </p> 
  <p></p>
  

  <h3>Piece Layout "NUMBER /NUMBER" Usage</h3>

  <p>
    When you write a piece layout to create a grid, you say something to the browser; "I will use the width of the piece as NUMBER by dividing the width I find into equal parts as NUMBER".For example, if you want to use half of the main width, you can use "1 /2", "2 /4", "3 /6", "4 /8", "5 /10", "6 /12", "7 /14", "8 /16", "9 /18", "10 /20", "11 /22" or "12 /24".
  </p>

  <p>
    Let's imagine a sample template before we start using the Piece layout. Have a place torn into 3 equal widths. In a place using a 20 piece arrangement, take the form of 3 columns with different widths between them. We can write our first example with the value "1 /3". We can write the other as "3 /20", "10 /20", "7 /20".
  </p>
  <div class="örnek">
    <h3>Preview: Example 1</h3>
    <div class="önizleme">
      <div data-gnl="1 /3">
        <div class="kutu">1 /3</div>
      </div>
      <div data-gnl="2 /3">
        <div class="kutu">2 /3</div>
      </div>
      <div data-gnl="4">
        <div class="kutu">4</div>
      </div>
      <div data-gnl="8">
        <div class="kutu">8</div>
      </div>
    </div>
    {% highlight html %}
    <div data-gnl="1 /3">
      <!-- content area -->
    </div>
    <div data-gnl="1 /3">
      <!-- content area -->
    </div>
    <div data-gnl="1 /3">
      <!-- content area -->
    </div>
    {% endhighlight %}
  </div>

  <div class="örnek">
    <h3>Preview: Example 2</h3>
    <div class="önizleme">
      <div data-gnl="3 /20">
        3 /20
      </div>
      <div data-gnl="10 /20">
        10 /20
      </div>
      <div data-gnl="7 /20">
        7 /20
      </div>
    </div>
    {% highlight html %}
    <div data-gnl="3 /20">
      3 /20
    </div>
    <div data-gnl="10 /20">
      10 /20
    </div>
    <div data-gnl="7 /20">
      7 /20
    </div>
    {% endhighlight %}
  </div>

  <div class="örnek">
    <h3>Preview: Example 3</h3>
    <p>Example 1 and 2 together.</p>
    <div class="önizleme">
      <div data-gnl="1 /3">
        1 /3
      </div>
      <div data-gnl="1 /3">
        1 /3
      </div>
      <div data-gnl="1 /3">
        1 /3
      </div>
      <div data-gnl="3 /20">
        3 /20
      </div>
      <div data-gnl="10 /20">
        10 /20
      </div>
      <div data-gnl="7 /20">
        7 /20
      </div>
    </div>
    {% highlight html %}
    <div data-gnl="1 /3">
      1 /3
    </div>
    <div data-gnl="1 /3">
      1 /3
    </div>
    <div data-gnl="1 /3">
      1 /3
    </div>
    <div data-gnl="3 /20">
      3 /20
    </div>
    <div data-gnl="10 /20">
      10 /20
    </div>
    <div data-gnl="7 /20">
      7 /20
    </div>
    {% endhighlight %}
  </div>

  <h3>"NUMBER /NUMBER" >> "NUMBER /NUMBER" Usage</h3>
  <p>
    By using this scheme, you tell the browser: "NUMBERp in the parent html tag is the default value for child tags. At the same time, the NUMBER I mention at the same time as the parent is the width of this label. All child tags are in this track order until the axel is specified. I can specify the width by typing NUMBER in the Child tags. If you specify /NUMBER in at least one child tag, this value becomes the new tag. The number value will also be the amount of parts of the new order."
  </p>
  <div class="örnek">
    <h3>Preview</h3>
    <div class="önizleme">
      <div data-gnl="2 /2">
        <div data-gnl="1 /4">
          1/4 piece of screens width.
        </div>
        <div data-gnl="1 /4">
          1/4 piece of screens width.
        </div>
        <div data-gnl="1 /4">
          1/4 piece of screens width.
        </div>
        <div data-gnl="1 /4">
          1/4 piece of screens width.
        </div>
      </div>
    </div>
    {% highlight html %}
    <div data-gnl="2 /2">
      <div data-gnl="1 /4">
        1/4 piece of screens width.
      </div>
      <div data-gnl="1 /4">
        1/4 piece of screens width.
      </div>
      <div data-gnl="1 /4">
        1/4 piece of screens width.
      </div>
      <div data-gnl="1 /4">
        1/4 piece of screens width.
      </div>
    </div>
    {% endhighlight %}
  </div>

  <h3>Grow vs Piece Layout</h3>
  <p>
    The grow layout and the piece layout are not created with the same calculation balances. Each expansion in the layout will interact with each other. In Piece layout, stable width is created. Let's understand better by example.
  </p>
  <div class="örnek">
    <h3>Preview</h3>
    <div class="önizleme">
      <div>
        <div data-gnl="1 /">
          1 /
        </div>
        <div data-gnl="4 /">
          4 /
        </div>
        <div data-gnl="2 /">
          2 /
        </div>
      </div>
      <div>
        <div data-gnl="1 /7">
          1 /7
        </div>
        <div data-gnl="4 /7">
          4 /7
        </div>
        <div data-gnl="2 /7">
          2 /7
        </div>
      </div>
    </div>
    {% highlight html %}
    <div>
      <div data-gnl="1 /">
        1 /
      </div>
      <div data-gnl="4 /">
        4 /
      </div>
      <div data-gnl="2 /">
        2 /
      </div>
    </div>
    <div>
      <div data-gnl="1 /7">
        1 /7
      </div>
      <div data-gnl="4 /7">
        4 /7
      </div>
      <div data-gnl="2 /7">
        2 /7
      </div>
    </div>
    {% endhighlight %}
  </div>