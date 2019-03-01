# Epsilon Stream and Global Math Week

**Nicholas Bartlett**

![Blog header image](https://es-app.com/assets/45sxj3.jpg){.blog-image-header}

The key force that drove us to create our premier free platform, [Epsilon Stream](https://oneonepsilon.com/epsilonstream/), is the spectacular mathematics content on YouTube. Dozens of incredible creators upload engaging, precise, surprising and useful content, dealing with almost every aspect of exploratory and educational mathematics.

At One on Epsilon, a key mission of our [content team](https://oneonepsilon.com/epsilonstream/#content-team) is to organize and present this content in a manner that is useful for students, educators and enthusiasts. To do that, we regularly call upon our experts to personally sort, evaluate and select the best mathematics videos. Members of our team are equipped with a proprietary back-end software tool that we created for this purpose. The fruits of our labor are then found in the free Epsilon Stream platform. 

But that is not all. Clearly, with the aid of [machines](https://epsilonstream.com/blog/machines-and-mathematics-play-together/), we can understand more about the YouTube content, its significance, volume, usage and the like. For this we began a data science project, mining information from YouTube, specifically focusing on mathematics content. Our goal with this project is to better understand the world of YouTube mathematics, as well as to deliver interesting bits of information and summary statistics to the hard working community of [YouTube mathematics content creators](https://epsilonstream.com/blog/incredible-mathematics-on-youtube/).

Our [first report](https://oneonepsilon.com/epsilonstream/#data-analysis) in this project is quite brief and minimal. We plan to update the figures in this report on a monthly basis. It currently reads as follows:

> We conduct an on-going survey of YouTube mathematics usage. For the month of July 2018 our conservative estimate indicates that in the English language alone, there were 1.8 million hours of mathematics views. Yes, that is 1,800,000 hours of mathematics videos educating, engaging and exploring audiences!
> 
> This is equivalent to 2 million people, each watching 12.5 minutes of mathematics videos per week!
> 
> This conservative estimate excluded significant channels such as Khan Academy, TED-ED, minute physics and Vsauce. 

Translating 1.8 million hours of viewing to the (example) statistic of 2 million people, each watching 12.5 minutes a week is rather straightforward. But how did we get the number 1.8 million? We now outline a few details.

Our data collection system operates by periodically pulling information through the [YouTube API](https://developers.google.com/youtube/v3/). This is an open free service that YouTube provides for the general public. We capture viewing information for a list of mathematics videos, published by channels that we know produce mathematics content. See [our survey](https://epsilonstream.com/blog/incredible-mathematics-on-youtube/) of many of these channels.

Our list of videos currently contains more than 34,000 videos! There is a possibility that some of the videos in our database are not mathematics videos, but given the channels that we use for the collection, these are a minority.

To calculate the hours of mathematics viewed in July, first we determine how many times each video in our database has been viewed in July. YouTube videos keep a running total of how many times they've been viewed since they were first posted - this is called the view count. With our data collection system, we know the view count of each video at any point in time - the difference in the view count between the start and end of the month is the number of views in that month! For videos with a view count higher than 300, YouTube applies a special filtering algorithm to make sure that view counts are not being pumped up by web bot activity or by attempts to game YouTube’s statistics. This makes view counts much more reliable and useful!

Then we multiply the number of views in July by the duration of the video. We then multiply this by 0.35. This is our guesstimated magic constant which allows for the fact that not every viewer watches a video all the way to the end. Note that we are trying to be as conservative as possible in our estimate. Communication with creators such as [James Tanton](http://gdaymath.com/about/), the mastermind behind [Exploding Dots](https://www.explodingdots.org/) and [The Global Math Project](https://www.globalmathproject.org/), indicate that typical numbers may be at values of around 0.40 or even 0.50 depending on the type of video and the time of year. 

Finally, we sum up all the individual video viewing hours and - voilà! This gives us an estimate for the total number of hours of mathematics content watched.

---

This is just the starting point of our data science process supporting Epsilon Stream. There will be more to come and more refined updates of the mathematics watch rate. Some highly viewed channels such as TED-ED and Khan Academy were not included in this initial survey because we didn't want to accidentally count videos that are not about mathematics. Our future updates will be able to count specific videos from these channels and others that deal with mathematics. 

Stay tuned for more by [registering with us](https://oneonepsilon.com/register/) and/or following on [twitter](https://twitter.com/oneonepsilon). 
