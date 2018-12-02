# 11, 15, 21, 30 or 36 possible outcomes?

*November 16, 2018*

**Yoni Nazarathy**

<center>
 <img class = "blog-inline-image" src="https://es-app.com/assets/44dice.jpg" alt="drawing" width="250px"/>
</center> 

Imagine that you have a pair of [dice](https://epsilonstream.com/topic/dice). That is, number cubes with the numbers $1, 2, 3, 4, 5$ and $6$ on each side. You are using these as part of a game, tossing the pair again and again. Then at one point you stop and ask:

**How many possible outcomes are there in a toss of 2 dice?**

 

So here is the catch: 

**There is not only one answer to this question, because it is not well defined.**

 
Valid answers include: $11, 15, 21, 30$ and $36$, and each of these quantities has its own specific story.

For example, $11$ is the number of possible sums that you can get. This is important, for example, in playing Monopoly, you toss and move your piece based on the sum. It can be $1 + 1 = 2$ at the minimum or $6 + 6 = 12$ at the maximum. Hence $2, 3, 4, 5,\ldots ,11, 12$ are outcomes, and there are $11$ possible outcomes. So we see that $11$ is the answer to the well defined question, "*How many possible outcomes are there for the sum of the dice*?"

OK, so we got $11$ out of the way. But how about $15, 21, 30$ and $36$? Where are these numbers from? Can you describe a question and/or a dice tossing scenario to which the answer is $15, 21, 30$ or $36$? How do you compute these values? Which answer is "most natural"? Pause and think about it before you read on...

<center>
 <img src="https://es-app.com/blog-assets/dicem3.jpg" alt="drawing" style="max-width:60%;" />
</center>

**The answer 36:** Ok, so if the dice are distinctly coloured then 36 is the number of possible outcomes.


There are 6 possible outcomes for the first colour and 6 possible outcomes for the other colour. Each pair of the form $(x, y)$ where $x$ and $y$ are values in the range $1, 2,..., 6$ is valid. There are $6 \times 6 = 36$ such pairs. 

---

**The answer 30:** Assume now that the dice are still distinctly coloured and you don't accept "doubles". That is, if you get the same result on both dice you say, "nah... gotta toss again." In this case there are 6 less options because the pairs $(1, 1), (2, 2), ..., (6, 6)$ are out of the picture. Hence 36 - 6 = 30. Another way to get 30 is to see that there are 6 options for the first toss and then once this is determined you are only left with 5 options for the second toss, so $6 \times 5 = 30$.

---

**The answer 15:** So what if we consider the case above where two outcomes of the same number are still not allowed but the dice have the same colour and are indistinguishable? 

In this case, you may write out all the possibilities and count that there are 15. These would be

<center>
$
\begin{array}{c}
\{1, 2\}, \{1, 3\}, \{1, 4\}, \{1, 5\}, \{1, 6\},\\
\{2, 3\}, \{2, 4\}, \{2, 5\}, \{2, 6\},\\
\{3, 4\}, \{3, 5\}, \{3, 6\},\\
\{4, 5\}, \{4, 6\},\\
\{5, 6\}. \\
\end{array}
$
</center>
 
Yes, you can count, but you can also think of it this way: Consider the case of 30 above where, for example, the pair $(3, 5)$ and the pair $(5, 3)$ came from different outcomes. The former came from a 3 for the green and 5 for the yellow and the latter came for 5 for the yellow and 3 for the green. Now in the current case where both dice have the same colour we cannot distinguish between $(3, 5)$ and $(5, 3)$. Instead we just denote this outcome by $\{3, 5\}$ agreeing that the curly braces imply that order doesn't matter. Then for every two outcomes in the former case there is a single outcome in the latter case and that is why we divide 30 by 2 to get 15.

---

**The answer 21:** In many ways, I believe that this is the "best" answer to the question posed at the start of this blog post. That is, if you don't specify anything else and ask me: "How many possible outcomes are there in a toss of 2 dice?" then I will say 21! This is the case where the dice are indistinguishable (e.g. both red) just like in the case above. Further, there isn't any problem with getting a "double". Hence take the count of the previous case and add the 6 additional possibilities:

<center>
$
\{1, 1\}, \{2, 2\}, \{3, 3\},
\{4, 4\}, \{5, 5\}, \{6, 6\}.
$
</center>

Then $15 + 6 = 21$ and there are $21$ possible outcomes. 

<center>
 <img src="https://es-app.com/assets/cn3zh2.jpg" alt="drawing" style="max-width:60%;" />
</center>


---

**Wrapping up:** The cases $15, 21, 30$ and $36$ are special cases of an interesting general setup often studied in basic combinatorics. What if you had k dice each with n sides? In the discussion up to now we had $k = 2$ and $n = 6$, however in general you can allow k and n to be any positive integers.

Exploration of these types of problems is very rewarding. If you are looking for partners for such investigations, consider checking out The Pascal's Triangle Facebook group. On that page, dozens of enthusiasts and experts continue to post cool attributes associated with Pascal's triangle and binomial coefficients.  

The cool thing is that the basics can be explored as we did in this post without any formulas. Then by using involved formulas and arguments, glorious patterns emerge. You can also watch this great TED-ED video by Wajdi Mohamed Ratemi. Let us know what you think.

<a href="https://epsilonstream.com/video/tvpxhi/">
	<center>
 		<img class = "blog-inline-image" src="https://i.ytimg.com/vi/XMriWTvPXHI/mqdefault.jpg" alt="drawing" width="250px"/>
	</center> 
</a>