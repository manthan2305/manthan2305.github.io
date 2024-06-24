<<<<<<< HEAD
---
layout: page
title: Webpage Phishing Detection
description: ML based solution
img: assets/img/pro3_1.jpg
# redirect: https://unsplash.com
importance: 3
category: work
---

#### __[Code](https://github.com/manthan2305/webpage-phishing-detection)__

### Abstract

In the era of online working in every field, the ratio of cyber attacks is increasing day by day. 
Among all cyber crimes, online fraud is one of the biggest malicious activities faced by the 
cyber world. In technical terms, online fraud is called phishing attack. The demand of opensource software that can only detect the phishing websites is increasing. There are many 
approaches being proposed and this project is one of them. This approach uses machine 
learning method to detect the phishing website only from the URL. Random forest (RF), 
Support Vector Machine (SVM) and Neural network (NN) are used as classifier because this 
approach is designed to solve binary classification problem and among all ML classifiers, 
these 3 can give high accuracy and more accurate result. 

Out of these three classifiers, SVM gives the poor accuracy – *69 %* only. One the other side, 
RF and NN give same *96 %* accuracy. These models can be used for building further 
detection system. The system which generates features of the URL itself and uses that result 
to predict the final class label – ‘legitimate’ or ‘phishing’. There are some dependencies 
(limitations) of this approach: The given URL has to be active and it has to generate exact 87 
features used to train the ML models. This approach can be extended by creating basic 
browser extensions that everyone can use. 

#### Structure of the URL

Phishing attack can be done in many ways. One of the techniques to conduct phishing attack 
is by tempering with URL and its component. Attacker can make few minor changes that a 
normal user cannot see or notice and could become a victim of phishing attack. For a normal 
user, URL refers as a whole link without knowing its components yet, it is important to know 
the components and parts of URL that makes the entire working URL structure. 
Different components of URLs are described below:

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/pro3_2.jpg" title="url-structure" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Structure and main components of URL
</div>


#### Dataset

> The dataset is created by **Hannousse, Abdelhakim; Yahiouche, Salima (2021), “Web page phishing detection”**, Mendeley Data, V3, doi: 10.17632/c2gw7fy2j4.3

> It can be accessed on their [website](https://data.mendeley.com/datasets/c2gw7fy2j4/3) as well as on [Kaggle](https://www.kaggle.com/datasets/shashwatwork/web-page-phishing-detection-dataset).

The dataset used for this project is having some “legitimate” URLs, few “phishing” URLs 
and the features with the class label phishing and legitimate. The dataset contains 11430 
URLs divided into 50% legitimate URLs and 50% phishing URLs and this latest updated 
version is published in June 2021. 

These features are extracted based on the structure of the 
URLs, the content of the corresponding web pages and some are from the querying external 
services. First 56 features are related to URL structure followed by 24 features of the content 
of webpages and 7 features of the querying external services. 

The last column of the dataset 
specifies the class label. The reason behind selecting this dataset is it focuses maximum 
number of URL features as the major concern was to build a system which focuses more on 
the URL.

#### Data Analysis

The plot show's the importanct of numerical values to predict website phishing or not,
1. Higher the length of URL, the ratio of being phishing is also high
2. High the length of hostname, chance of being legitimate is less.
3. More the length of Longest_word_raw and longest_word_path, high possibility of being phishing website. 

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/pro3_3.jpg" title="numerical-features" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Distribution of feature's value for each class
</div>

In the case of all features, there are 30 numerical data features and 59 categorical features 
(includes class label column as well). 
The correlation matrix of numerical data features is shown in this figure. 
From the figure, the majority relation matrix is made in the middle corner which is same as 
the obtained from the URL features. All 14 relations obtained from the previous URL 
features are still described the strong relation. Five more relationships are seen in the case of 
all numeric features. 1st is, ratio_inthyperlinks and safe_anchor, 2nd is ratio_inthyperlinks 
and ratio_intMedia, 3rd is ratio_inthyperlinks and links_in_tags, 4th is ratio_exthyperlinks 
and ratio_extMedia, 5th is links_in_tags and ratio_intMedia. 

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/pro3_4.jpg" title="correlation matrix" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Correlation matrix of numerical features
</div>

The impact of numerical data features over the class legitimate and phishing has been derived 
from the average values of numerical data. The observation of the following graph is: In the 
case of all features, compared to other numerical data feature, web_trafficing is the only 
feature which reflects direct on the class output.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/pro3_5.jpg" title="more-analysis-numerical-features" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Further analysis of numerical features
</div>

### Output of various methods

Various machine learning algorithm used with different parameters, here is the table to review all the experiments:

|Algorithms |features	|Parameters(specific)	| Acuuracy(%)|
|---|---|---|---|		
|SVM|	URL only|	C=1000  |   42|
|   |		    |   C=100   |   42|
|   |           |   C=1     |   42|
|SVM|   all 	|   C=1 , kernel = linear|  69|
|	|           |   C=100   |   69|
|RF |URL        |	n_estimators=20|    90|
|	|       	|   n_estimators=40|    91|
|   |       	|   n_estimators=60|    91|
|RF |all        |	n_estimators=20|    96|
|	|	        |   n_estimators=40|    96|
|	|	        |   n_estimators=60|    96|
	
---
#### Inference

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/pro3_6.jpg" title="output" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Inference output
</div>
=======
---
layout: page
title: project 3 with very long name
description: a project that redirects to another website
img: assets/img/7.jpg
redirect: https://unsplash.com
importance: 3
category: work
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
