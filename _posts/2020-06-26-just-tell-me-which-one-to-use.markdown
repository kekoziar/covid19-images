---
layout: post
title:  "Just Tell Me Which One to Use!"
date:   2020-06-26 06:42:53 -0700
categories: COVID-19 Racial Disparities
image:
 path: /images/jpg/COVID-19_CA-Demographics_graphs_20200625-all_Page_5.jpg


---

*(California demographic visualizations are at the bottom of the post.)*

A tendency I sometimes observe in data science is a belief that visualizations, algorithms, and analysis methods - data science tools - can be applied the same way on any data. This belief that the data will magically reveal itself after using standard (or even custom) tools actually causes all sorts of problems which have been 
[extensively](https://safiyaunoble.com){:target="_blank"} 
[documented](https://www.goodreads.com/book/show/38212110-technically-wrong){:target="_blank"} 
[by](https://www.goodreads.com/book/show/34964830-automating-inequality){:target="_blank"} 
[others](https://www.goodreads.com/book/show/42527493-race-after-technology){:target="_blank"}.  These authors often focus on the need for good training data for the machine learning algorithms, so the edge cases are represented. And, that’s part of it. You also need to understand the different aspects of the methods you’re using, because algorithms, visualizations, and analysis methods *are* biased. They can highlight certain parts of the data, while obscuring others. (Also [well](https://www.goodreads.com/book/show/51291.How_to_Lie_with_Statistics){:target="_blank"} [documented](https://www.goodreads.com/book/show/28186015-weapons-of-math-destruction){:target="_blank"}). If all you have is a hammer, everything starts to look like a nail.

The *purpose* of your analysis will add conditions that helps you to narrow and select a proper tool, but before you get there, you also need to know what your data is *about*.  “Aboutness” is a nice library science term that allows you to explore data (or really, anything). In terms of LIS, it’s often used to help discover and then describe the subject of an item to be cataloged. But, IMO it means more than just a subject; it can be used to describe the (simple to complex) essence of an object.  In terms of other sciences, it can also be correlated with boundary conditions and data gathering/creation methods. 

I like the term “aboutness” because it allows you to explore using natural language. Name everything you know about a dataset, and you’ll have both described its “aboutness” and likely created a really good framework for its metadata. And, if you can't describe your data well, maybe you should take some time getting to know it before you use it.

*(I'm re-reading my post, and on the surface it seems like it's all over the place. What's important? knowing your tools or knowing your data?  They're both important and need to be used together. If you use one without the other, you will exaggerate the bias which already exists in both your data and your tools.)*  
<br>

---

---
<br>

I started thinking recently about this in terms of visualizations because of something a materials engineering PI told me years ago as I created graphs for a report and article. He insisted the axes of the different graphs were all uniform so we could easily compare the results. And so, my default is now to standardize axes so we can easily compare across graphs. And, this works well in certain cases, such as using the below graphs to select an alloy and heat treatment for a particular tensile strength. Obviously, we want Alloy A and will disregard Alloy C & D if we're looking to improve tensile strength.

| --- | --- |
| ![Combo Bar/Line Graph of Fake Materials Science Test Data]({{ "/images/jpg/Fake-Materials-Process_graphs_20200625_Page_1.jpg" | relative_url }}) | ![Combo Bar/Line Graph of Fake Materials Science Test Data]({{ "/images/jpg/Fake-Materials-Process_graphs_20200625_Page_2.jpg" | relative_url }}) |
| ![Combo Bar/Line Graph of Fake Materials Science Test Data]({{ "/images/jpg/Fake-Materials-Process_graphs_20200625_Page_3.jpg" | relative_url }}) | ![Combo Bar/Line Graph of Fake Materials Science Test Data]({{ "/images/jpg/Fake-Materials-Process_graphs_20200625_Page_4.jpg" | relative_url }}) |

But, now look at the graphs with the real metadata, which are COVID-19 case/deaths demographics compared with California population demographics.  When the real metadata is revealed, you can see that standardizing the y-axis actually obscures an important aspect of the data, specifically that the rates of cases and deaths are in certain cases double the percentage represented in the population.  

| --- | --- |
| ![COVID-19_CA-Demographics, Latino]({{ "/images/jpg/COVID-19_CA-Demographics_graphs_20200625-1-4_Page_1.jpg" | relative_url }}) | ![COVID-19_CA-Demographics, White]({{ "/images/jpg/COVID-19_CA-Demographics_graphs_20200625-1-4_Page_2.jpg" | relative_url }}) |
| ![COVID-19_CA-Demographics, Black]({{ "/images/jpg/COVID-19_CA-Demographics_graphs_20200625-1-4_Page_3.jpg" | relative_url }}) | ![COVID-19_CA-Demographics, Asian]({{ "/images/jpg/COVID-19_CA-Demographics_graphs_20200625-1-4_Page_4.jpg" | relative_url }}) |



And so we adjust the axes to the data.  Because one size does not fit all for data science or visualizations. 

Get to know your data. Learn everything about it. Who does it involve?  Who can it harm? Then, instead of throwing brute force at the data and hoping something sticks, you can think about your data, and develop an elegant and time saving approach that takes into account all stakeholders of the data. 

This also means we need to increase data literacy in general.  As viewers and consumers of information, we should be cognizant of data and graphs presented to us.  Look at the whole of a graph. What is it about? What story is it telling? And, what story is being overlooked?

​​​![COVID-19_CA-Demographics, ​Latino]({{ "/images/jpg/COVID-19_CA-Demographics_graphs_20200625-all_Page_8.jpg" | relative_url }})

![COVID-19_CA-Demographics, White]({{ "/images/jpg/COVID-19_CA-Demographics_graphs_20200625-all_Page_7.jpg" | relative_url }})

​​![COVID-19_CA-Demographics, ​Asian]({{ "/images/jpg/COVID-19_CA-Demographics_graphs_20200625-all_Page_6.jpg" | relative_url }})

​​![COVID-19_CA-Demographics, ​African American/Black]({{ "/images/jpg/COVID-19_CA-Demographics_graphs_20200625-all_Page_5.jpg" | relative_url }})

​![COVID-19_CA-Demographics, ​Multi-Race]({{ "/images/jpg/COVID-19_CA-Demographics_graphs_20200625-all_Page_4.jpg" | relative_url }})

​![COVID-19_CA-Demographics, ​American Indian or Alaska Native]({{ "/images/jpg/COVID-19_CA-Demographics_graphs_20200625-all_Page_3.jpg" | relative_url }})

​![COVID-19_CA-Demographics, ​Native Hawaiian and other Pacific Islander]({{ "/images/jpg/COVID-19_CA-Demographics_graphs_20200625-all_Page_2.jpg" | relative_url }})

![COVID-19_CA-Demographics, Other]({{ "/images/jpg/COVID-19_CA-Demographics_graphs_20200625-all_Page_1.jpg" | relative_url }}) 


---

Data is from tables on 
[the California Department of Public Health](https://www.cdph.ca.gov/Programs/CID/DCDC/Pages/COVID-19/Race-Ethnicity.aspx#){:target="_blank"} webpage. 
Also note, about 30% of the cases are missing race/ethnicity information according to the CDPH page.

