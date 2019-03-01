The full blog post is still accessed through [here](https://www.1onepsilon.com/single-post/2017/06/17/Neglect-and-Respect-a-Quarter-of-a-Percent). We are in the process of moving it to the current location.

# Neglect and Respect a Quarter of a Percent

*June 17, 2017*


**Coco Bu and Yoni Nazarathy**

<center>
 <img class = "blog-inline-image" src="https://es-app.com/assets/OOTR35.png" alt="drawing" width="250px"/>
</center> 

The other day Coco and Yoni caught up to discuss their journey with One on Epsilon. They started talking about mathematics, curiosity and education. Quite quickly they got onto the subject of children and teenagers. Yoni is the father of three children and Coco interacts with dozens of teenagers as a school teacher.

Yoni mentioned that his eldest daughter is going on a school trip to Australia's capital, Canberra. It's her first time being away from home for several days. Yoni sounded a bit anxious, but mainly proud of his daughter. Just yesterday she was his baby, and now she has grown up so fast to become an engaging and curious young person.

Without noticing, Coco and Yoni's conversation moved onto math...

---

**Coco:** So, does it really feel like your daughter grows fast? How does that happen? If you were to consider one attribute such as her height, how fast do you think her height increases? 

**Yoni:** At this point in life, I reckon my daughter's height increases by about 5% every year. I haven't looked deeply into it, but if you ask me, that would be my guess. Actually, I wonder, 

**If her height increases by 5% each year, 
does that mean that over a period of 2 years, it would increase by 10%?** 

**Coco:** Well, yes and no. If you say the growth in height is roughly 5% per year, you can say that over a two-year period the growth in height is roughly 10%. However, if you say that the growth rate is exactly 5% per year, then your calculation is not that accurate. You are actually off by a quarter of a percent.

**Yoni:** Really? How come? Tell me more.

**Coco:** Why don't you do the calculation yourself? I will assist you. Let's say your daughter is 1 meter tall now, that is 100 centimeters (about 3 ft 3 in). If her height increases by exactly 5% each year, how tall will she be in a year's time?

**Yoni:** I think she will be 105 centimeters tall, right? I know that,

$$
\mbox{Current height} + \mbox{Height growth in a year} = \mbox{Height next year}
$$
 
In an equation, it should be,

$$
100 + 100 \times 5\% = 100 \times (1 + 0.05) = 100 \times 1.05 = 105
$$
 
**Coco:** Yes, you are right. But you know what? You just discovered that multiplying the current height by 1.05 gives you the height in a year with 5% growth. The number 1.05 is called the growth factor.

**Yoni:** Oh, I see. Similar computations occur in finance and investment, right? For example, if I deposit \$1,000 in the bank with 5% interest rate per year, then by next year I will have $1000 \times 1.05 = \$1,050$.

**Coco:** Exactly. Do you want to know your daughter's height in two years? 

**Yoni:** Since you reminded me the meaning of multiplying by the growth factor 1.05, I just need to multiply by it twice. So it is:

$$
100 \times 1.05 \times 1.05~~\mbox{or}~~ 100 \times 1.05^2 \qquad (\mbox{squared})
$$
 
Let me calculate. Oh, it is $110.25$ centimeters. 

**Coco:** Yes, 110.25 should be her height in two years but your initial guess wasn't exactly this. It is off by a quarter of a percent.

**Yoni:** So, at the beginning I guessed her height grows by 10% in two years, which should be 110 centimeters. The difference between the accurate calculation and my estimation is 0.25 centimeters. That is indeed a quarter of a percent of her original height. How did you know that this was the error from the start?

**Coco:** It is all related to this equation:

$$
(1 + \epsilon)^2 = 1 + 2 \epsilon + \epsilon^2.
$$

**Yoni:** Whoa, whoa, whoa, Coco. Hold on! What do you mean? What is that symbol?

**Coco:** That is Epsilon, just like in One on Epsilon:

Take Epsilon = 0.05. In this case the growth factor is $1.05$, and over two years it is $1.05^2$, which can be written as $(1 + 0.05)^2$.

**Yoni:** Still, I don't understand the equation. Where does it come from? Why is it needed?

**Coco:** Let me first answer your first question. The equation comes from this algebraic identity: 

$$
(a+b)^2 = a^2 + 2ab + b^2
$$

where $a = 1$ and $b = \epsilon$. Now to answer your second question. Keep in mind that Epsilon = 0.05 and this is small compared to 1.

**Yoni:** So?

**Coco:** Notice that a small number squared gets even smaller. In this case, $\epsilon^2 = 0.05^2 = 0.0025$. That is our quarter of a percent. Hence to approximate, you can neglect $\epsilon^2$ from the first equation and get:

$$
(1+\epsilon)^2 \approx 1 + 2 \epsilon
$$

**Yoni:** Oh, I see. That is why you were saying I was off by a quarter of a percent because $\epsilon^2$ was neglected in my original estimation. Can we now explore the algebra of it? Can you describe more, Coco?

**Coco:** Consider the $(a+b)^2$ formula from above, where does it come from? 

It comes from the expansion of brackets and distributive law, like this:

QQQQ

If you want to revise your knowledge on expanding brackets and how to use the distributive law, watch this neat Mathantics video:

Another way to understand this formula is to consider a geometric representation. Imagine we have a square of side length $(a+b)$, then $(a+b)^2$ is the total area of this square.

In our example using the height of Yoni's daughter, a = 1 and b = Epsilon = 0.05. This square then has side length (1+Epsilon) or (1+0.05); hence area (1+0.05)^2. Now, break this square into four parts like this:



Can you pick out the individual parts from the formula?

The gray square region has side length 1 and hence area 1. Each of the blue rectangular region has side lengths 0.05 and 1; hence area 0.05. Two of them make the area be $2 \times 0.05$. The red square region has side length 0.05. What is the area of this red square?

You guessed it. It is 0.0025, which is the "quarter of a percent". The area of the red square region is very small compared to the area of the entire square, that's why you may neglect it if approximating.

**Yoni:** Whoa Coco, thank you! You know, when I was in my teenage years I was always intimidated by basic algebra. But now it seems so clean and useful to me. My father was actually always trying to help me with this stuff, but I somehow couldn't do it well. I guess I had to grow a bit in order to fall in love with mathematics.

**Coco:** I'm glad we could discuss, it would be fun to explore more another day. Perhaps I can leave you with a related problem today: If you were to invest \$100 in something risky and first loose 5% and then gain 5%. How much money would you end up with?  Do you believe you would end up having your \$100 back, or loose a bit, or earn a bit? Hint: Consider "growth factors" of 0.95 and 1.05.

![Blog header image](https://es-app.com/assets/OOTR35.png){.blog-image-header}
