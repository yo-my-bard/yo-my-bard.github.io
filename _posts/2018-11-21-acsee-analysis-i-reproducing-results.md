---
layout: post
title: "ACSEE Analysis I: Reproducing Results"
date: 2018-11-21 19:13
author: Yusuph Mkangara
comments: true
categories: [Education, Python]
---
After publishing my previous post, I took to Twitter to declare my desire to "ponder less, and push myself more" - an alliterative variation of a bias for action. For the last two months, I have focused on publishing Amazon skills. The process of publishing skills also provided ample opportunity for introspection. I've been thinking about what made me excited when I was growing up. So far, I think building things and creativity are central to who I am as a learner. At the tail end of high school, that meant constructing narratives in meter while thinking I wanted to be an engineer or doctor. Now that I'm leaning toward a STEM-like career again, I find the basis of commonality between my different stages so far lies somewhere in this amorphous notion of creative building. I engage fully with projects that allow me to be creative and to tinker with the solution and thankfully for me, programming has been a pleasant outlet for this work. To bring it back to the topic at hand, I am on Thanksgiving break this week and wanted to find something that I could use to practice coding. I didn't have a clear idea for something like a Skill and so I spent the first two days of the break desperately trying to write a wrapper for some common matplotlib plots for work. After electing to close up shop on that work, I felt unsatisfied and a little lost on what I could do next. Fortunately, I keep breadcrumbs of projects/ideas; a personal Trello board and Twitter are my favorite organization tools at the moment.<!--more-->

During the summer, there was <a href="https://www.thecitizen.co.tz/magazine/success/-Understanding-Form-Six-regional-results-puzzle/1843788-4690616-rcjhhd/index.html" target="_blank" rel="noopener">an article posted online by The Citizen</a> about Form 6 (advanced secondary school) results. I remember reading it and noticing that the top 3 regional performers were not who I would expect. I couldn't make sense of it and didn't quite know when I'd want to return to tackle it. After wrapping up my work with matplotlib, I was itching to jump into a more structured analysis.

The Citizen published an article with claims based on an analysis of the ACSEE exam results. I wanted to see if I could reproduce the statistics cited in the article. One way to learn with programming is to try to reproduce what others have made in the past. Particularly in research, creating an analysis or experiment that is reproducible by others is critical for credibility. As always, I posted <a href="https://github.com/yo-my-bard/Scraping-NECTA/blob/master/Reproducing_The_Citizen_Article.ipynb" target="_blank" rel="noopener">my Jupyter Notebook code on GitHub</a> - I strongly encourage trying to reproduce these numbers as well or conduct your own analysis! (Note: Data is available <a href="https://www.kaggle.com/yusuph/necta-test-results" target="_blank" rel="noopener">at Kaggle as well</a>). After pulling some metadata about the testing centers, I was able to reproduce most of the statistics provided in the article. This was overall encouraging news (though it does mean I have less to talk about in this blog)! One notable discrepancy was on the 55% of test takers earning Div I or Div II (passing results). My analysis found that this may be an overestimation (I had 50.5%) and consequently the reported 4.5% of students who received the lowest marks of Div IV and Div 0 may be an underestimation (I had 7%). Numbers were close enough or exact for the rest of the statistics; I do wonder why there might be discrepancy. It may be cynical of me, but I believe that there is a substantial change in perception between "50% of our students passed" and "55% of our students passed". Therefore, there is arguably an incentive to fudge the numbers a little. It is very possible that 55% is a statistic at which one could arrive, but it doesn't seem possible to do so by using the same methods/assumptions as all the other statistics.

I named this post <em>ACSEE Analysis I</em> because I think this data deserves another visit. For one, there isn't anything original/new here. Second, there is a wealth of metadata that I would like to add to the analysis particularly around school rankings. Finally, I think there are plenty of unexplored layers in this dataset:
<ul>
	<li>Gender</li>
	<li>Subject-based analysis</li>
	<li>Year over Year analysis</li>
	<li>Some combinations of the above</li>
</ul>
To that end, I look forward to the challenge of arriving at some novel ideas to share in the next blog post.