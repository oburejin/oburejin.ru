+++
date = ""
draft = true
title = "Javascript is missing"

+++
Actually no, I planned to do this without JS as much as possible and for now there is no JS at all, not in external scripts, no inline, no even statistics. I got this idea because a lot of sites have too much JS that is not needed there and it slows pages. I don't know where this journey will take me, so I may add something, but my goal is to go as much as possible without it, it is a blog, after all, and not an application.

Also pages are missing, like "About" page or so, but I don't know yet how to do pages on HUGO, sure it should not be hard to do, but I have only a couple of evenings to work on it, so progress is very slow, but I'm learning to accept that and with this seems to work. Even when I spend all my free 30 minutes a day to find some small thing I'm still satisfied that I did that. This doesn't work well for my main activities and I get frustrated when little is achieved (it's most of the times, because this is how things work, little by little), but I'll get there.

This update I added a `shortcode` that allows to insert a raw html, I wanted this to add some small things I can do with HTML/CSS, and maybe JS in some cases.

{{< rawhtml >}}

  <style>

  .wrapper {

    position: relative;

    width: 100%;

    height: 100px;

    border-radius: 5px;

  }

  .box,

  .box1,

  .box2,

  .box3,

  .box4,

  .box5,

  .box6 {

    position: absolute;

    width: 50px;

    height: 50px;

    margin: auto;

    top: 0;

    left: 0;

    right: 0;

    bottom: 0;

    background-color: coral;

    animation-name: rotate;

    animation-duration: 7s;

    animation-iteration-count: infinite;

    animation-timing-function: ease-in;

    z-index: 10;

  }

  .box1 {

    background-color: cornflowerblue;

    animation-delay: .1s;

    z-index: 9;

  }

  .box2 {

    background-color: teal;

    animation-delay: .2s;

    z-index: 8;

  }

  .box3 {

    background-color: #b00b15;

    animation-delay: .3s;

    z-index: 7;

  }

  .box4 {

    background-color: gray;

    animation-delay: .4s;

    z-index: 6;

  }

  .box5 {

    background-color: hotpink;

    animation-delay: .5s;

    z-index: 5;

  }

  .box6 {

    background-color: limegreen;

    animation-delay: .6s;

    z-index: 4;

  }

  @keyframes rotate {

    0% {

      transform: rotateZ(0deg);

    }

    50% {

      transform: rotateZ(180deg);

    }

    100% {

      transform: rotateZ(0deg);

    }

  }

  </style>

  

  <div class="wrapper">

    <div class="box"></div>

    <div class="box1"></div>

    <div class="box2"></div>

    <div class="box3"></div>

    <div class="box4"></div>

    <div class="box5"></div>

    <div class="box6"></div>

  <div>

{{< /rawhtml >}}