
# Inna and Yoni Choosing Pizza
*March 11, 2017*


**Inna Lukyanenko and Yoni Nazarathy**

<center>
 <img class = "blog-inline-image" src="https://es-app.com/assets/uIld21.png" alt="drawing" width="250px"/>
</center>

**Yoni:** The other day, I met my friend Inna, a mathematician. Inna is originally from the grand city of St. Petersburg, Russia. But these days she lives between the cities of Brisbane and Melbourne in Australia. We caught up in Brisbane and enjoyed a forest walk together. We then got hungry and went to grab some pizza. Yum Yum yum

 

As we waited for the pizza to be made, I asked Inna about her relationship with mathematics and how she got into her field of mathematical physics. But Inna is sometimes a dreamer so instead of speaking about mathematical physics she started speaking about her imaginary pizzeria.

 

**Inna:** I often catch myself thinking: why on earth did I end up doing maths? Aren’t there so many other exciting careers that do not require so much mental effort? For instance, how about opening a pizza restaurant?

 

Running a pizza place can be great fun. I’ll get to make diners happy with good pizza and a nice atmosphere. I’ll enjoy chatting with my clients and staff and perhaps I may still be thinking maths from time to time. For instance, how many different kinds of pizza shall I offer?

 

As a scientist I appeal to clarity and simplicity, so instead of a usual menu, which I always find hard to choose from, I would set up a simple ordering board like this:



Then the customer can simply “tick” the ingredients he or she wants on their pizza. For example, if they are just after the usual Margherita, they would simply put:



Or, to the outrage and horror of the whole Italian nation, they might want to order an abomination of the noble idea of pizza – Hawaiian! By the way, I must confess this is my own personal favourite! In this case the board will look like this:



**Yoni:** OK Inna, it is very cute when you dream and I actually think your menu concept is a nice one. But let us ask a concrete question:

 

How many different pizzas can you create with these 6 ingredients?

**Inna:** Ahh great question! In order to compute this, let's use a binary system to indicate whether we include a certain ingredient or not. We simply put “1” if we want to include the ingredient and “0” if not.

In this case Margherita looks as follows:

And the Hawaiian:



Can we now give an answer to our question? Let’s see. For each ingredient there are 2 possibilities: either it is there or not, or, in other words, we either have “1” or “0”. Now, how many possibilities are there?

 

Here we come to an important mathematical idea: to obtain the total number of possibilities we need to take the number of possibilities for each ingredient and multiply them all together. You may ask: why multiplying?

 

To get your head around this idea let us start with a few smaller examples:

 

If we only have 2 ingredients the possible choices are:

 

00, 01, 10, 11 → 2 x 2 = 4 possibilities.

 

For 3 ingredients we end up with

 

000, 001, 010, 011, 100, 101, 110, 111 → 2 x 2 x 2 = 8 possibilities.

 

In other words, adding a new ingredient doubles the total number of possibilities. This picture of the (complete) binary tree describes just that. The first possibility allows you to go left or right ("0" or "1"). Then the next possibility allows you again to go either left or right, but you are faced with that choice twice. Once if you previously went left and once if you previously went right. The process continues for each possibility. Hence you multiply possibilities as you progress down the tree and end up with a pizza choice.


Continuing in this manner, for our 6 ingredients we need to take the 6th power of 2 and we end up with

 

2 x 2 x 2 x 2 x 2 x 2 = 2^6 = 64 possibilities.

 

Now, let us ask how many pizzas can we create with 7, 8, 9... ingredients, or moving up a level of abstraction, with N ingredients, where N can be any positive whole number. Here the logic is the same: for each ingredient we have 2 possibilities (say “0” or “1”) and multiplying these

 

2 x 2 x … x 2 (N times) = 2^N possibilities.

 

Note that this is a good example of a statement that can be easily proved by induction, which was discussed in our blog post about adding the powers of 2. I will let you ponder on this.   

Yoni: Great explanation Inna. Thank you! It is actually quite incredible how powers of 2 are so popular in simple math problems such as this. As you reminded me, our blog post with induction, also dealt with powers of 2. So did the blog post about lentils, only that there the 2 was in the denominator. In fact, the blog post about the number game also discusses log base 2 and hence the powers of 2.

 

Tell me Inna, this thing about counting possibilities, what area of mathematics does it come from?

Inna: Through this simple and tasty example, we got acquainted with an area of mathematics called combinatorics, which deals with counting things. In our case we wanted to count how many different pizzas can be created out of a certain number of ingredients, which we denoted by N. But you could also ask: how many different groups of people can you form out of a group of N people? Or, how many color combinations can we get out of N colors?

 

Or, formulating it more mathematically: how many subsets are there in a set of N elements. By a set we mean any collection of distinct objects, such as various ingredients for a pizza. Note that the possible subsets include the empty set (this is just the pizza bread with nothing on it, which doesn’t sound very exciting…) and the full set (all the ingredients included).

 

And, as we just managed to figure out, the answer to this question is 2^N, no matter what kind of objects we are considering. Now, isn’t that wonderful? So maybe next time when you go to grab a pizza with your kids you can drive their curiosity by encouraging them to think about my pizza problem!

Yoni: I enjoyed Inna's explanation very much and wanted to hear more. She explained with clarity and passion. I wasn't sure if her passion was more directed towards the mathematics or the pizza, but it didn't matter. Passion is passion.

 

Then, just as I was about to ask how many pizzas she can make with exactly 4 out of the 6 toppings... the pizza that we ordered arrived. Yum!

 


 


 

Search Tags:

combinatorics

powers of 2

