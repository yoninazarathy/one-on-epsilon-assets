# Is it Divisible by 3?
*January 15, 2017*


**Yoni Nazarathy**

![Blog header image](https://es-app.com/assets/7fnxAN.png){.blog-image-header}

I am the father of three kids, hence for me division by three is an integral part of life. A pack of $12$ water balloons is [divisible by three](https://epsilonstream.com/topic/divisibility3). A pack of $30$ works well too. But get a pack of $16$ and you are left with a remainder of $1$ and a philosophical debate about who deserves it.
	
For parents with $2$ kids, things are typically simpler. [Even numbers](https://epsilonstream.com/topic/evenNumbers) are divisible by $2$ and [odd numbers](https://epsilonstream.com/topic/oddnumber) are not. But if you are into $3$'s, how to know if a whole number is divisible by $3$? Is there some simple rule or pattern?

Well, there is a good chance that your child has been taught this at school. Maybe you even remember this “trick” back from the days. It goes as follows: 

**Add up the individual digits of the number and see if the sum of the digits is divisible by three. If the sum of the digits is divisible by 3 then so is the original number. Otherwise, it isn’t.**

The trick also works similarly for $9$, but we’ll focus on $3$ here. Nine kids with water balloons - too much to handle!

---

Here is an example: Take $264$. The sum of the digits is $2+6+4 = 12$. Now $12$ is divisible by $3$ and this implies that $264$ is divisible by $3$. In fact, $264 = 88 \times 3$. 

Similarly, take $301$. The sum of the digits is $3+0+1 = 4$. This is not divisible by $3$ and hence neither is $301$. Try to divide it by $3$ and you’ll get a non-whole number or a remainder.

Well, that’s the trick. You can even use it recursively if you really wish. For example, on the noon of January 15, 2017 (Beijing time) the population of China was estimated to be at $1,382,765,241$ (almost $1.4$ billion people). Is this exact number divisible by $3$? Well the sum of the digits is,

$$1+3+8+2+7+6+5+2+4+1 = 39$$

And this translates the question to: “is $39$ divisible by $3$”? Well, you probably see immediately that yes, but to answer this you can also look at $3+9=12$. And then to see if $12$ is divisible by $3$, you can even look at $1+2=3$ and yes it is. Hence since $3$ is divisible by $3$, $12$ is divisible by $3$ and hence $39$ is divisible by $3$ and hence the population of china (estimate of that exact time) is divisible by $3$. This recursion is more of an academic exercise, because you already saw that $39=3 \times 13$ is divisible by $3$.

Ok, so that was the “trick”, a “math trick”. But frankly, us mathematicians are often weary of using the word trick because we like to understand the deeper meaning behind things. In fact, we would often like to see a proof that this trick actually works for any number. Sure, we can check it on the number $264$, the number $301$ and the population of China, but how to know that it always works?

---
 
So here is a simple explanation: Look at the number $264$ as an example.

$$264 = 2\times 100 + 6 \times 10 + 4$$

Right? This is what we mean when we write the number $264$ (in base $10$ as we usually do). This can also be done for the population of China, where the leading term would be, $1\times 10^9$ (that reads as "10 to the power 9" i.e. a billion), the second term is $3 \times 10^8$, the third term is $8 \times 10^7$ and so fourth. 

Going back to the $264$ example, we can now represent $100$ as $99+1$ and $10$ as $9+1$ hence,

$$264 = 2\times (99+1) + 6\times (9+1) + 4$$

Now comes the fact that $2\times (99+1) = 2\times 99 + 2\times 1$. This is called the [distributive property](https://epsilonstream.com/topic/distributiveProperty). That is,

$$A\times(B+C) = A\times B + A\times C$$

where we notice that the order of operations is to first perform $$A\times B$ and $A\times C$ and only later to do the plus between these terms. Hence,

$$264 = 2\times 99 + 2 + 6\times 9 + 6 + 4$$

We can now reorder this to,

$$264 = 2\times 99 + 6\times 9 + (2+6+4)$$

Now observe that the last bit above, $(2+6+4)$, is actually the sum of the digits, hence we got,

$$264 = 2\times 99 + 6\times 9 + \text{sum of digits}$$

The terms, $2 \times 99$  and $6 \times 9$ are always divisible by $3$,  because $99$ and $9$ are always divisible by $3$. Now assume that the sum of the digits is divisible by $3$ (as it is in the case of $2+6+4$). Then all terms on the right hand side are divisible by $3$ and then $264$ is divisible by $3$. That is why the rule worked for $264$.

---

### Let’s try it on the number $2324$:

$$
\begin{align}
2324 &= 2\times (999+1) + 3\times (99+1) + 2\times (9+1) + 4 \\
&= 2 \times 999 + 3\times 99 + 2 \times 9 + \text{sum of digits}\\
\end{align}
$$
 
Now the sum of the digits is $2+3+2+4 = 11$ and is not divisible by $3$. But the first bit, $2 \times 999 + 3 \times 99 + 2 \times 9$ is divisible by $3$. So this means that,

$$2324 =  \text{something divisible by 3} + \text{something not divisible by 3}$$

Hence, $2324$ is not divisible by $3$.

---

So we now see the basis for the [divisibility by $3$ rule](https://epsilonstream.com/topic/divisibility3). While there is a very good chance that your kids are taught the rule, are they taught why it works? You can now explore it with them.
