# May the Odds Be Ever In Your Favor

**Clara Valtorta and Yoni Nazarathy**

![Blog header image](https://es-app.com/assets/3h3h3h.jpg){.blog-image-header}

*Update*

**We got an insightful email from a reader which pointed out a problem with our original model. When you read the simplified example, think about the following question. Is a randomly selected person more likely to live on a street with two or three houses?**

**The post will soon be updated with the correction. Thank you Andres!**

---

A few years ago, a Facebook poll asked: "Do you live in an odd numbered house or an even numbered house?" Outright, it is not the most interesting of questions, but watching James Grime's engaging video describing the surprising results may change your mind. After watching this video, we decided to squeeze a bit more mathematical exploration out of the poll results.

---

So, let's start with an overview of results of the poll. As described by James Grime, the first results he saw were 125,710 odd and 124,653 even. A few days later, the results were 211,803 odd and 209,964 even. So, in both cases, about 50.2% of the participants reported living in an odd numbered house. A natural question is: Why not exactly 50%?

One may initially believe that such a seemingly slight deviation from 50% is due to statistical error. For example, if we tossed 1000 fair coins, there would be nothing surprising if 502 of them landed on tails. However, with the large sample size of the poll, it is not statistically likely to obtain these results if the true probability for odd is really 50%.

Still, why?

YOUTUBE VIDEO

Even though in general, there are just as many even numbers as odd numbers, consider streets with an odd number of houses. Generally, they will have one more odd numbered house. For example, a street with three houses would have houses numbered 1, 2 and 3. That is two odds and only one even.  A street with 11 houses would have six odd numbered houses and only five even houses. Notice though, that the more houses on the street, the less the percent of odd houses differs from 50%. For example, a street with 1001 houses has 501 odd houses, which is about 50.05%. And a street with 4501 houses has about 50.01% odd. Still, when averaging over all possible street sizes, there are slightly more odds than evens.

This is where we went a step further. Based the results of the poll, this was our objective:

**We want to estimate the number of houses per street.**

We found out that on average, there are 644 houses per street. At least that is our estimate. How did we do that?

Before we dive in, let's assume a simpler, hypothetical situation. We live on a planet with only two types of streets: those with two houses, and streets with three houses. We'll use the percent of people living in odd numbered houses from the poll, or 0.502. In our equations, α represents this proportion; so α = 0.502. We do not know the proportion of streets that have two houses or the proportion of houses that have three houses. Let's define the unknown proportion of streets that have two houses as p. Then, (1 - p) is the proportion of streets that have three houses. 

Let N equal the number of houses on a street. If N is 2, the probability of a randomly selected house on that street being odd is 1/2. If N is 3, or there are 3 houses on the street, the probability of a randomly selected house on that street being odd is 2/3.

EQ

Here we use the idea of conditional probability. The strength of conditional probability is that it allows us predict the value of α by conditioning on the value of N. To do this, we'll find the sum of the products of the probability of randomly selecting an odd house for each value of N and the proportion for that value of N. Here it is:

EQ

We can solve for p to represent it in terms of α.

EQ

The expected number of houses per street, or E[N], can be represented by the following equation.

EQ

Can you explain why we multiplied p by 2 and (1 - p) by 3?

Previously, we found p in terms of α. Now substitute that expression for p, and we get this expression for E[N].

EQ

We can now use this expression. When α = 0.502, E[N] = 2.012. That is, under the (unrealistic) assumption that there are two or three houses per street, the expected number of houses per street is just slightly over 2. What if the poll reported the percent of odd numbered houses as 60%, or α = 0.6? Then the expected number of houses per street would be 2.6.

Extension Questions: What is the maximal α possible? What is the minimal?

IMAGE

And now back to reality.... streets do not only have two or three houses. In reality, for a randomly chosen street, the number N is a random variable that can essentially take any positive integer value. However, we are still interested in estimating the number of houses per street, or E[N].

When we assumed N could only be 2 or 3, it was clear that the probability distribution of N was determined by the single number, p. However, for a more general N, there are many options for its form and shape of its distribution. Which one should we choose?

Here there isn't a single correct answer. In fact it is here where, if we don't have other information, we need to make a leap and make some choices. It is here where mathematical analysis transforms into mathematical modelling. We needed to chose a distribution that on the one hand appears realistic and plausible while on the other hand is easy enough to manipulate mathematically. We chose a geometric distribution. 

With the geometric distribution, the chance of N = k, is given as follows:

EQ

Here the parameter p is a number in the range (0, 1). If you know about infinite geometric series, you can check that the sum of probabilities above, over k = 1, 2, 3,... up to infinity equals 1. With a bit more algebra, you can even verify that E[N] = 1/p.  

---

Now, having assumed a geometric distribution, we can do some computations and try to obtain E[N]. For this, the key formula is

EQ

As we had in our simpler, hypothetical situation, the equation relates α with the unknown parameter p. Only this time, since N can take any value of k = 1, 2, 3, 4, ..., we need to sum over all possible (infinite) possibilities. If you want a refresher on this Sigma (summation) notation, check out this video. 

Now we ask, what is the probability that a randomly chosen house on a street with N houses is odd?

Well, for an even value of k this conditional probability is just 1/2.  Then for an odd value of k it is (k + 1)/(2k). Can you see why? Try it for k = 1, 3, 5, and 7.

With these ingredients in place, all that remains is to try and find the p which yields the correct α. This isn't done with analytical ease, so we approximate this value with numerical computations. Details are here. Our end result is that E[N] = 644.

**We estimate that the mean number of houses on each street is 644.**

Is it really the mean street size? Frankly it seems a bit high. Still, it is not an unreasonable estimate and the nice thing is that it is based on a single empirical number 0.502 and some cool mathematics and modeling.

---

Where else in science, geography or engineering does one make such leaps and go from a measured number such as 0.502 to an estimate such as 644? We believe there are plenty of cases where such practice takes place. Where? What do you think of these mathematical leaps? Let us know. 