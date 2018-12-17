The full blog post is still accessed through [here](https://www.1onepsilon.com/single-post/2017/07/15/Seeking-Patterns-with-Math/). We are in the process of moving it to the current location.

# Seeking Patterns with Math

*July 15, 2017*

**Yousuf Marvi and Phillip Isaac**

<center>
 <img class = "blog-inline-image" src="https://es-app.com/assets/4fiwXA.jpg" alt="drawing" width="250px"/>
</center>

Is math important to you? Is it because you make use of basic math facts in your daily life, such as when you go shopping or [walking down the street](https://nrich.maths.org/5546)? Sure, but some people use it for technical work in fields such as finance, engineering, chemistry and architecture, just to name a few. Pretty much every field has some math applications. Math can be an incredibly useful tool. Is it a mistake, however, for us to think of math as only being a tool? We believe it is so much more. 

In fact, math can be studied for its own sake. As [Arthur Benjamin](https://www.math.hmc.edu/~benjamin/), author of [The Magic of Math: Solving for x and Figuring Out Why](https://www.amazon.com/Magic-Math-Solving-Figuring-Out/dp/0465054722/ref=asap_bc?ie=UTF8), beautifully says, “*Math is the science of finding patterns.*” Those patterns could involve anything from numeric sequences to geometric relationships. For example, **modular arithmetic**, first developed by [Carl Friedrich Gauss](https://en.wikipedia.org/wiki/Carl_Friedrich_Gauss), is a type of arithmetic done on a **number circle** rather than a **number line**. Numbers reset to $0$ upon reaching a certain fixed number. The classic example is arithmetic on a clock: when we get to $12$, the count resets to $0$. So, for example, on a clock, $10$ o’clock plus $4$ o’clock equals $2$ o’clock. This is mod $12$ arithmetic.

While modular arithmetic does have some wonderful properties, one of its major practical uses only came about in the 1970s when mathematicians used it in developing [RSA encryption](https://simple.wikipedia.org/wiki/RSA_algorithm) -- a method used to send and receive secure data like [private love letters](http://theconversation.com/the-rsa-algorithm-or-how-to-send-private-love-letters-13191).

In a short ten minute [Numberphile](https://www.numberphile.com/) video [James Grime](http://singingbanana.com/) wonderfully explains how the RSA key works:

[Encryption and HUGE numbers - Numberphile](https://epsilonstream.com/video/w1tn50)

If math is the science of finding patterns, then how do we actually find them? Well, there may be many avenues; here, let’s consider two popular themes:

1) **Induction**: we find a new or a unique rule that helps explain the pattern.

2) **Deduction**: we use other existing patterns to help uncover the new pattern.

In this blog, we will use the deductive method to help us solve the following puzzle:

<center>
 <img class = "blog-inline-image" src="https://es-app.com/blog-assets/seekingPatternsWithMathImage2.png" alt="drawing" width="250px"/>
</center>

In the above diagram, we have two primary shapes: a quarter circle with a radius, $r$, of length $6$ inches, and a rectangle inscribed inside the quarter circle whose side lengths of $x$ and $y$ add up to $8$ inches. The problem is to find the area of the white triangle.

---

To solve this problem, we can use our existing knowledge of these shapes (hint: deduction). Observe that the area of the white triangle is half the area of the rectangle with sides of length $x$ and $y$ as in the picture.

<center>
 <img class = "blog-inline-image" src="https://es-app.com/blog-assets/seekingPatternsWithMathImage3.png" alt="drawing" width="250px"/>
</center>

Now, since the area of the whole rectangle is $xy$ (that is, $x$ multiplied by $y$), the area of the white triangle is:

Area = $\frac12 xy$

Identifying the area *formula* is a really important step. What we need now is a way to calculate $xy$. Well, don't forget that the problem teases us with a clue: $x + y = 8$. Unfortunately, this equation alone is not enough to find $xy$. We need something else.

Actually, there is a very special pattern hidden in this picture. We know that when we are attempting to measure a missing side length of a right-angled triangle, we can use [Pythagoras' Theorem](https://www.1onepsilon.com/single-post/2017/05/13/Cut-corners-and-save-up-to-29):

$$a^2+b^2=c^2$$

Clearly, we can tell that the perpendicular side lengths $a$ and $b$ in the formula will be substituted by $x$ and $y$, but what about $c$ - the hypotenuse?  Before you read on, give it a try on your own.

<center>
 <img class = "blog-inline-image" src="https://es-app.com/blog-assets/youngGirlReachingHigh.jpg" alt="drawing" width="250px"/>
</center>

Notice that the hypotenuse of the triangle we are interested in has the same length as the radius of the circle. Hence, $c = 6$.  Using the Pythagoras' Theorem, we can then see:

$$x^2+y^2=6^2=36$$

<center>
 <img class = "blog-inline-image" src="https://es-app.com/blog-assets/seekingPatternsWithMathImage4.png" alt="drawing" width="250px"/>
</center>

This might just be the extra something that we need! We now make an unexpected move that combines the given algebraic information $x + y = 8$ and the deduced Pythagorean equation: We take the square of $x + y = 8$. Let’s see:

$$(x+y)^2 = 8^2$$

$$\Rightarrow x^2+2xy+y^2=64$$

$$\Rightarrow 2xy = 64-(x^2+y^2)$$

$$\Rightarrow xy=\frac{64-(x^2+y^2)}{2}$$

$$\Rightarrow xy  = \frac{64-36}{2} = 14$$

Notice that in the second to last step, we isolate $xy$. Also, in the last step, do you see how Pythagoras' Theorem played a role in the substitution of $x^2+ y^2$? Additionally, every time we write "$\Rightarrow$", we read it as “which means that”, so it gives us a sequence of statements, each following on from the previous one.

Now that we have worked out the product of $x$ and $y$, then the area of the white triangle is just:

Area $= \frac12 xy = \frac12\cdot 14 = 7.$

**Reflection time**: What do you think was the most difficult part of our working? 

<center>
 <img class = "blog-inline-image" src="https://es-app.com/blog-assets/sunThroughClouds.png" alt="drawing" width="250px"/>
</center>

Perhaps it was the point where we decided to take the square of the equation $x + y = 8$. What on earth made us decide to do that? It was because we had insight to deduce where that mathematical process would lead us. We knew that to complete this mathematical puzzle, we needed to find $xy$. We did it by using the information given, deducing new information (the Pythagorean equation) from the geometric patterns of the puzzle, and then putting it all together in a clever way.

Here's an open-ended question: Is there only one such triangle that will match the conditions given in the problem? In other words, what are all the values of $x$ and $y$ that would still give us an area of $7$?

---

We appreciate [feedback](https://oneonepsilon.com/contact)! You may have also tried solving the problem differently. Do you have any insight from that? Did you explore your solution with your loved ones? We would love you to share your working with us.   

With a little inspiration, curiosity and persistence, people of all different math comfort levels can make their own discoveries.  In the link below, Arthur Benjamin, in his TED talk, “The Magic of Fibonacci Numbers” shares his inspiration.   

[The magic of Fibonacci numbers - Art Benjamin](https://youtu.be/SjSHVDfXHQ4)