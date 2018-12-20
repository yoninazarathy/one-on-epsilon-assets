# Powers of 2 and your family tree

*Dec 22, 2018*

**Phillip Isaac**

![People standing on the horizon](https://es-app.com/assets/tree87.jpg){.blog-image-header}

My 9-year old daughter occasionally enjoys calculating the powers of 2. Starting with 1, she will happily sit there working out the powers of 2 until they are surprisingly large numbers. Recently I had a curious conversation with her related to her calculations that I thought I would share in this blog post.

Dad: How many parents do you have?

Daughter: You know that! I have 2 parents!

Dad: How many grandparents do you have?

Daughter: 4

Dad: How many great-grandparents?

Daughter: 8.

Dad: How many great-great-grandparents?

Daughter: 16… wait, these are powers of 2.

Dad: What if you kept going with this? 

Daughter: How far back in time can you go?

Okay, so it was at this point that we had to lay a few ground rules. What we were actually doing was starting to create a mathematical model describing the number of new ancestors in history, given a particular year. To progress, one of the key assumptions that we decided to make was that a new generation occurs every 30 years. Is this reasonable? Well, it is something we could change later if we wanted.

In any case, under this simple assumption, we can produce the following table, that gives the number of new ancestors (right hand column) that were born around that year (left hand column). Note that the only reason I started at 2009 was because this was the year my daughter was born. The table conveys the information that 1 new generation member was born around 2009, and 2 direct ancestors in the previous generation were born around 1979, 4 direct ancestors in the previous generation were born around 1949, and so on. Note that the total number of ancestors would be the sum of powers of 2. This has already been discussed in a previous blog post:

[![](https://es-app.com/assets/vmK21a.png){.blog-image-inline-small}](https://www.1onepsilon.com/single-post/2017/02/17/Adding-the-Powers-of-2)


|      |                |
|------|----------------|
| 2009 | 1              |
| 1979 | 2              |
| 1949 | 4              |
| 1919 | 8              |
| 1889 | 16             |
| 1859 | 32             |
| 1829 | 64             |
| 1799 | 128            |
| 1769 | 256            |
| 1739 | 512            |
| 1709 | 1,024          |
| 1679 | 2,048          |
| 1649 | 4,096          |
| 1619 | 8,192          |
| 1589 | 16,384         |
| 1559 | 32,768         |
| 1529 | 65,536         |
| 1499 | 131,072        |
| 1469 | 262,144        |
| 1439 | 524,288        |
| 1409 | 1,048,576      |
| 1379 | 2,097,152      |
| 1349 | 4,194,304      |
| 1319 | 8,388,608      |
| 1289 | 16,777,216     |
| 1259 | 33,554,432     |
| 1229 | 67,108,864     |
| 1199 | 134,217,728    |
| 1169 | 268,435,456    |
| 1139 | 536,870,912    |
| 1109 | 1,073,741,824  |
| 1079 | 2,147,483,648  |
| 1049 | 4,294,967,296  |
| 1019 | 8,589,934,592  |
|  989 | 17,179,869,184 |

This is where it gets interesting. The data in the table suggest that around the year 1799, there were 128 distinct individuals whose existence contributed to my daughter’s life. That’s not inconceivable, but it can be easy to become lost in the quagmire of large numbers. Indeed, the real surprise starts to manifest when we go further back in time to, say, the year 1019. Our simple model indicates that over 8 billion individuals must have been born around that year who were direct ancestors of my daughter. According to [world population estimates](https://en.wikipedia.org/wiki/World_population_estimates) from the U.N., around the year 1000, the population was around 310,000,000 (310 million). So our data says that around that year, the number of my daughter’s ancestors born numbered somewhere between 8,000,000,000 (8 billion) and 17,000,000,000 (17 billion)! That is more than the world’s population! Something must be wrong with the model. The Battle of Hastings (year 1066) was certainly not just an argument among my family! What could we have missed?

After a bit of thought, you might have guessed that one of our key assumptions in the model may not be valid. Indeed, the assumption that the ancestors in a particular generation are all distinct individuals is plainly false. In other words, it must be the case that some of our ancestors were having children with their own extended family! In fact, this is discussed by Michaels Stevens on the VSauce YouTube Channel in the video entitled “We Are All Related”:

<iframe width="350" height="196" src="https://www.youtube.com/embed/BhtgINeaJWg" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

Could we modify our model to take this into account? Yes, but it can become extremely complicated very quickly. There are many possibilities to consider, and even the simplest modification may not be straightforward to implement. For instance, one ancestor may have had children to multiple partners. Or, one ancestor may have had children with their fourth cousin twice removed. (For a discussion on cousins, first cousins, second cousins, once/twice removed and so on, see this article by Livescience: [What's a Second Cousin vs. a First Cousin Once-Removed?](https://www.livescience.com/32121-whats-a-second-cousin-vs-a-first-cousin-once-removed.html) ).

As an example, try to think about how to adapt the model if we say that every second generation in the family tree has exactly one set of grandparents who were first cousins. That is, to assume that in the family tree of a current person, one set of grandparents were first cousins, and one grandparent has grandparents who were first cousins, and so on. It is not easy! You would end up with a sequence like this: 1, 2, 4, 8, 14, 28, 54, 108, 214, 428, 854,... That is, from the number "4" in the sequence, you apply the following rule: Multiply by 2 every step, but every second step you also subtract 2. Try to work this out for yourself. Is it possible to represent this in a concise mathematical way? Well, here is one way to summarise this sequence. Set $a_1=1$, $a_2=2$, $a_3=4$, and then apply the formula
$$
a_{n+1} = a_n - 4\left( \frac{n+1}{2} - \left\lfloor\frac{n+1}{2}\right\rfloor \right), \ \ n=3,4,\ldots
$$
Here, $\lfloor x \rfloor$ denotes the "[floor function](https://epsilonstream.com/topic/floorFunction)", or the "integer
part", of $x$ (in other words, we just round down $x$ to the nearest whole
number). Implementing this modification in the data used above, going back to the year 1019 would give the number 7,158,278,828. More than one billion less than the original model, but still far too high to be realistic. The art is to now introduce further modifications to approach some kind of realism. Without explicit data, though, this is not really feasible. Maybe you can try some othere variants and see if you can come up with mathematical formulae that take into account your new assumptions.

I have a brother who is keenly interested in our family tree, although he refers to it as the family briar patch. There is no denying that our family histories can be quite complex. Next time you pass by a stranger in the street, perhaps now you cannot help but wonder how distantly you might be related. 
