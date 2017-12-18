---
layout: page
title: The tools
subtitle: What tools and libraries did we use?
---

### Cloud storage

Both datasets were stored in a computer cluster (IC Cluster), hosted in EPFL.

The [datasets]({{site.baseurl}}/thedatasets) were huge (in terms of terabytes for Tweets Leon and in terms of gigabytes for Swiss Tweets) and they were were stored in a <a href="https://hadoop.apache.org/" target="_blank">Hadoop</a> file system (HDFS).

In order to conduct the analysis we wrote some Python scripts and ran them via <a href="https://spark.apache.org/" target="_blank">Spark</a> on the cluster.

### The analysis and plots

<a href="https://pandas.pydata.org/" target="_blank">Pandas</a> and <a href="https://jupyter.org/" target="_blank">jupyter</a> notebooks were indispensable tools while conducting the analysis of this project and made it easier to try things out and to share/showoff all of our intermediate results.

The plots found in this site were made possible via <a href="https://plot.ly/" target="_blank">plot.ly</a> and its Python API.

### This site

This site was created with <a href="https://jekyllrb.com/" target="_blank">Jekyll</a>, using the <a href="https://deanattali.com/beautiful-jekyll/" target="_blank">beautiful-jekyll</a> theme and is hosted via <a href="https://pages.github.com/" target="_blank">GitHub pages</a>.


### Source code

The source code of this project can be found on <a href="https://github.com/sagap/ADAExercises2017/tree/master/project" target="_blank">GitHub</a>.
