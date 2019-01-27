The full blog post is still accessed through [here](https://www.1onepsilon.com/single-post/2018/01/28/How-Many-Times-Does-a-Number-Appear-on-the-Times-Table). We are in the process of moving it to the current location.

# Who Gets to be on the Multiplication Table?


*February 2, 2018*

**Aapeli Vuorinen and Yoni Nazarathy**

![Blog header image](https://es-app.com/assets/843nxa.jpg){.blog-image-header}

The multiplication table is a central object in the life of young mathematicians. Some find it exciting, but many others get bored of it after a while. This is perhaps understandable. Is it really so exciting to memorize the fact that 7x8=56? Perhaps 9x9=81 is slightly more exciting, but not by much. 

TABLE

But what if we were to investigate the numbers on the multiplication table like statisticians? Let's momentarily forget the mathematical structure of the table and just look at the data. This can even be done with young children.

 

Excel Fun:

 

List all the numbers 1,...,100. Then for each number, count the number of times it occurs in the table.  For example, The number 12 occurs 4 times. The number 100 occurs only 1 time. The number 13 doesn't occur at all.

 

One way in which you can do this is create a column in Excel of the numbers 1,...,100. Then in a column next to it, fill in the occurrences manually.  Show the multiplication table to a youngster and ask them to count how many 1's, how many 2's, how many 3's etc... Sit together next to the computer and fill it out together - believe it or not - kids think Excel is fun.

IMAGE

Plotting the count of occurrences for each of the numbers, you may generate a graph similar to this:

HISTOGRAM

As you see, all numbers between 1 and 100 occur either 0, 1, 2, 3 or 4 times. For example the number 80 occurs twice via 10x8 and 8x10.  The number 81 occurs only once via 9x9. The Number 17 doesn't occur at all, and so forth.

 

Time for some insights:

 

There are 58 numbers that don't appear at all. Hence only 42 numbers appear. You can then carry out some inquisitive investigations: What is the smallest number that doesn't appear? What is the smallest even number that doesn't appear? Can a prime number appear on the multiplication table? How about a prime number greater than 10; can such a number appear?

 

There are 6 numbers that appear only once. For example 25, 81 and 100. What are the others?

 

There are 23 numbers that appear twice. Why is appearing twice so popular?

 

There are only 4 numbers that appear three times. For example, 9. What are the others?

 

There are 9 numbers that appear 4 times. What are those numbers? What makes them special?  Does any number appear more than 4 times?

 

Here is a graph showing how many numbers occur 0, 1, 2, 3 or 4 times:

HISTOGRAM

Beyond the 10 Table: 

 

But what if we didn't restrict our analysis to a multiplication table of size 10 by 10? For example, what if we considered the 11 by 11 table, the 12 by 12 table or even the 100 by 100 table? Can there be a number that appears more than 4 times on these bigger tables? Try for example the 12 times table, you'll see that there is a single number that appears 5 times and two numbers that appear 6 times. What are they?

 

And what if we were to venture to really big multiplication tables? Watch this little animation illustrating multiplication tables going from size 1 up to size 400. Each spot on the table is a pixel that is shaded based on how often the number appears on the table. Numbers that appear frequently are light blue and numbers that are rare are darker. Watch it a few times and ponder about some of the patterns that emerge. You can also pause the animation near the start to see the 10 by 10 table and make sense of the colors.

VIDEO

We enjoyed making this animation. Then after we watched it a few times, we were struck by this question:

 

What proportion of the numbers 1,...,n² appear on the n by n table?

 

That is, for the 10 by 10 table, 42 out of the 100 possible numbers appear, hence the proportion is 0.42. However, what happens to this proportion for bigger multiplication tables? What happens to this proportion as the size of the multiplication table grows? 

 

For example, considering tables of increasing sizes (up to 400 by 400) and counting how many numbers appear on the table, we see that the proportion behaves as the graph below.

GRAPH

For reference, the right most point of the graph corresponds to the multiplication table based on multiplying the numbers 1,...,400. This table has 160,000 numbers in it. A computer program then shows that only 41,872 of these numbers appear on the table. Hence the proportion of numbers on the table is 0.2617; about a fourth. 

 

We don't have answers to everything: 

 

So what if we look at bigger and bigger tables? Would the proportion of numbers that appear flatten out at some quantity or would it get closer and closer to zero? We are actually not sure about the answer. 

 

Our curiosity drove us to compute values of up to n=20,000. With this we reached the proportion 0.219846. However, based on such numerical investigation, we can't determine if the proportion will go to 0 as n grows, will reach some other limit, or perhaps behave in a more erratic manner.

 

Still, the numerical experimentation was fun and thought provoking. Now we are left with an unanswered problem. There is fun in that too.

---

Follow up (Updated a week later): After searching the Online Encylopedia of Integer Sequences we found out that the problem discussed above is known and solved. You can read more about it in this post.

 

 
