<<<<<<< HEAD
---
layout: page
title: Leetcode questions analysis
description: Insights and predict topics
img: assets/img/pro2_1.jpg
importance: 2
category: work
---

#### __[Code](https://github.com/manthan2305/leetcode-questions-analysis)__

### About Dataset

Leetcode is very popular among programmers. It has so many quality questions for various topics. It is crucial for content provider to understand the question quality with difficulty levels, most/less popular topics among programmers, most liked/disliked questions etc. It will be helpful to get overall trend, skill improvization pathway and which topic needs much more attention then any other to work. Each question contains similar questions title and text, which can be used to sugget similar questions.

> Dataset is available on [Kaggle](https://www.kaggle.com/datasets/manthansolanki/leetcode-questions)

Entire project is divided into three major tasks:
1. Data Scraping
2. Data Analysis
3. Topic prediction

#### Data Scraping

The data is scraped from this [webpage](https://leetcode.com/problemset/all/) using this [file](https://github.com/manthan2305/leetcode-questions-analysis/blob/main/scrape_data.py).
<br>
:warning: **Disclaimer**: *The purpose of the data scraping is solely for generating insights.*

---
#### Data Analysis

At the time of working on this project, the Leetcode website offers a grand total of **2239 questions** spanning across **72 distinct topics**.
<br>

Among these, the **'Medium'** difficulty level emerges as the category with the highest number of questions, coming in at just under 1200.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/pro2_2.jpg" title="difficulty-level" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Number of questions for each difficulty level
</div>

The graph visually represents the distribution of questions by topic, showcasing the total number of questions for each topic. The predominant topics with the highest number of questions include **'Array'**, **'String'**, **'Hash Table'**, **'Dynamic Programming'**, and **'Math'**.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/pro2_3.jpg" title="topicwise questions" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Number of questions in each topics
</div>

Upon analyzing the graph, we observe that when considering the combined factors of difficulty level and total number of questions per topic, the **'Medium'** category emerges as the one with a significant number of questions across various topics.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/pro2_4.jpg" title="top-and-difficulty" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Total questions by topic and difficulty Level
</div>

We can infer that problem solvers found **'Shell'** questions to be notably challenging and strenuous to solve, while a majority of coders were able to solve **'Database'** questions with relative ease.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/pro2_5.jpg" title="average-min-max-accuracy" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Topics with average minimum and maximum accuracy
</div>

Discover the top four most popular topics on Leetcode, highly favored by problem solvers.
1. Array
2. String
3. Hash Table
4. Dynamic Programming

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/pro2_6.jpg" title="most-likes-topics" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Top leading topics on Leetcode
</div>

---
#### Topic prediction

To predict the topic based on question and description text, a systematic approach involves data processing, which includes text cleaning, word frequency analysis, and record preparation. 
<br>
Subsequently, the data is divided into training, validation, and test sets. Utilizing either simple regression methods or advanced models like Bert, we can effectively predict the topics.

### Results

| Methods | f1-score |
|---|---|
| Logistic Regression | 0.55 |
| Bert | 0.88 |

> Both notebooks are available [here](https://github.com/manthan2305/leetcode-questions-analysis/tree/main/notebooks).
=======
---
layout: page
title: project 2
description: a project with a background image and giscus comments
img: assets/img/3.jpg
importance: 2
category: work
giscus_comments: true
---

Every project has a beautiful feature showcase page.
It's easy to include images in a flexible 3-column grid format.
Make your photos 1/3, 2/3, or full width.

To give your project a background in the portfolio page, just add the img tag to the front matter like so:

    ---
    layout: page
    title: project
    description: a project with a background image
    img: /assets/img/12.jpg
    ---

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/1.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/3.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/5.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Caption photos easily. On the left, a road goes through a tunnel. Middle, leaves artistically fall in a hipster photoshoot. Right, in another hipster photoshoot, a lumberjack grasps a handful of pine needles.
</div>
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/5.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    This image can also have a caption. It's like magic.
</div>

You can also put regular text between your rows of images.
Say you wanted to write a little bit about your project before you posted the rest of the images.
You describe how you toiled, sweated, _bled_ for your project, and then... you reveal its glory in the next row of images.

<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/6.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/11.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    You can also have artistically styled 2/3 + 1/3 images, like these.
</div>

The code is simple.
Just wrap your images with `<div class="col-sm">` and place them inside `<div class="row">` (read more about the <a href="https://getbootstrap.com/docs/4.4/layout/grid/">Bootstrap Grid</a> system).
To make images responsive, add `img-fluid` class to each; for rounded corners and shadows use `rounded` and `z-depth-1` classes.
Here's the code for the last row of images above:

{% raw %}

```html
<div class="row justify-content-sm-center">
  <div class="col-sm-8 mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/6.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
  </div>
  <div class="col-sm-4 mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/11.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
  </div>
</div>
```

{% endraw %}
>>>>>>> upstream/master
