---
toc: false
layout: post
description: Some notes on significant figures.
categories: [markdown]
title: A Significant Confession
---
# A Confession
It was a cold winter evening in January.  My son brought me his Chemistry test for grading, and I noticed a disturbing trend. All of his calculated answers were just a little off. I could tell that he was making errors due to not dealing properly with significant figures.As a practicing data scientist, you can imagine how heart wrenching this was. My own son.

I called him in and asked him to sit down. He knew I had something serious to discuss. I showed him his test with the marks, expectinging nothing else needed to be said. He seemed unmoved.

Finally, I asked him: Where did you learn such disregard for precision and significant figures?" His answer cut me straight to the heart. 

"I learned it from you Dad."

I staggered and fell back into my chair. 

He was right. 

I, like every other technical person, snickers at the sight of a measurement in inches that indicates precision at the atomic level. But I realized, there are cases that I don't really understand. 

I've been peripherally aware of the rules, but I have a confession: I've been winging it, just like my son has been.

I realized that the problem for me was I never intuitively picked up the rules because there are legitimately ambiguous cases. 

How many significant figures are in the number *100*? 

It has at least one. If we wanted to communicate there are 3, we could
always write *100.* But surely there exist situations where we know we
have 2. How do we specify that? 

#An obnoxious old friend to the rescue

It turns out, scientiic notation is more than just the occassional obnoxious output from numpy necessitating I look up again how to supress it... it serves the purpose of specifying precisely what we know. 

*1 x 10^2* has 1, *1.0 x 10^2* has 2, and *1.00 x 10^2* has 3 significant figures.

