The full blog post is still accessed through [here](https://www.1onepsilon.com/single-post/2018/04/27/Can-the-truth-be-tabulated/). We are in the process of moving it to the current location.

# Can the truth be tabulated?

*April 27, 2018*

**Phillip Isaac and Clara Valtorta**


<center>
 <img class = "blog-inline-image" src="https://es-app.com/assets/lglg27.jpg" alt="drawing" width="250px"/>
</center> 


How often during the day do you think about what is true or what is false? What does it mean for a statement to be true? Are some statements more true than others? Think about the last time someone asked you a question. When you responded, was there a clear distinction between a true answer and a false answer?

 

In regular day to day communication, often the issue of true vs. false can become quite a grey area. What about truth in mathematics? In mathematical logic, statements are taken as either true or false. In this post, we consider some examples of circumstances where this thinking can lead to a contradiction. Enter the paradox.

 

A paradox can mean many things in mathematics. Sometimes it refers to a result that is counter-intuitive or unexpected. Other times it refers to a situation that results in an incorrect conclusion because of a subtle error or incorrect assumption made somewhere along the way.

 

Here, we would like to explore a well-known paradox that occurs in the context of mathematical logic known as Curry’s Paradox. Before we delve into Curry’s Paradox, let's consider a simpler logical paradox.

Consider the following statement:

 

This sentence is false.

 

Think about this for a moment. If the sentence is actually false, as it claims to be, then the sentence must be true. Alternatively, if the sentence is true, then the sentence must be false! Hang on, we’re going in circles here! This statement is an example of a logical paradox, that is, a statement that is inconsistent with logic. The paradox arises due to the statement referring to the value of its own truth.

 

In using the word logic here, we mean that every statement is either true or false, but it cannot be both true and false. Furthermore, if a statement is not true, then it is false, and vice versa. 

 

In order to carefully examine and understand Curry’s Paradox, let’s first explore compound statements. A compound statement is one that is made up of two or more statements. Here is an example of a compound statement:

 

It is raining or the kids are playing outside.

 


We can use brackets to separate out the distinct statements.

 

(It is raining) or (the kids are playing outside).

 

Let’s set A to represent the statement “it is raining” and B to represent the statement “the kids are playing outside.” Our sentence is then:

 

A or B.

 

One way to analyze a compound statement is by using a truth table. This is a table that keeps a record of all possibilities of the truth-value of each statement. These values are used to determine the value of the compound statement.

 

There are two possible values for statement A, true or false. There are two possible values of statement B, true or false. The compound statement, "A or B" uses the Boolean operator OR. We can think of it as, "When A and/or B is true, this statement is true." Here is the truth table for "A or B":



Note that the compound statement "A or B" is only false if A and B are both false.

 

Two statements are logically equivalent if their truth tables are the same. It might seem strange at first, but another way of conveying the meaning of that original sentence is the following logical conditional statement:

 

If (not A) then B



Let’s look at this a bit more closely. If “not A” (the hypothesis) is true, then the entire statement can only be true if B (the conclusion) is also true.

 

We must be very clear to take the statement at face value and not interpret anything further than what is being said. The overall statement makes no claim in the case the premise is false. Look at the actual statement again: “If it is not raining then the kids are playing outside.” No claim is being made about where the kids play if it is raining. So, when it is raining, or "not A" is false,  the compound statement is not false, and is therefore true.

 

The situation represented by these logically equivalent statements can be summarized in the following diagram:


Now we can have fun with Curry’s Paradox!

 

We find ourselves in quite a logical mess if we make a statement about that very statement's truth or falsehood in a compound logical statement, especially one with a nonsensical conclusion. Consider:

 

This sentence is false or zero is equal to one.

 

Set C to represent the statement “this sentence is false” and D to represent the statement “zero is equal to one.” The form of the sentence simplifies to:

 

C or D.

 

Looking through our mathematical lens, we produce this truth table as before:



Here is where the logical paradox arises. In rows 1 and 2, C is true. However, C is a statement that refers to its own value. When C is true, this corresponds to saying that the statement “this sentence is false” is true, which means the sentence is false. That is inconsistent with the value in the right-most column. 

 

Something similar occurs in row 4, where C is false. This corresponds to saying that the statement “this sentence is false” is false, which means that the sentence is true. Again, we see in the right-most column, in row 4, that the full sentence is false in this case. So far, it has all been inconsistent.

 

What about row 3? Well, the entries for "C" and "C or D" seem to be logically consistent. Great! What about the entry in the column for "D"? That corresponds to D being true. Unfortunately, that would mean that the statement "zero is equal to one" is true. Eeek! This goes against our broader experience and knowledge, and indeed the foundations of mathematics! So everything is a mess: Indeed, it's a paradox!

 

By the way, another common presentation of this paradox is the conditional statement:

 

If this sentence is true then zero is equal to one.

If you are interested in looking at other types of mathematical paradoxes, check out this video on the Banach-Tarski paradox by VSauce:

 


 

You can also check out the “proof” that pi = 4 by Vihart:

 


Although neither of these are a logical paradox like Curry's Paradox, they demonstrate that mathematics is more than just a set of rules that we follow to make intuitive deductions. There is so much more richness to mathematics!

 

Do you have a favourite mathematical paradox? Is it just impossible to decide? Well, the word “impossible” is not in our vocabulary!

 

 