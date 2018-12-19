# Is it Divisible by 3?
*January 15, 2017*


**Yoni Nazarathy**

![Blog header image](https://es-app.com/assets/7fnxAN.png){.blog-image-header}

I am the father of three kids, hence for me division by three is an integral part of life. A pack of 12 water balloons is divisible by three. A pack of 30 works well too. But get a pack of 16 and you are left with a remainder of 1 and a philosophical debate about who deserves it.

 

For parents with 2 kids, things are typically simpler. Even numbers are divisible by 2 and odd numbers are not. But if you are into 3's, how to know if a whole number is divisible by 3? Is there some simple rule or pattern?

 

Well, there is a good chance that your child has been taught this at school. Maybe you even remember this “trick” back from the days. It goes as follows: Add up the individual digits of the number and see if the sum of the digits is divisible by three. If the sum of the digits is divisible by 3 then so is the original number. Otherwise, it isn’t. The trick also works similarly for 9, but we’ll focus on 3 here. Nine kids with water baloons - too much to handle!

 

Here is an example: Take 264. The sum of the digits is 2+6+4 = 12. Now 12 is divisible by 3 and this implies that 264 is divisible by 3. In fact, 264 = 88*3. Similarly, take 301. The sum of the digits is 3+0+1 = 4. This is not divisible by 3 and hence neither is 301. Try to divide it by 3 and you’ll get a non-whole number or a remainder.

 

Well, that’s the trick. You can even use it recursively if you really wish. For example, on the noon of January 15, 2017 (Beijing time) the population of China was estimated to be at 1,382,765,241 (almost 1.4 billion people). Is this exact number divisible by 3? Well the sum of the digits is,

 

1+3+8+2+7+6+5+2+4+1 = 39.

 

And this translates the question to: “is 39 divisible by 3”? Well, you probably see immediately that yes, but to answer this you can also look at 3+9=12. And then to see if 12 is divisible by 3, you can even look at 1+2=3 and yes it is. Hence since 3 is divisible by 3, 12 is divisible by 3 and hence 39 is divisible by 3 and hence the population of china (estimate of that exact time) is divisible by 3. This recursion is more of an academic exercise, because you already saw that 39=3*13 is divisible by 3.

 

Ok, so that was the “trick”, a “math trick”. But frankly, us mathematicians are often weary of using the word trick because we like to understand the deeper meaning behind things. In fact, we would often like to see a proof that this trick actually works for any number. Sure, we can check it on the number 264, the number 301 and the population of China, but how to know that it always works?

 

So here is a simple explanation: Look at the number 264 as an example.

 

264 = 2*100 + 6*10 + 4.

 

Right? This is what we mean when we write the number 264 (in base 10 as we usually do). This can also be done for the population of China, where the leading term would be, 1*10^9 (that reads as "10 to the power 9" i.e. a billion), the second term is 3*10^8, the third term is 8*10^7 and so fourth. 

 

Going back to the 264 example, we can now represent 100 as 99+1 and 10 as 9+1 hence,

 

264 = 2*(99+1) + 6*(9+1) + 4.

 

Now comes the fact that 2*(99+1) = 2*99+2*1. This is called the “distributive property”. That is,

 

A*(B+C) = A*B+A*C,

 

where we notice that the order of operations is to first perform A*B and A*C and only later to do the plus between these terms. Hence,

 

264 = 2*99 + 2 + 6*9 + 6 + 4.

 

We can now reorder this to,

 

264 = 2*99+6*9 + (2+6+4).

 

Now observe that the last bit above, (2+6+4), is actually the sum of the digits, hence we got,

 

264 = 2*99 + 6*9 + sum of digits.

 

The terms, 2*99 and 6*9 are always divisible by 3,  because 99 and 9 are always divisible by 3. Now assume that the sum of the digits is divisible by 3 (as it is in the case of 2+6+4). Then all terms on the right hand side are divisible by 3 and then 264 is divisible by 3. That is why the rule worked for 264.

 

Let’s try it on the number 2,324.

 

2324 = 2*(999+1) + 3*(99+1) + 2*(9+1) + 4

           = 2*999 + 3*99 + 2*9 + sum of digits.

 

Now the sum of the digits is 2+3+2+4 = 11 and is not divisible by 3. But the first bit, 2*999 + 3*99 + 2*9 is divisible by 3. So this means that,

 

2324 =  something divisible by 3 + something not divisible by 3.

 

Hence, 2324 is not divisible by 3.

 

The above is the basis for the proof of this divisibility by 3 rule. There is a very good chance that your kids, when aged 8-13 are taught this in school. But when taught it, the teacher often doesn't risk explaining where the rule comes from. It is left as a "trick".

 

If you had the patience to read all the way down to here, then maybe you can further take the time and work out these details, together with your children. Nurture your connection with them and drive their curiosity about the source of such mathematical tricks and others.

Search Tags:

Numbers

