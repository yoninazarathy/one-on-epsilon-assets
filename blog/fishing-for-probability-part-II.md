The full blog post is still accessed through [here](https://www.1onepsilon.com/single-post/2016/10/31/Fishing-for-Probability-Part-II/). We are in the process of moving it to the current location.

# Fishing for Probability, Part II
*October 31, 2016*


**Yoni Nazarathy**

Ok, so you may have read the previous post describing the following situation: You are fishing exactly 3 fish. This is from a tiny lake with 7 fish in total, 3 of which are gold and 4 of which are grey. The random quantity X, denotes the number of gold fish that come out. These are the possibilities for X:

 

X = 0, you come out with 0 gold fish (and 3 grey). 

X = 1, you come out with 1 gold fish (and 2 grey fish).

X = 2, you come out with 2 gold fish (and 1 grey fish).

X = 3, you come out with 3 gold fish (and 0 grey fish).

 

In this situation the following holds:

 

(A) It is more likely to have all grey fish (X = 0) in comparison to all gold fish (X = 3).

 

(B) An outcome of X = 1 is more likely than X = 2.

 

Both (A) and (B) come from the fact that there are more grey fish than gold fish. Your kids would understand that too if you ask them to think about it.

 

Did you and/or your children try and guess probabilities? Even though there is no immediate "easy way" to get the exact numbers, I've previously observed that children guess numbers that are not too way off.

 

Here are the actual exact probabilities:

 

The probability of X = 0 is 4/35 =11.4%

The probability of X = 1 is 18/35 = 51.4%

The probability of X = 2 is 12/35 = 34.3%

The probability of X = 3 is 1/35 = 2.9% 

 

Do these agree with (A) and (B) above?

 

Observe that there is only about 3% chance of coming out with all gold fish. As opposed to that there is a roughly 50% chance of getting exactly 1 gold fish.

 

You may ask what I mean by "exactly". After all, there is nothing exact about this process of fishing. Well, "exact" does not refer to the outcome of X - this is indeed a random quantity. But what is made exact is the calculation of the probabilities associated with X. We use a mathematical model to describe the probability of each possible outcome.

 

Mmmm....  "a mathematical model"?  Yes, here is a very sensible model for such a scenario: Without further detailed knowledge about how these fish swim inside the lake and go for bait, the most sensible assumption is that at any given time, if there are Z fish in the lake, then the chance of each of them catching the bate is 1/Z. For example if there are Z = 5 fish in the lake at a given time, then there is an equal chance of 0.2 for catching each one. Sensible no? Our model further assumes that any fish catch at any time does not affect other events (this is sometimes called independence).


How do we then compute the probabilities of each of the outcomes of X? One way to do this is to give each fish a name or a label (e.g. 1,2,...,7). Then with each fish uniquely labeled, we count the number of possibilities for selecting 3 fish out of the 7 fish. How many such possibilities are there? Well, it turns out there are 35. Here they are: 

 {1, 2, 3}, {1, 2, 4}, {1, 2, 5}, {1, 2, 6}, {1, 2, 7},

 {1, 3, 4}, {1, 3, 5}, {1, 3, 6}, {1, 3, 7}, {1, 4, 5},

 {1, 4, 6}, {1, 4, 7}, {1, 5, 6}, {1, 5, 7}, {1, 6, 7},

  {2, 3, 4}, {2, 3, 5}, {2, 3, 6}, {2, 3, 7}, {2, 4, 5},

  {2, 4, 6}, {2, 4, 7}, {2, 5, 6}, {2, 5, 7}, {2, 6, 7},

 {3, 4, 5}, {3, 4, 6}, {3, 4, 7}, {3, 5, 6}, {3, 5, 7},

{3, 6, 7}, {4, 5, 6}, {4, 5, 7}, {4, 6, 7}, {5, 6, 7}.

 

Would you like to challenge your child to write out all 35 possibilities of selecting 3 unique fish names? Frankly, I'm not sure that it is the best thing for helping them connect to math. But still you may consider giving some simpler enumerations for them to do. My eldest has done such enumeration exercises before and found it relaxing.

 

Getting the number 35 is a matter of combinatorics. The way it is computed is by computing 7!/(4! x 3!). What's with the exclamation marks you ask? Well, these are factorials. For example,

 

4! = 4 x 3 x 2 x 1 = 24.

 

We won't describe how factorials play a role here. Instead, I'll leave it to another blog post. But keep in mind, that asking your kids to calculate 3!, 4!, 5!, 6!, up to say 7! = 5,040 can be an engaging activity. But don't go crazy and ask your child to compute 

 

50! = 30414093201713378043612608166064768844377641568960512000000000000.

 

Most kids find it a bit too exhausting and you are bound to run into some resistance.

 

OK, so there are 35 possible fish sets. Now assume that the fish labeled 1, 2, 3 are gold and the fish labeled 4, 5, 6, 7 are grey. Fishing out, for example, the fish set {1, 2, 3} would imply we got all gold fish. That would mean X = 3. Are there other fish sets that would make X = 3? No! Hence:  The probability of X = 3 is 1/35 = 2.9%. This is because there is only one possible outcome out of the 35 outcomes that would yield X = 3.

 

Try calculating now the probability of X = 0? What sets of fish will yield X = 0? There are four such possibilities right? Hence: The probability of X = 0 is 4/35 =11.4%.

 

Calculating the probabilities of X = 1 and X = 2 follow in the same manner. But the counting is slightly delicate and tedious. A systematic way for calculating the numerator of the probability of having X = k is by the formula (3!/((3-k)! x k!)) x (4!/((k+1)! x (3-k)!)). Again, understanding the derivation of such a formula would require more understanding of combinatorics and we'll leave that for a different day. Nevertheless, I have previously engaged with 10 year old kids in using this formula. This you can do with your kids too.

 

I'd like to also encourage you to try this fishing experiment at home with your kids: Put a bucket with 7 balls, 3 of which are gold and 4 of which grey (you can obviously go for other object types and colors). Have your child pull out 3 balls blindly. That is always fun!

 

Repeat this 10 times. What kind of results do you expect? Well, it would take an average of 35 attempts to get all gold! Maybe your kids will do it in less, maybe in more. That is now a matter of luck both for your kids and for the fish.

 

 

Search Tags:

Probability

