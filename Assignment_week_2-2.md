
# Assignment for week 2

Use the following table to provide us with

|name | exam number|
|----|----|
|Bastiaan Heerius| 2002377|
|other group member's name| exam number|

In the following cell type in markdown the text with a link and an image that you can find [here](http://janboone.github.io/programming-for-economists/_downloads/markdown_text_programming_for_economists.html).

Note that we are interested in seeing bold text, italics and math etc. Use your browser to find the image's address.

After you type your text, press SHIFT-ENTER and check whether the text looks the same as [here](http://janboone.github.io/programming-for-economists/_downloads/markdown_text_programming_for_economists.html).

# This is a section

## This is a subsection

A bullit list looks *like this*:
* Bullit 1
* Bullit 2
* **bullit 3**

We can like to this [wonderful page](http://janboone.github.io/programming-for-economists/index.html).

And we can add a picture to the text as well.

![alt text](http://images2.mtv.com/uri/mgid:file:docroot:mtv.com:/crop-images/2013/11/05/the_who_umg.jpg?enlarge=false&maxdimension=1300&matte=true&matteColor=black&quality=0.85)

Let's type some math:
$$
\sin(x)+\cos(x)=2
$$

As a rule, I really like this line

----

We are done


Install plotly on your computer using these [instructions to install plotly.](https://plot.ly/python/getting-started/) Note that with anaconda you can use "conda install plotly" instead of "pip install".

Now let us check whether it works, run the code in the following cell:


```python
import plotly 
plotly.tools.set_credentials_file(username='BastiaanHeerius', api_key='N3KgqSJfyIpANnoMjfbn')
```


```python
from plotly.offline import download_plotlyjs, init_notebook_mode, plot, iplot
from plotly.graph_objs import Bar, Scatter, Figure, Layout
init_notebook_mode(connected=True)
from numpy import arange
range_x = arange(-2,2.1,0.1)
iplot([{"x": range_x, "y": [x**2 for x in range_x]}])
```


<script>requirejs.config({paths: { 'plotly': ['https://cdn.plot.ly/plotly-latest.min']},});if(!window.Plotly) {{require(['plotly'],function(plotly) {window.Plotly=plotly;});}}</script>



<div id="c77edb5d-899b-4f77-a5c0-50a4637ab3ea" style="height: 525px; width: 100%;" class="plotly-graph-div"></div><script type="text/javascript">require(["plotly"], function(Plotly) { window.PLOTLYENV=window.PLOTLYENV || {};window.PLOTLYENV.BASE_URL="https://plot.ly";Plotly.newPlot("c77edb5d-899b-4f77-a5c0-50a4637ab3ea", [{"x": [-2.0, -1.9, -1.7999999999999998, -1.6999999999999997, -1.5999999999999996, -1.4999999999999996, -1.3999999999999995, -1.2999999999999994, -1.1999999999999993, -1.0999999999999992, -0.9999999999999991, -0.899999999999999, -0.7999999999999989, -0.6999999999999988, -0.5999999999999988, -0.49999999999999867, -0.3999999999999986, -0.2999999999999985, -0.1999999999999984, -0.09999999999999831, 1.7763568394002505e-15, 0.10000000000000187, 0.20000000000000195, 0.30000000000000204, 0.40000000000000213, 0.5000000000000022, 0.6000000000000023, 0.7000000000000024, 0.8000000000000025, 0.9000000000000026, 1.0000000000000027, 1.1000000000000028, 1.2000000000000028, 1.300000000000003, 1.400000000000003, 1.500000000000003, 1.6000000000000032, 1.7000000000000033, 1.8000000000000034, 1.9000000000000035, 2.0000000000000036], "y": [4.0, 3.61, 3.2399999999999993, 2.8899999999999992, 2.5599999999999987, 2.2499999999999987, 1.9599999999999984, 1.6899999999999984, 1.4399999999999984, 1.2099999999999982, 0.9999999999999982, 0.8099999999999983, 0.6399999999999983, 0.4899999999999984, 0.3599999999999985, 0.24999999999999867, 0.15999999999999887, 0.0899999999999991, 0.03999999999999936, 0.009999999999999662, 3.1554436208840472e-30, 0.010000000000000373, 0.040000000000000785, 0.09000000000000123, 0.1600000000000017, 0.2500000000000022, 0.36000000000000276, 0.4900000000000034, 0.640000000000004, 0.8100000000000046, 1.0000000000000053, 1.210000000000006, 1.4400000000000068, 1.6900000000000077, 1.9600000000000084, 2.2500000000000093, 2.5600000000000103, 2.8900000000000112, 3.240000000000012, 3.610000000000013, 4.000000000000014]}], {}, {"showLink": true, "linkText": "Export to plot.ly"})});</script>


Do you see the graph in your notebook? If not, ask us during the tutorial!

After you have finished, we need to upload this notebook on github. Make sure that you upload the file on the github page of each group member.

Instructions on how to upload this on github can be found [on this page](http://janboone.github.io/programming-for-economists/github.html). This page has two screencasts: one shows how to drag the notebook onto your github page, the other shows how you can use the command line to upload your notebook.


Remember to update the README file in your repository to include a link to this notebook on github.


