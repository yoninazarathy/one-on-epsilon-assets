
# Adding the Powers of 2
*February 17, 2017*


**Yoni Nazarathy**


Have a look at this equation:

 

1 + 2 + 4 + 8 + 16 = 32 - 1.

 

What does it describe?

 

Here is one possibility: Say you embark on a 5 day trip, planning to take photos on the way. On the first day you only shoot one photo. Then on each new day you shoot twice the number of photos that you shot on the previous day. Hence with a 5 day trip you shoot 1+2+4+8+16 = 31 photos in total. This is already a nice collection of photos to share with your friends.

 

But then you ponder:

 

If I extend the trip by one more day,
how will that affect the size of my photo collection?

 

Q: How many photos will you get from an additional day?

A: Since in our story, the number of photos you shoot doubles every day, you'll get 2 x 16 = 32 new photos. 

 

Q: How many photos will you have in total?

A: Previously you had 31, now with 32 more photos: 31 + 32 = 63 in total.

 

You just discovered that extending by one day makes the total number of photos grow by a bit more than 100%. It doubled plus one more! An additional day was really useful for your photo collection. Wasn't it?


Is this property specific to the case of a 5 day trip? Or does it hold for any number of days? To answer this, look for example at the equation 

 

1 + 2 + 4 = 8 - 1.

 

This corresponds to a 3 day trip, yielding 7 photos in total. A fourth day would yield 8 additional photos. Your collection would now be of size 7 + 8 = 15.

 

As another example, look at this equation:

 

1 + 2 + 4 + 8 + 16 + 32 + 64 + 128 + 256 = 512 -1.

 

This one corresponds to a 9 day trip where you shoot 511 photos in total. An additional (tenth) day would then yield 512 additional photos. Your collection would now be of size 511 + 512 = 1023.

 

It certanly seems like there is a pattern here. It can be roughly summarised as follows:

 

The sum of the first powers of two is one less than the next power of two.

Powers of two are very common in life and especially in computers and technology. For example, computer memory sizes are often 1, 2, 4, 8, 16, 32, 64, 128, 256, 512... Gigabytes. To referesh your memory about power, consider 2 to the power 5 (this equals 32):

 


Note also that any number to the power 0 is defined to equal 1 and any number to the power 1 is just itself. In the case of 2, 


 

Q: So using powers of 2, how do we describe the blue equations above? 

A: Here is one way to write it:


 

For N = 0 the equation is just

 

1 = 2 - 1,

 

for N = 1 the equation is 

 

1 + 2 = 4 - 1,

 

and for N = 2 the equation is

 

1 + 2 + 4 = 8 - 1.

 

Note that to match the photography story, N denotes the number of nights in our trip (1 less than the number of days). But this isn't a critical detail.

We saw that our discovery works for a few specific cases of N. But how do we know it holds for all N? You can suggest that we just trust our instinct and believe that the rule works. However, in mathematics we can often do better. We can prove that our statement holds for all N.

 

One way to prove it is by starting with N=0. In that case since 1 = 2 - 1, we immediately see that the statement holds. We can then "grow out the truth" by showing that if it holds for N then it also holds for N+1. This logical process is called induction.

 

Many teenagers find induction confusing when they see it first. Reflecting back on my late teenage-hood, I remember associating induction with suffering and confusion. I never really understood it back then and it made me feel stupid. Combine induction with a bit of algebraic immaturity, lack of focus and raging hormones and you'll end up with a frustrated teenager. So educators and parents - please keep this in mind and be gentle when it comes to teenagers+induction.

 

Having said all that - let's do some induction! 

 


 

In our case, the trick is to look at one equation in the sequence and see how to get the next equation from it. To get the hang of it, look for example at

 

1 + 2 = 4 - 1.  

 

Our goal with induction is to manipulate this equation to become

 

1 + 2 + 4 = 8 - 1.

 

How can we do that? How about multiplying by 2. What does that do to the equation?

 

2 x (1 + 2)  = 2 x (4 - 1) 

 

We get, 

2 + 4  = 8 - 2.

 

But what we want is 1 + 2 + 4 = 8 -1. So how about adding 1 (after we multiply by 2)? 

 

Doing that yields

 

2 + 4 + 1 = 8 - 1.

 

This is exactly what we wanted. We did it! We moved from the equation for N=1 to the equation for N=2. It is quite an impressive achievement.

 

Did we finish the proof? No. Not exactly, this was just a warm up so that we get the hang of what is going on. But we discovered that "multiply by 2 and then add 1" works well. It brought us from N=1 to N=2. If the same recipe works for general N, brining us from N to N+1 then it will complete the proof.

 

Let's try and do this for the equation of general N (multiply by 2 and then add 1):

 


Now we can distribute the multiplication by 2 and slightly rearrange to get, 


Yes! We did it. We got the general equation for N+1. It looks just like the equation for N, but with N+1 replacing N. This completes the induction proof. We saw that this equation holds for N=1 and then we saw that if it holds for any N then it will hold for N+1. So the goddess of mathematical logic tells us: It holds for all N. That's induction.

 

So the next time you go on a trip armed with a camera, in case you run out of battery, storage or film, just pull out a notepad, sketch some geometric sums as above, and enjoy playing with induction.

 

 

Search Tags:

Algebra

Induction

Mathematics

powers of 2

