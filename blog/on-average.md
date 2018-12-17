The full blog post is still accessed through [here](https://www.1onepsilon.com/single-post/2018/07/21/What-do-you-mean-on-average-Arithmetic-Geometric-or-Harmonic). We are in the process of moving it to the current location.


# Why use the geometric mean? Why harmonic?
*July 21, 2018*

**Yoni Nazarathy**

![Blog header image](https://es-app.com/assets/34xnA8.jpg){.blog-image-header}

How often do you think about averages? In my case, there isn't a day that goes by in which I don't think about some sort of "average". However, when I do so, I seldom have a specific mathematical concept in mind. Instead I think about the average representing a "typical value". 

For example, when I shop for 

One can either postulate about such typical values, or obtain them from data. When considering data, the most common the most common is the **arithmetic mean**. To caluculate it given, a collection of $N$ numbers, $X_1,\ldots,X_N$, we have,
$$
\text{arithmetic mean} = \frac{X_1+\ldots+X_N}{N}.
$$
For example try to think about how many times you <a href="https://www.youtube.com/watch?v=U9cGdRNMdQQ">smile per day</a>.  Say that over a period of three days, we record the following number of smiles per day
$$
X_1=25,\quad
X_2=15, \quad
X_3=50.
$$
In this case, summing up the values and dividing by $3$, the average number of daily smiles is $30$. 

--

However, there are other ways of describing typical values, often referred to **measures of centrallity**. For example as discussed <a href="https://www.1onepsilon.com/single-post/2017/05/27/Choosing-a-Fair-Estimate">here</a> we can also use the <a href="http://epsilonstream.com/search?q=median">median</a>. Then there are also weighted averages and a variety of other varients such as the <a href="https://en.wikipedia.org/wiki/Truncated_mean"> truncated (trimmed) mean</a>. Another related term is <a href="http://epsilonstream.com/search?q=mathematical+expectation">mathematical expecation</a> dealing with an average of a probability distribution as opposed to the average of data. 

Other alternatives to the arithmetic mean include the **geometric mean** and **harmonic mean**. Some students, study these for the case of two data points, $X_1$ and $X_2$ as part of their high school studies (see for example QQQQ). Then, some data scientistis understand why they are usefull in their applied work (see for example QQQQ).

So why are there so many alternatives to describe the "typical value"? Which alterantive should we use? 

Let's not focus on all the possible common measures of centrallity. Instead, let's consider two less popular friends of the arithmetic mean. These are the **geometric mean** and **harmonic mean**. You might have heard about these two alternative types of means before. But do you what are they good for?

--

To motivate the situation consider three scenarios where we make use of an average value, $A$:

**(i) Total calculations**: Say you are about to carry $N$ items and wish to estimate the total weight you will carry. In this case, if $A$ is the average item weight, then clearly,
$$
\text{total weight} = N \times A.
$$

**(ii) Return on investment calculations**: Say you invest $K$ dollars in a variable return account for $N$ years. If the average growth rate per year is at a rate of $A$ then after $N$ years you have:
$$
\text{return} = K \times A^N.
$$
This is because during the first year, your dollar grows to be $K\times A$ and after two years it is $K \times A \times A$, etc...

**(iii) Distance-time-speed calculations**: Say you are travelling for a distance of $N$ kilometers at an average speed of $A$ kilometer/hour. In this case, the time travelled is:
$$
\text{total time} = \frac{N}{A}.
$$

--

In each of the cases (i)--(iii), the average value $A$ signifies a typical quantity. That is a typical weight in case (i), a typical growth factor in case (ii) and a typical speed in case (iii). Indeed, if all we are presented with is the value $A$, then we would probably use the above formulas without trouble.

--

However, what if we are actually given data matching each of these scenarios? How would we compute the average matching the data? For example, what if $N=4$ and we were given,
$$
X_1 = 1.05,\quad
X_2 = 0.85, \quad
X_3 = 1.2, \quad
X_4 = 1.5.
$$
The meaning of $X_1,\ldots,X_4$ would vary depending on the context.
For case (i) these values represent 4 individual weights, say in kilograms. For case (ii) these values represent growth factors for each of the 4 periods. For example the value $X_1=1.05$ represents growth by $5\%$ and the value $X_2=0.85$ represents decay by $15\%$. Then for case (iii) let's assume that these values represent the speeds taken over consecuative miles. That is $X_1=1.05$ represents a speed of $1.05$ km/h during the first kilometer of motion, etc... these are quite slow speeds... but perhaps signify the speeds you would use when walking over tight rope (this is still a bit unrealistic because the world's longest tightrope walk record is for 547 meters).

Now with such a meaning for these values, how would we compute the average, $A$? It turns out, that each case has an ideally suited average. These are the **arithmetic mean**, the **geometric mean** and the **harmonic mean**.

Without further delay, lets compute these three means:

**Arithmetic mean** - this is simply the sum of the values divided by the total number of values:
$$
A_a=\frac{X_1+X_2+X_3+X_4}{4} = 1.15.
$$

**Geometric mean** - this is a product of the values and then taking the $N$'th root of it. For example if there were only two values, you would multiply them and take their square root. In our case, $N=4$:

$$
A_g=\sqrt[4]{X_1 X_2 X_3 X_4} = 1.1258232.
$$

**Harmonic mean** - This is the inverse of the arithmetic mean of the inverse of the values. That is, instead of a value $X_i$ consider $1/X_i$, sum up these values and divide $N$ by that sum. For $N=4$ we have:
$$
A_h = \frac{4}{\frac{1}{X_1} + \frac{1}{X_2} + \frac{1}{X_3} + \frac{1}{X_4}} = 1.102277
$$

You can observe that the average values that we get are not exactly the same. Infact,
$$
A_h \le A_g \le A_h,
$$

and this inequality can be shown to hold for any data values, $X_1,\ldots,X_N$. Still, as you probably use the arithmetic mean all the time, why do we need geometric mean and harmonic mean?

--

To see the strength of each of these means, let's return to the cases (i), (ii) and (iii) above. Remember that an average is supposed to serve as a "typical value". Ideally, it can replace the actual data values. 

So let's see. Consider formula (i) and replace $A$ by $A_h$:

$$
\text{total weight} = 4 \times A_h = 4 \times  \frac{X_1+X_2+X_3+X_4}{4} = X_1+X_2+X_3+X_4.
$$
That seems to work well! As desired, the total weight is exactly reproduced.

Now consider formula (ii). What type of mean should we use in place of $A$? As you can guess, $A_g$ does the job:

$$
\text{return} = K \times A_g^N = \Big(\sqrt[4]{X_1 X_2 X_3 X_4}\Big)^4 = K  X_1 X_2 X_3 X_4.
$$

You see, by using the geometric mean, $A_g$, the exact return rate is retrieved.

As you might expect now, the harmonic mean works perfectly for case (iii). Use $A_h$ in place of $A$ to obtain:
$$
\text{total time} = \frac{4}{\frac{4}{\frac{1}{X_1} + \frac{1}{X_2} + \frac{1}{X_3} + \frac{1}{X_4}}} = \frac{1}{X_1} + \frac{1}{X_2} + \frac{1}{X_3} + \frac{1}{X_4}.
$$
This is also the desired quantity. Since on each kilometer we had a different speed $X_i$ and the time for kilometer $i$ was $1/X_i$.

--

So you see, there are different ways to average depending on the context. In practice, the arithmetic mean is the most common way, however for specific contexts involving growth rates, the geometric mean works better and for contexts involving rates the harmonic mean does the job.

Have you ever used the geometric or harmonic mean? Let us know.

