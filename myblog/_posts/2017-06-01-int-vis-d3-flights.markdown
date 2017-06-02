---
layout: post
title:  "Interactive visualizations using D3.js and D3 wrappers in Shiny"
date:   2017-04-30 20:43:02 -0700
categories: jekyll update
---

I think D3.js is the one of the best libraries out there for interactive visualizations. This post will cover two cases; the first one uses D3.js while the second one uses D3 wrappers in Shiny.

### Domestic Flights by City in the US

The interactive plot is located here – [Chord Diagram][chord-diag].

The mouseover interactions can only be seen at the link above. The following screenshots only show some examples of static content and do not do justice to the actual figure.

![Chord1]({{ site.url }}/assets/chord1.png)

![Chord2]({{ site.url }}/assets/chord2.png)


The code for the chord diagram and the flights data can be found [here][flights-repo].

### Diabetes visualizations in Shiny using D3 wrappers

Three different visualizations on a diabetes data set are located here – [Diabetes Visualizations][diabetes-vis]

Again, to explore the full interactivity of these plots, I recommend that you visit the above link. The following examples are screenshots of static content.

### Parallel Co-ordinates Plot with Brushing

![diab1]({{ site.url }}/assets/diab1.png)

Here, you can select certain ranges of variables using brushing:

![diab2]({{ site.url }}/assets/diab1.png)

Scatterplot Matrix colored by different factors

Here, there are three different factor variables that can be used to color the points – race, gender, and age.

![diab3]({{ site.url }}/assets/diab3.png)

You can select certain points in one square using brushing, and the same points are selected in the other squares:

![diab4]({{ site.url }}/assets/diab4.png)

### Heatmaps with different groupings

For these heatmaps, a user can select groupings to visualize measures such as the time in the hospital, and the number of lab procedures performed on diabetes patients.

![diab5]({{ site.url }}/assets/diab5.png)

The user can mouse over a particular cell to see the average value for that particular column or measure across the row or grouping.

The code for all of the diabetes data visualizations can be found [here][diab-repo].


You’ll find this post in your `_posts` directory. Go ahead and edit it and re-build the site to see your changes. You can rebuild the site in many different ways, but the most common way is to run `jekyll serve`, which launches a web server and auto-regenerates your site when a file is updated.

To add new posts, simply add a file in the `_posts` directory that follows the convention `YYYY-MM-DD-name-of-post.ext` and includes the necessary front matter. Take a look at the source for this post to get an idea about how it works.

Jekyll also offers powerful support for code snippets:

{% highlight ruby %}
def print_hi(name)
  puts "Hi, #{name}"
end
print_hi('Tom')
#=> prints 'Hi, Tom' to STDOUT.
{% endhighlight %}

Check out the [Jekyll docs][jekyll-docs] for more info on how to get the most out of Jekyll. File all bugs/feature requests at [Jekyll’s GitHub repo][jekyll-gh]. If you have questions, you can ask them on [Jekyll Talk][jekyll-talk].

[chord-diag]: https://shivathudi.github.io/flights-chord/
[flights-repo]:   https://shivathudi.github.io/flights-chord/
[diabetes-vis]: https://shivathudi.shinyapps.io/diabetes-vis2/
[diab-repo]: https://github.com/shivathudi/data-visualization/tree/master/diabetes_data