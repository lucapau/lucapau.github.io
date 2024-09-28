---
layout: page
title: 4-in-1 QT App
description: A multi-functional application featuring Weather Forecasting, Currency Conversion, Password Management, and Note-Taking.
img: assets/img/12.jpg
importance: 1
category: work
related_publications: true
---

The 4-in-1 QT App is a comprehensive tool designed to streamline everyday tasks. It includes a weather forecasting feature, currency conversion, a password manager, and a note-taking function, all wrapped in a user-friendly interface.

To give your project a background in the portfolio page, just add the img tag to the front matter like so:

    ---
    layout: page
    title: 4-in-1 QT App
    description: A project with a background image
    img: /assets/img/12.jpg
    ---

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/weather_forecast.jpg" title="Weather Forecast Feature" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/currency_converter.jpg" title="Currency Converter Feature" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/password_manager.jpg" title="Password Manager Feature" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Showcase of features: Left - Weather Forecast, Middle - Currency Converter, Right - Password Manager.
</div>

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/note_taking.jpg" title="Note-Taking Feature" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    The Note-Taking feature allows users to manage tasks efficiently.
</div>

You can also put regular text between your rows of images, even citations {% cite einstein1950meaning %}.
Say you wanted to write a bit about your project before you posted the rest of the images.
You describe how you toiled, sweated, _bled_ for your project, and then... you reveal its glory in the next row of images.

<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/overall_design.jpg" title="Overall Design" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/ui_example.jpg" title="User Interface Example" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    The overall design of the app showcases its user-friendly interface.
</div>

The code is simple.
Just wrap your images with `<div class="col-sm">` and place them inside `<div class="row">` (read more about the <a href="https://getbootstrap.com/docs/4.4/layout/grid/">Bootstrap Grid</a> system).
To make images responsive, add `img-fluid` class to each; for rounded corners and shadows use `rounded` and `z-depth-1` classes.
Here's the code for the last row of images above:

{% raw %}

```html
<div class="row justify-content-sm-center">
  <div class="col-sm-8 mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/overall_design.jpg" title="Overall Design" class="img-fluid rounded z-depth-1" %}
  </div>
  <div class="col-sm-4 mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/ui_example.jpg" title="User Interface Example" class="img-fluid rounded z-depth-1" %}
  </div>
</div>
{% endraw %}