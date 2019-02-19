# A Formula for the Personality of a Number
*March 25, 2017*

**Yoni Nazarathy**

![Blog header image](https://es-app.com/assets/64anNN.png){.blog-image-header}

What factors make up a person’s personality? This psychological question has intrigued many but I don't think that the answer is simple. Actually, for me, numbers are often simpler to understand than humans, so let me ask the same question about numbers. What is the personality of a positive whole number?
 
Do numbers have personalities? Maybe they do. Clearly $12$ has a softer personality than $17$, doesn’t it? And how about $25$ and $16$? How do they compare?

Assume that you could associate numbers with the personalities of your children. What numbers would you choose? The questions to ask are: How do you describe the personality of a person? How about the personality of a number?

Scientific [investigation of personalities](https://en.wikipedia.org/wiki/Personality_psychology) is a much newer area of research than the investigation of numbers. The following result has been known for [millennia](https://en.wikipedia.org/wiki/Euclid's_Elements):

**A positive whole number can be uniquely written as a product of prime numbers.**

For example,

$$ 
2394 = 2 \times 3 \times 3 \times 7 \times 19.
$$
 

The numbers $2$, $3$, $7$ and $19$ are [prime factors](https://epsilonstream.com/topic/primeFactor) of $2394$, with the factor $3$ appearing twice. If the number $2394$ was a person, what would be its **personality traits**? 

According to our analogy they are $2$, $3$ (going twice), $7$ and $19$. These are the prime factors of $2394$ and in many ways they determine the personality of the number. Just in case you haven't dealt with primes for a while: 

**A [prime number](https://epsilonstream.com/topic/primeNumber) is a whole number greater than $1$ that is not divisible by any other number except for $1$ and itself. For example $2$, $3$ and $19$ are prime, but $9$, $15$ and $24$ are not.**

Go to [see 2394 on numbermatics](https://numbermatics.com/n/2394/). This neat website allows you to enter positive whole numbers and see their prime factorization.

What is the personality of $12$?

$$ 
12 = 2 \times 2 \times 3.
$$

How about $81$?

$$
81 = 3 \times 3 \times 3 \times 3.
$$
 
And how about $101$? You can check that $101$ is prime by seeing that it isn't divisible by any other number. So there is only one personality trait for $101$, and it is $101$ itself. All we can write is $101 = 101$.

---

I don't know much about psychology, but I recently found an interesting list of $638$ [primary personality traits](http://ideonomy.mit.edu/essays/traits.html). These include “*articulate*”, “*daring*”, “*playful*”, “*stubborn*”, “*tolerant*” and many other traits. Since people are more complicated than numbers, psychologists and researchers in the social sciences need to work hard to categorize personality traits. To me, it isn't clear what makes up a personality trait and what doesn't. As I said, I don't know much about psychology.

But with numbers, things are more well defined. It is clear how to see if a number is a personality trait or not. Just check: **is it prime?** Sometimes computing this may take much time. We'll discuss computational aspects of this another day. Here you can find a list of the first $10,000$ primes.

In fact, it is known that there is no limit to the number of personality traits of numbers (primes). These days, mathematics researchers are sometimes trying to discover new huge primes. The [largest known prime](https://en.wikipedia.org/wiki/Largest_known_prime_number) to date has about $22$ million digits. That is quite a personality trait! Any [composite number](https://epsilonstream.com/topic/compositeNumber) that has this prime as a factor must be at least twice as large. 

---

So how does the [prime factorizaton](https://epsilonstream.com/topic/primeFactorization) look for any given number? Can it be described with one neat formula?  Yes, it can! Here is the formula for the **personality of a number**:

$$
n = \prod_{k=1}^m p_k^{a_k}.
$$

The letter $n$ on the left hand side denotes the number and the right hand side describes its personality. The mathematical notation,

$$
\prod \mbox{something}.
$$

implies multiplying $m$ factors of "something", each time recalculating "something" with a different value of $k$. In our case, "something" is a **prime number raised to a power**.

For example, in the case of $2394$, the primes (personalty traits) are

$$
p_1 = 2,
\qquad
p_2 = 3,
\qquad
p_3 = 7,
\qquad
p_4 = 19.
$$

The number of times each of them appears in $2394$ are as follows:

$$
a_1 = 1,
\qquad
a_2 = 2,
\qquad
a_3 = 1,
\qquad
p_4 = 1.
$$
You may wonder if a person needs a very specific personality to understand this formula. I actually think not. Understanding how to read formulas is a straightforward mechanical task, that can be achieved with some basic practice. I think that with the right mindset, everyone can do that. It is just that some personalities are perhaps drawn to formulas more than others. 

---

So we explored prime numbers, personalities and the formula for the personality of a number. This is often called the [fundamental theorem of arithmetic](https://en.wikipedia.org/wiki/Fundamental_theorem_of_arithmetic). Children aged 10-14 typically come across this concept when learning how to factorize numbers. Perhaps try to engage your children with discussion about personalities and numbers. You might discover some of their prime factors as you go.

