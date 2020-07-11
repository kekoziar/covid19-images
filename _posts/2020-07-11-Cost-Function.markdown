---
layout: post
title:  "Cost Function"
date:   2020-07-11 07:01:53 -0700
categories: COVID-19 Timelapse

custom-css-list:
     - slider/image-slider.css
---
I posted this on my [FB back in March](https://www.facebook.com/shadowd1/posts/10157142375674632){:target="_blank"}. It's still a lesson worth learning.

In data science, there's this thing called a cost function. It estimates the cost of your predictions based on if you predicted right or wrong. What is the cost of actions plus inactions for each case?

Pretend we're using data science to predict if an xray image of luggage contains a bomb. What are the costs for all scenarios?

- You predict there is a bomb, and there is no bomb: people get mad from the inconvenience. (False positive)
- You predict there is no bomb, and there is no bomb: nobody notices. (True negative)
- You predict there is a bomb, and there is a bomb: crisis averted\*. (True positive)
- You predict there is no bomb, and there is a bomb: BOOM. (False negative)

So, you weight your predictions to minimize the cost. In this case, it's better to think something is there and get it wrong, than to think something is not there and get it wrong.

\*To extend one of the prediction scenarios: if you predict there is a bomb, and there is a bomb, not only is the crisis averted, but *very few people notice*. The people directly involved, sure, but the wider public doesn't notice anything changed, because to them life goes on. But the policies and actions to avert the crisis still happen, and are still needed. If those policies and behaviors are removed because of public pressure, the crisis is no longer averted.  We're back at the BOOM scenario.

This is why we plan. This is why we take precautions. And, this is why policies, actions, and behaviors should stay in place until we know the cause for crisis is gone.  


---
---
<br>
Comparing this week's new cases to four weeks ago.  

{% include slider/slider-20200710-4wks.html %}

---
---
<br>
And with last week.  

{% include slider/slider-20200710-1wk.html %}

---
---
<br>

### Timelapse, Created July 11, 2020

United States, normalized by population of each county
![US animated gif of COVID-19 cases]({{ "/images/gifs/covid-US-20200710-100k.gif" | relative_url }})
