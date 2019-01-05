# 4104 is Second Place!

*January 6, 2018*

**Yoni Nazarathy**

![Blog header image](https://es-app.com/assets/2da9xx.jpg){.blog-image-header}

You can search the web for "*nobody remembers second place*" and get about $5,300$ search results. However if you search for the opposite: "*somebody remembers second place*" you get about 1.3 million  results! So is second place memorable or not? I guess it depends on who you ask.

Now when it comes to numbers, is there also a first and second place? Well I guess, you should define the competition. Here is one famous example:

**Find a number, $X$, as small as possible, that can be expressed as the sum of two positive whole cubes in more than one way.** 

Try for example the number $X=35$. You can write

$$2^3 + 3^3 = 35$$

As you can see it is the sum of two cubes. So this is one way. The question is now if there are other numbers, $a$, $b$ such that

$$a^3 + b^3 = 35$$

Try as you might, you won't find such $a$ and $b$. So the smallest $X$ is clearly not $35$. What is the smallest such $X$?

If you are a math enthusiast, or if you watched The Man who Knew Infinity, then you probably heard about the extraordinary Indian mathematician [Srinivasa Ramanujan](https://epsilonstream.com/topic/ramanujan).  In this clip from the movie, Ramanujan states that $X = 1729$ comes first. 

VIDEO

His friend and colleague, [G. H. Hardy](https://epsilonstream.com/topic/hardyMathematician), was not aware of such a "competition". Later in historical notes, Hardy mentioned Ramanujan's observation about $1729$:

$$9^3 + 10^3 = 1729 = 1^3 +12^3$$

Indeed Ramanujan was a remarkable man of numbers and mathematics. Few are the people who would recognise an arbitrary number like $1729$ and make such an observation about it:

**1729 comes in first place.**

You may watch this neat [Standupmaths](https://www.youtube.com/channel/UCSju5G2aFaWMqn-_0YBtq5A) video where Matt Parker tells us much more about Ramanujan's investigations:

VIDEO

---

So if $1729$ comes first who comes second? Is there a second? A third? How would you compute that? The following image of a simple Excel spreadsheet does the job:

IMAGE-SHEET

You can download our [example spreadsheet](), or you can try and create one of your own. It is nothing more than an "addition table" of the cubes $1$, $8$, $27$, $64$,... all the way up to $15625$ ($25$ cubed). You can then inspect it visually and see that $1729$ is the first such duplicate value. So who comes second?  You got it: $4104$.  

$$9^3 + 15^3 = 4104 = 3^3 + 16^3$$

Actually, when creating such a sheet, you don't have to visually inspect. You can also try to use Excel's conditional formatting and have Excel highlight duplicate values.

---

There is much more to discover about the sequence $1729$, $4104$, $13832$,.... and related sequences.  Some more information is in [this page](http://www.durangobill.com/Ramanujan.html). You can also search for ["1729"](https://epsilonstream.com/topic/1729) in our free Epsilon Stream App to find out more.