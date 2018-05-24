
# Are There More Evens Than Odds?
*March 4, 2017*


*Yoni Nazarathy**


 

Before you rush to answer, please consider my claim: Asking this question is just as important as answering. Indeed, a central goal of many of our blog posts is to empower parents and educators with basic ideas and knowledge for guiding children through mathematical exploration.

 

A simple question such as this one, can do just that. Serve it to your children with the right tone at the right time, and watch them embark on a discovery process. Come armed with just a bit of knowledge beforehand, and you'll be a tool at their side, helping them feed their curiosity.

 

In preparation for this blog post, I asked my children:

"Are there more even numbers than odd numbers?

Or is it the other way around?"

The question resulted in a fascinating discussion between my daughters where one claimed "there is one more even number since the evens start at 0 and the odds start at 1", but the other claimed that "numbers never stop". She continued her thought process and concluded that "-4, -2 and other negative numbers are also even". So maybe "numbers never start". After some discussion, both of my daughters jointly agreed that there is the same amount of evens and odds. An infinite amount. For every even you can find an odd and for every odd you can find an even. 

 

Even though it was only a five minute discussion, I think that the concepts that they pondered about will stay with them for a lifetime.

 

Some of you may know that set theory can go further in answering such a question, but we won't do that today. We'll leave it to another day, to explore concepts dealing with the size of infinite sets. Instead, let's play a bit with evens and odds to discover useful and basic properties.

To do this, let’s get back to the Fibonacci sequence, touched upon in last week’s blog post. This is a fun sequence of numbers to compute. You start with a value of 1 for the first two numbers. Then each additional number is the sum of the previous two. It goes like this:

 

1, 1, 2, 3, 5, 8, 13, 21, 34, 55, 89, 144, 233, 377, 610,…

 

For example 13, the seventh number in the sequence, is the sum of it’s predecessors:  5 + 8 = 13.

 

The first 20 or so elements of Fibonacci can be fun to compute for kids. But now let's look at something else. Which numbers in the sequence are even and which are odd? Here is how it looks:

 

O, O, E, O, O, E, O, O, E, O, O, E, O, O, E, O, O, E, O, O, E,…..

 

Do you see a pattern? Sure you do. Every third number appears to be even while the rest appear to be odd. Why is that?

Before we investigate the Fibonacci "ooeooe" phenomenon, let's explore an additional sequence. The sequence of perfect squares. 

 

0, 1, 4, 9, 16, 25, 36, 49, 64, 81, 100, 121, 144, 169,...

 

How is this sequence looking in terms of evens and odds?

 

E, O, E, O, E, O, E, O, E, O, E, O, E, O,...

 

There is a simple pattern here also. What is happening?

The Fibonacci sequence thrives on addition and the sequence of perfect squares thrives on multiplication. So lets explore addition and multiplication of whole numbers, and see what happens to evens and odds in the process.

 

A year ago I asked one of my daughters (she was seven at the time) about the sum of two odd numbers. Is it “always even”, “always odd” or “it depends”. She tried a few numbers: 5 + 7,  19 + 3,  101 + 21. Following her experimentation she concluded "always even"! 

 

But I pushed a bit more and asked, "are you sure? why?". I sometimes ask my kids such questions at the wrong time and get ignored at best. But here I grabbed my precious little explorer just at the right moment. She was curious and enjoyed the discovery process. She thought a bit more and concluded:

 

“Well, every odd is an even number plus one. Now add two odds and you’ll be adding the two even parts; and then adding plus one twice.”

 

She already knew that adding up evens keeps us in the set of evens. It is like skipping by twos. So she concluded: 

 

“Odd + Odd = Even. Always!”

 

Clearly I was proud of my little sweetie’s proof. Through such a process, she discovered herself that:

 

Odd + Odd = Even,

Even + Even = Even,

Even + Odd  = Odd.

 

Given these rules, do you see what is happening with Fibonacci? 

 

The first two numbers are odd and hence the third number is even. Then the next number (4th) is Odd + Even = Odd. Similarly for the one that follows (5th). But then the situation repeats for the sixth number. Since the previous two were odd, the sixth number is even. This process then continues forever. 


Now let's move to the perfect squares. The square of a number is the number multiplied by itself, so we should think about multiplication. Let's consider first Even x Even? In this case it is quite clear that Even x Even = Even.

 

After all, multiplication is addition of (say) the first even, an even (second even) number of times.

 

How about Even x Odd? Even though this type of multiplication doesn't happen in the case of the sequence of perfect squares, it won't hurt to give it some thought. 

 

Well here, we can think of the multiplication as addition of the even number, an odd number of times. Since we are adding evens, the result remains even. 

 

So we discovered so far that,

 

Even x Even = Even,

Even x Odd  = Even.

 

To complete the picture in the perfect squares, we are missing 1, 9, 25, 49, 81, 121,...

 

Through some experimentation, you can see that Odd x Odd  appears to be odd always. I believe that if you think about it a bit yourself, you'll find the proof for this. But let's see a way to do it using some algebra.

 

You see, every even number can always be written as 2 x K where K is some whole number. Similarly, every odd number can be written as 2 x K + 1 where K is some whole number.

 

What is K for 17? K = 8. 

 

What is K for 26? K = 13.

 

What is K for -2? K = -1.

 

What is K for -7? K = -4.

 

What is K for 1001? K = 500.

 

Let's call this K, the building block of the number (this isn't a generally accepted mathematical term, but let's use it here).

 

So now say we are multiplying two odd numbers. We are then multiplying

 

(2 x K+1) x (2 x L+1),

 

where K  and L are the building blocks of the two odd numbers. Now with basic algebra (and omitting the "x" symbol) we have:

 

(2K + 1)(2L + 1) = 4KL + 2K + 2L + 1 = 2(2KL + K + L) + 1.

 

So if we treat M = 2KL + K + L as a building block, we see that the product is again an odd number. Cool, no? We proved that, 

 

Odd x Odd = Odd.

 

This type of algebra can be used to derive all of the even and on properties that we saw. Maybe explore it together with your loved ones.

 

 

Search Tags:

Algebra

Numbers