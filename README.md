## Website Performance Optimization portfolio project

Your challenge, if you wish to accept it (and we sure hope you will), is to optimize this online portfolio for speed! In particular, optimize the critical rendering path and make this page render as quickly as possible by applying the techniques you've picked up in the [Critical Rendering Path course](https://www.udacity.com/course/ud884).

To get started, check out the repository and inspect the code.

### Getting started

#### Part 1: Optimize PageSpeed Insights score for index.html

Some useful tips to help you get started:

Improvements Implemented:

Index.html

1- Compressed pizzeria.jpg.
2- Compressed profile picture.
3- Compressed cam_be_like.jpg.
4- Compressed 2048.png
5- Inlined css.
6- Removed request for google fonts and included the the required fonts in html.
7- Minify index.html.

#### How To Run it:
double click on index.html

#### Part 2: Optimize Frames per Second in pizza.html

1- Edit main.js file so the resizing of the pizzas happens in less than 5 ms and the scrolling runs at 60 FPS

2- Simplify the function resizePizzas so it doesn't trigger forced synchronous layout (FSL). The pizzas width simply gets set to a certain percentage of the original image size, depending on the slider position.

3- Changed updatePositions so it doesn't trigger FSL by first getting scrollTop and then updating all elements later.

4- Updated querySelectorAll("#mover") to getElementsByClassName("mover") so it doesn't have to recalculate on every iteration.

5- replace querySelector with getElementById and getElementsByClassName.

#### How To Run it:
1- Go to project folder -> views folder -> open pizza.html

2- Right click on pizza.html window, select inspect, go to console to view time to generate layout and paint in miliseconds (ms)

### Optimization Tips and Tricks
* [Optimizing Performance](https://developers.google.com/web/fundamentals/performance/ "web performance")
* [Analyzing the Critical Rendering Path](https://developers.google.com/web/fundamentals/performance/critical-rendering-path/analyzing-crp.html "analyzing crp")
* [Optimizing the Critical Rendering Path](https://developers.google.com/web/fundamentals/performance/critical-rendering-path/optimizing-critical-rendering-path.html "optimize the crp!")
* [Avoiding Rendering Blocking CSS](https://developers.google.com/web/fundamentals/performance/critical-rendering-path/render-blocking-css.html "render blocking css")
* [Optimizing JavaScript](https://developers.google.com/web/fundamentals/performance/critical-rendering-path/adding-interactivity-with-javascript.html "javascript")
* [Measuring with Navigation Timing](https://developers.google.com/web/fundamentals/performance/critical-rendering-path/measure-crp.html "nav timing api"). We didn't cover the Navigation Timing API in the first two lessons but it's an incredibly useful tool for automated page profiling. I highly recommend reading.
* <a href="https://developers.google.com/web/fundamentals/performance/optimizing-content-efficiency/eliminate-downloads.html">The fewer the downloads, the better</a>
* <a href="https://developers.google.com/web/fundamentals/performance/optimizing-content-efficiency/optimize-encoding-and-transfer.html">Reduce the size of text</a>
* <a href="https://developers.google.com/web/fundamentals/performance/optimizing-content-efficiency/image-optimization.html">Optimize images</a>
* <a href="https://developers.google.com/web/fundamentals/performance/optimizing-content-efficiency/http-caching.html">HTTP caching</a>

### Customization with Bootstrap
The portfolio was built on Twitter's <a href="http://getbootstrap.com/">Bootstrap</a> framework. All custom styles are in `dist/css/portfolio.css` in the portfolio repo.

* <a href="http://getbootstrap.com/css/">Bootstrap's CSS Classes</a>
* <a href="http://getbootstrap.com/components/">Bootstrap's Components</a>
