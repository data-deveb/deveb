---
layout: default
permalink: 1.0/en/grid-system/spacing-layout
lang: en
title: Spacing Layout
description: 
---

<p class="girlik">
  Create a more aesthetic look by leaving spacings between objects. Use several options, such as self-calculated range widths, constant range widths, and so on. More below.
</p>

<h3>space-between & space-around</h3>
<p>
  The "space-between" parameter is used when it is desired to create a space between objects. The range width automatically changes according to the width of the container label.
</p>
<p>
  Use the "space-around" parameter if you want to leave a space around the objects. The range is automatically set according to the width of the container label. The interval between objects is twice that between the outer edge and the outer edge.
</p>
<div class="örnek">
  <h3>Preview</h3>
  <div class="önizleme">
    <div data-gnl="space-between">
      <div data-gnl="1 /8">
        space-between
      </div>
      <div data-gnl="1 /8">
        space-between
      </div>
      <div data-gnl="1 /8">
        space-between
      </div>
    </div>
    <div data-gnl="space-around">
      <div data-gnl="1 /8">
        space-around
      </div>
      <div data-gnl="1 /8">
        space-around
      </div>
      <div data-gnl="1 /8">
        space-around
      </div>
    </div>
  </div>
</div>
{% highlight html %}
  <div data-gnl="space-between">
    <div data-gnl="1 /8">
      space-between
    </div>
    <div data-gnl="1 /8">
      space-between
    </div>
    <div data-gnl="1 /8">
      space-between
    </div>
  </div>
  <div data-gnl="space-around">
    <div data-gnl="1 /8">
      space-around
    </div>
    <div data-gnl="1 /8">
      space-around
    </div>
    <div data-gnl="1 /8">
      space-around
    </div>
  </div>
{% endhighlight %}

<h3>space-between-NUMBER</h3>
<p>
  Use this feature to leave a gap in the static width between objects. Width values are indicated by 1, 2, 3 numbers. By typing "space-between-1", you get a result like this:
</p>
<div class="örnek">
  <h3>Preview</h3>
  <div class="önizleme-1">
    <div data-gnl="space-between-1 5-5">
      <div>
        <div class="kart">1</div>
      </div>
      <div>
        <div class="kart">2</div>
      </div>
      <div>
        <div class="kart">3</div>
      </div>
      <div>
        <div class="kart">4</div>
      </div>
      <div>
        <div class="kart">5</div>
      </div>
      <div data-gnl="2 /5">
        <div class="kart">6</div>
      </div>
      <div>
        <div class="kart">7</div>
      </div>
      <div>
        <div class="kart">8</div>
      </div>
      <div>
        <div class="kart">9</div>
      </div>
      <div>
        <div class="kart">10</div>
      </div>
      <div data-gnl="3 /5">
        <div class="kart">11</div>
      </div>
      <div>
        <div class="kart">12</div>
      </div>
    </div>
  </div>
</div>
{% highlight html %}
  <div data-gnl="space-between-1 5-5">
    <div>
      <div class="kart">1</div>
    </div>
    <div>
      <div class="kart">2</div>
    </div>
    <div>
      <div class="kart">3</div>
    </div>
    <div>
      <div class="kart">4</div>
    </div>
    <div>
      <div class="kart">5</div>
    </div>
    <div data-gnl="2 /5">
      <div class="kart">6</div>
    </div>
    <div>
      <div class="kart">7</div>
    </div>
    <div>
      <div class="kart">8</div>
    </div>
    <div>
      <div class="kart">9</div>
    </div>
    <div>
      <div class="kart">10</div>
    </div>
    <div data-gnl="3 /5">
      <div class="kart">11</div>
    </div>
    <div>
      <div class="kart">12</div>
    </div>
  </div>
{% endhighlight %}