The full blog post is still accessed through [here](https://www.1onepsilon.com/single-post/2017/04/07/Guessing-in-Multiple-Choice-Exams---Part-I). We are in the process of moving it to the current location.

# Guessing in Multiple Choice Exams

*April 7, 2017*

**Yoni Nazarathy**

![Blog header image](https://es-app.com/assets/32uic2.png){.blog-image-header}

Say you are taking a multiple choice exam. There are 20 questions, each one with four possible answers (a), (b), (c) or (d), one of which is correct. You are feeling lucky and hence don't read the questions. Instead you are guessing random answers. How bad can that be?

 

Frankly, years ago at high school, this was my typical mode of operation. I wasn't too keen on studies, could not concentrate and often felt frustrated at exams. So I thought that by guessing, I will end up doing not so bad. After all, the goddess of chance may make it possible to get all answers correct.

 

Only years later, I realized that the chance of actually passing such an exam, by getting a result of 11/20 or better, is very low. Theoretically it actually stands at about 0.00394. That means that only about one out of 254 exams is going to be a passing exam. Hence by guessing, I was actually almost guaranteed to fail. In fact, it is practically impossible to guess all answers correctly.

---

Let's understand this a bit better.

 

Q: What is the chance of guessing the answer for a single question correctly?

A: There are four options for each question, so the chance is 1/4 = 0.25.

 

Q: So on average, how many questions can I expect to get correctly in the whole exam?

A: There are 20 questions, and on average 1/4 of the questions will be answered correctly. So on average, the number of correct answers is 1/4 of 20. That is 5.

 

Q: But surely it is possible to get more than 5 questions correct. For example, what is the chance of getting all 20 correct?

A: Here getting all 20 correct requires success in the first question, the second question, the third,... all the way up to the last question. The chance of each such success is 1/4. Since our guesses don't affect each other, the chance for success in all 20 is

FORMULA

As you may imagine, this is actually an incredibly small number. It equals about 10^(-12) or 0.000000000001.

 

To help you interpret such a low probability, try and guess the answer to this question:

 

If you were filling out a random exam solution every 30 seconds and having it automatically checked, what is the expected (average) time until you fill out a perfect exam?

 

Answer options (select one):

 

(a) 60 seconds.

(b) 20 years.

(c) 250 years.

(d) One million years.

Did you try and make an educated guess for the correct answer?

 

Solution: Say you can fill out an exam in 30 seconds. So in a sleepless day, you can fill out 2 x 60 x 24 = 2,880 exams. Then multiplying by 365, in a year you can fill out 1,051,200 exams. This is about a million exams a year. Sounds fun! Now the number of exams you need to do on average until filling one out with all questions correct is 10^12 (a trillion). This means you'll need to work for about 10^12/10^6 = 10^6 years, or about a million years until acing your first exam.

 

Of course you may be lucky and ace an exam before a million years pass. But don't forget that we didn't take sleep into consideration, so at the minimum you'll need quite a few coffee breaks and those will slow you down. Alternatively with some study and if you choose to read the questions and make more educated guesses, you may increase the chance of success in each question from 1/4 to 1/2, 0.8, 0.9 or even 0.99.

 

Perhaps try to repeat the calculation for a chance of success per question of 0.9. In that case, what is the chance of succeeding in all questions?

---

Back to guessing? Here are more facts about the exam.

 

Q: Is the chance of getting all answers wrong the same as the chance of getting all answers correct?

A: Here similar reasoning shows that failing at all 20 questions happens with a chance of (3/4)^20. This is also a small number, but certainly not as small as (1/4)^20. It stands at about 0.00317. On a positive note this means that there is a chance of 1 - 0.00317 = 0.99683 (almost certain) of getting at least one question correct. 

Perhaps take a moment for this fact:

 

The chance of failing at all 20 questions (317 out of 10,000) is very similar to the chance of passing the exam with 11 or more correct answers (394 out of 10,000). 

 

Q: So how do you calculate the chance of passing (getting 11 or more correct answers out of 20)? 

A: This is actually not as simple as the other calculations we carried out. It isn't overly complicated, but requires using something called the Binomial Distribution.

 

As a start, you can visit this Binomial Calculator on Stat Trek. On that page, key in 0.25 for "Probability of success in a single trial", 20 for "Number of trials" and 11 for "Number of successes". You'll then see resulting probabilities associated with our exact problem. Do you spot the chance of passing the exam, 0.00394?

 

We'll discuss the details of this binomial calculation in a future blog post. In the meantime, if anyone around you is studying for an exam, nurture your connection with them by helping them enjoy the learning process.

 

It is actually important to remember that grades are not all that matters. The knowledge acquisition process is often much more important. Maybe ask the goddess of chance, Fortuna, what she thinks.

IMAGE