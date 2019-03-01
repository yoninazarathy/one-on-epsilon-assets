The full blog post is still accessed through [here](https://www.1onepsilon.com/single-post/2017/05/21/Thinking-Optimization). We are in the process of moving it to the current location.

# Thinking Optimization

*May 21, 2017*

**Yoni Nazarathy**

![Blog header image](https://es-app.com/assets/df28ND.jpg){.blog-image-header}

Depending on your favorite strand of English you may write 'optimise' or 'optimize'.  But don't worry about the spelling, instead think about how often you use this word? What does 'optimization' mean for you? Here is one definition: "make the best or most effective use of a situation or resource”. Is this how you think about optimization? Actually, when was the last time that you optimized?

 

Maybe it was when you were driving around your familiar neighbourhood, dropping off and picking up children from friends and activities. You might have been planning the optimal route. What does that mean?

 

Or if you are a farmer, maybe you tried to optimize the number of tomatoes that grow on your patch by using just the right amount of fertilizer. If you add too much you kill the crop, but if you don't add enough then the yield is low.

 

What if you are an athlete, running a long distance as fast as possible. Or perhaps you are swinging a baseball bat at just the right angle, aiming for a home run. In that case you probably optimize all the time. Don't you?

 

In all of the above examples, you make some choice, a sequence of choices or an action. These actions then influence the outcomes. You try to do the best choice so as to maximize or minimize some objective. You may try to maximize profit or yield, minimize time or effort, maximize enjoyment, minimize pain, maximize the chance of getting the right prediction, minimize the number of attempts at taking a shot,... the list goes on and on.

---

Is this how you think about optimization? Maybe sometimes?

There is a slightly different view as well: Say you are a software engineer. In this case, you probably use the word optimization for describing the process of improving your product. For example as you start creating it, your computer program or application may run in a slow and inefficient manner. This means that the user has to wait for output or maybe the program uses a lot of battery power and network resources.

As you improve your app, you use creative means to make it more efficient. It will then run faster, use less battery power, less network resources and perhaps be more responsive to user input. In such a process, there isn't necessarily a well defined numerical objective. Nevertheless, it is called 'optimization' and the act of making incremental improvements to your product is called `optimizing'.

IMAGE

But let us focus on optimization where there is a clear quantity you want to improve. Something you can measure. Time, distance, monetary expenses, weight, profit, score, fuel consumption or in general, a number that you either call `value' if you are trying to maximize, or 'cost' if you are trying to minimize. Think of some more examples from your day to day life. Now ask - how does mathematics fit in?

---

Before we explore a simple and concise mathematical way of grasping optimization, let's see a few more examples. You see, optimization is not necessarily operational. By this I mean that when you carry out optimization, the result doesn't always influence your choice, action or behaviour. For example at your current geographical location, how long is the longest day of the year and what is that day? How about the shortest day?

 

This is clearly not operational. No one has yet been able to influence the length of days. Luckily, the spin of the earth and our movement around the sun are beyond our control. Nevertheless, as an optimization question, it is very legitimate: When is the longest day?

 

Answer: If you are in the northern hemisphere then it is at the June solstice, and for us on the south side, it occurs at the December solstice. The actual length of that day depends on the exact location on the globe.

Or here is another example. Say you are playing Monopoly. On each turn you toss a pair of 6 sided dice and add up their numbers to see how many steps your player needs to move. What is the most likely number of steps?  

Answer: 7. You can get an intuition for this by seeing that getting a sum (number of steps) such as 2 or 12 can occur only with a specific result (1 + 1 for 2 and 6 + 6 for 12). That is, getting either 2 or 12 isn't likely. But getting 7 can occur in more ways: 1 + 6, 2 + 5, 3 + 4, 4 + 3, 5 + 2, and 6 + 1. So it is more likely and if you think about it a bit more, you'll see it is the most likely outcome. 

IMAGE

As another example, say you have a 1 meter long string. What shape can you create so as to maximize area? 

 

Can you visualise this? Maybe grab some string, or draw a few shapes. Notice that all shapes will have a perimeter (called circumference when the shape is curved) of 1. But the area of the shape will vary.

Hint: The maximal area is 1/(4 pi). What shape with a perimeter (circumference) of 1 has such an area? You can probably take a guess.

---

So you see, sometimes optimization is a means for deciding what to operationally do as in the navigation, farming and sporting examples. At other times, optimization is just about answering a maximization or minimization problem. This is a subtle distinction, but it just comes to show that there are different ways for thinking about optimization.

 

It is sort of like the difference of asking:

"Where is the highest point in Ireland?"

as opposed to,

"Where should I go in Ireland to be highest?".

In both cases the answer is Carranutoohil, a peak at 1,038 meters above sea level (3,406 ft). I have never climbed it. But cycling near it, in the Ring of Kerry, was an incredible experience. Believe me, Ireland is mystically beautiful.

IMAGE

---

So how can we view optimization mathematically?  

The common way to do this is to think in terms of a function. As an example, consider last week's blog post dealing with triangles.  In that context, we encountered,

FORMULA

Such a mathematical expression may look intimidating, but don't fret over it. It is a function of the variable x. The function is called "f". When you give the function a value of x, you get in return f(x). Take for example x = 0. This means to replace x by 0, everywhere in the equation above. Keeping in mind that the square root of 1 is 1, we get f(0) = 0. Can you see this? 

Or as we showed in last week's blog post, if x = 1 then y = 0.295 (approximately). And this is actually the maximum of the function. Here is a plot of the values of f(x) for x in the interval [0,10].

IMAGE - GRAPH

So in general, what is a function?

A function is a machine that transforms an input x to an output y.

This can be written as

FORMULA

But where do functions appear in the many optimization examples discussed above?

---

When considering general optimization problems we let x be in a domain of values that isn't necessarily composed of numbers. For example, x can be a route you take in your neighbourhood, a trajectory of a baseball bat, a shape made by a string of length 1 or a location in Ireland. The domain, exactly specifies that set of allowed values and depends on the problem at hand.

 

Consider for example my children's cats: "Booboo", "Lily", "Grey". Say we are interested in the (simple) optimization problem of finding the heaviest cat. For this, let f(x) be the function that takes x as the cat and specifies the cat's weight in kilograms. In this case the domain is 

FORMULA

What would then be the function? Is there a formula for it? No, in this case we don't have a formula for the function. We rather write a table:

TABLE

In fact, you can always view a function as a table. Note though, that when the domain is infinite, you need a very long table, an infinite table. Keep in mind, that having a formula is a luxury, it is actually an exception as opposed to the rule.

 

How about the output value y? Can it also be anything or does it need to be numerical? Well, here, since we are using functions for optimization, we want to be considering real functions. This is a function that has a real number as an output. After all, when you optimize, you treat the output as 'value' or a 'cost'. In a fancy mathematical way you can introduce a function like this: 

FORMULA

Here the curly looking D, is the domain of the function. Then the impressive looking R is the set of all real numbers. This is called the range of the function. So real functions are functions whose range is the set of real numbers. 

 

Wow! Fancy notation. How would you then describe an optimization problem? Say a maximization problem? Well just write,

FORMULA

This mathematical notation states that y* is the maximal value obtained by the function over the whole domain. It implies to "try" f(x) for every x in D and choose the maximal value.  In the case of my children's cats we have y* = 4.1.

Then there is also,

FORMULA

This means that x* is the point that maximizes the function. In the case of my children's cat's we have, x* = "Lily". In the case of the Ireland example we have x* = "Carranutoohil". 

So basically, when you come to a mathematical optimization problem, all you need, is f(x), a domain D, and then just search for x* and y*. However, you should keep in mind that for some problems, y* doesn't always exist and/or x* is not always unique.

---

So wow! With three simple formulas, optimization looks so simple and compact. Is it? Well, often finding a useful representation of the function f(x) is a hard mathematical modelling challenge. In operational problems, you want f(x) to describe reality well. This isn't always easy.

Further, even if a problem is represented correctly, understanding that there exists a y* and/or a unique x* can be a mathematical challenge. Finally, and most importantly, finding efficient ways for computing the pair (x*,y*) is a real challenge. In fact, some problems are known to be computational nightmares. Have you heard of the travelling salesman problem, for example? Let's keep that for another day.