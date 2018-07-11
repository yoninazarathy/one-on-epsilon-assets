
# Averages that make sense
*July 21, 2018*


**Yoni Nazarathy**

We use the term "average" all the time. If not stated otherwise the average of a collection of values is their **arithmetic mean** taken as their sum divided by the number of values. 

However, there are different types of averages and it isn't always clear which type should be used. For this let's consider three specific cases where we may use the average value:

--

**(i) Total count calculations**: Say there are $N$ items in total and the average weight of an item is $A$. The total weight is:
$$
\mbox{weight} = N \cdot A
$$

**(ii) Return on investment calculations**: Say we invest a single dollar for a period of $N$ years. If the average growth rate per year is at a rate of $A$ then after $N$ years we have:
$$
\mbox{return} = A^N
$$

**(iii) Distance-time-speed calculations**: Say we know the distance travelled $N$ and know an average speed $A$. In this case, the time travelled is:
$$
\mbox{time} = \frac{N}{A}
$$

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
For case (i) these values represent 4 individual weights, say in kilograms. For case (ii) these values represent growth factors for each of the 4 periods. For example the value $X_1=1.05$ represents growth by $5\%$ and the value $X_2=0.85$ represents decay by $15\%$. Then for case (iii) let's assume that these values represent the speeds taken over consecuative kilometers. That is $X_1=1.05$ represents a speed of $1.05$ km/h during the first kilometer of motion, etc... these are quite slow speeds.

Now with such a meaning for these values, how would we compute the average, $A$? It turns out, that each case has an ideally suited average. Let's look at the **arithmetic mean**, the **geometric mean** and the **harmonic mean**.

**Arithmetic mean**:
$$
A=\frac{X_1+X_2+X_3+X_4}{4} = 1.15.
$$

**Geometric mean**:
$$
A=(X_1 X_2 X_3 X_4)^{1/4} = 1.1258232.
$$

**Harmonic mean**:
$$
A = \frac{4}{\frac{1}{X_1} + \frac{1}{X_2} + \frac{1}{X_3} + \frac{1}{X_4}} = 1.102277
$$

Now which of these means (averages) suites which scenario. Let's look. Plug in the arithmetic mean in case (i):
$$
\mbox{weight} = 4 \cdot \frac{X_1+X_2+X_3+X_4}{4} = X_1+X_2+X_3+X_4.
$$
Walla, the arithmetic mean seems to work for this case . That is, if the average used in case (i) is calculated using the arithmetic mean, then using it yields the desired sum of weights.

--

Now plug in the geometric mean in case (ii):
$$
\mbox{return} = A^N = \Big((X_1 X_2 X_3 X_4)^{1/4}\Big)^4 = X_1 X_2 X_3 X_4
$$
Walla, the geometric mean seems to work. That is, if the average used in case (ii) is calculated using the geometric mean, then using it yields the desired product of growth factors.

Finally plug in the harmonic mean in case (iii):
$$
\mbox{time} = \frac{4}{\frac{4}{\frac{1}{X_1} + \frac{1}{X_2} + \frac{1}{X_3} + \frac{1}{X_4}}} = \frac{1}{X_1} + \frac{1}{X_2} + \frac{1}{X_3} + \frac{1}{X_4}
$$
This is also the desired quantity. Since on each kilometer we had a different speed $X_i$ and the time for kilometer $i$ was $1/X_i$.

--


