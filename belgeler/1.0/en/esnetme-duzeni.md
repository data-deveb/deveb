---
layout: default
permalink: 1.0/en/grid-system/flexing-layout
lang: en
title: Flexing Layout
description: 
---
<p class="girlik">
    You can create grid fields simply by specifying the expansion. Grow layout is based on "CSS FLEX" feature. It is enough to write "NUMBER /" class to display attributes (data-gnl, data-md ...) for Grow layout use. NUMBER can be a value between 1 and 24. For example, you want to divide the page into two and make the left side twice as wide as the right side. For this you can define the attributes data-gnl = "2 /" data-gnl = "1 /".
  </p>
  <h3>How to Use Grow Layout</h3>
  <p>
    Let's create a layout with three columns in all of the screens. As an example, let's make the layout distribution 1 4 2.
  </p>

  <div class="örnek">
    <h3>Preview</h3>
    <div class="önizleme">
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
  </div>
  {% highlight html %}
    <div data-gnl="1 /">
      1 /
    </div>
    <div data-gnl="4 /">
      4 /
    </div>
    <div data-gnl="2 /">
      2 /
    </div>
  {% endhighlight %}

  <h3>Why Use Grow Layout?</h3>

  <p>
  Let's first remember piece layout. The piece layout was used to define the centrally defined widths. Because of this situation, the widths of the pieces included in the width continue to line up when they fill the width. Let's take a look at grow layout. Grow layout How much you add will not add to the bottom line. So every time you add it, it will be recalculated and grow widths will change and the same row will be recovered. If you want to continue from the bottom line, you need to create an empty item 100% wide.
</p>
<p>
  In addition to these, you can use piece layout and grow layout together. Including widths made with other methods. Grow layout will be a place for itself according to the structure. Examine the mixed use example below.
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
      <div><!--100% width empty item--></div>
      <div data-gnl="1 /">
        1 /
      </div>
      <div data-gnl="4 /">
        4 /
      </div>
      <div data-gnl="2 /">
        2 /
      </div>
      <div data-gnl="1 /">
        1 /
      </div>
      <div data-gnl="4 /">
        4 /
      </div>
      <div data-gnl="2 /">
        2 /
      </div>
      <div><!--100% width empty item--></div>
      <div data-gnl="1 /">
        1 /
      </div>
      <div data-gnl="4 /">
        4 /
      </div>
      <div data-gnl="2 /">
        2 /
      </div>
      <div data-gnl="1 /2">
        1 /2
      </div>
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
      <div><!--100% width empty item--></div>
      <div data-gnl="1 /">
        1 /
      </div>
      <div data-gnl="4 /">
        4 /
      </div>
      <div data-gnl="2 /">
        2 /
      </div>
      <div data-gnl="1 /">
        1 /
      </div>
      <div data-gnl="4 /">
        4 /
      </div>
      <div data-gnl="2 /">
        2 /
      </div>
      <div><!--100% width empty item--></div>
      <div data-gnl="1 /">
        1 /
      </div>
      <div data-gnl="4 /">
        4 /
      </div>
      <div data-gnl="2 /">
        2 /
      </div>
      <div data-gnl="1 /2">
        1 /2
      </div>
    </div>
  {% endhighlight %}
<h3>Grow vs Piece</h3>
<p>
  Grow layout and piece layout are not created with the same account balances. In grow layout, each width is interactive. In Piece layout, stable width is created. Let's understand better by example.
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