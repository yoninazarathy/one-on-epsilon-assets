The full blog post is still accessed through [here](https://www.1onepsilon.com/single-post/2018/07/06/July-2018-Editors-Picks). We are in the process of moving it to the current location.



# Book Reviews: Julia for Data Science
*October 26, 2016*

**Yoni Nazarathy**

Data Science is clearly a hot area, and so is Julia. Maybe you haven’t heard about the programming language Julia? It is a high level dynamic programming language, designed to be both fast and flexible from the start. Fast, means having (almost) comparable performance to C. Flexible, means that it feels like a scripting language (but it is Just-In-Time compiled). Julia has mechanisms and libraries in place to carry out data scientific and numerical tasks similarly to R or Python (NumPy). Indeed, after following the Julia language for the past few months, I am quite convinced that it is a revolutionary tool in scientific computing; it is here to stay.

 

This free open sourced language is in many ways still at its infancy. The current stable release is 0.5 and version 1.0 is still not around the corner. Nevertheless, the large community of Julia developers and users is making quick headway. These include developers from both academia and industry. In fact, at The University of Queensland, where I do research and teach, colleagues and I will be using Julia as the language of choice for a major statistics course taken by 500 mechanical and civil engineering students each year. Similar teaching choices have previously been made by prominent professors in Stanford and other well-known universities. At UQ we decided to follow in their steps. Similarly, at One on Epsilon, Julia will be the language of choice for massive data processing applications that are soon to come. Here too, we are following the steps of more mature companies using and contributing to Julia, such as for example Brisbane’s Fugro-Roames.

 

With Julia gaining such popularity and with Data Science being a hot topic, one can only expect that some literature dealing with Data Science and Julia will pop up, left right and center. This is indeed the case. Two books, both titled, “Julia for Data Science” were recently published:

 

   (1) Julia for Data Science, by Zacharias Voulgaris, Technics Publications, 350 pages, 9/2016, $44.95.​​

 

   (2) Julia for Data Science, by Anshul Joshi, Packt Publishing, 325 pages, 9/2016, $49.99.

 

As you can observe, both books share the same name, a similar price, are released on the same month and are of similar size!

 

I recently obtained these two books as part of preparation for the engineering statistics course, mentioned above. I am also using them as an aid in developing materials for a new Masters of Data Science program that we are launching at The University of Queensland. Having spent time with the books, and since their basic attributes are essentially identical, I decided to write a comparative review contrasting the two books. 

 

Which book should you choose? Is one book better for a specific purpose in comparison to the other? Is one superior? Are they both acceptable and useful?

 

After an extensive reading (including trying out some of the numerical examples from both books), my personal verdict is very clear: Book (1), Julia for Data Science, by Zacharias Voulgaris is clearly a superior choice. It is a useful introduction to both the Julia language and a variety of Data Science tools and methods, mixed with data-driven examples, useful commentary and much insight.

 

As opposed to that, even though it contains some material not present in Book (1), I found Book (2) to be unsatisfactory. It is littered with mistakes and inaccuracies; it is not formatted with care; it does not contain clear data-driven examples; and in many ways, it focuses on insignificant material (for the Data Scientist). Further, it presents that material without any mathematical precision. An illustration of this, is Chapter 4, titled “Deep Dive into Inferential Statistics”. That chapter is merely a pointless description of the Distributions.jl package, spelling out artefacts such as the harmonic mean and the Cauchy distribution. How are these needed and related to Data Science? As an applied probabilist, I actually really like the Cauchy distribution – this is a typical example of a distribution with infinite support and no defined mean. But its inclusion in the book is simply not in place.

 

That example, is just one of many, where I found book 2, to miss the mark by a long shot. Further, the many inaccuracies (even in the sample variance formula of the same chapter) are in my view more than mere typos. Finally, the lack of supporting data sets and examples is a major deficiency. The presentation simply uses a few standard built in data sets in some cases, and generates random examples in other cases. Such a discussion would make sense for a very scientifically precise book. But that level is just not reached.

 

Before departing from Book 2, I should mention a few positive things about it. I did actually learn about the all-important DataFrame in the book’s chapter 2. The book does attempt to present different types of phenomena that occur in clustering in chapter 7, and finally, the discussion of recommendation systems gave me a bit more exposure to the field. Further, the inclusion of time series is blessed (albeit imprecise).

 

In communicating with the book’s author, Anshul Joshi, a seasoned Data Scientist, he mentioned that he may come out with a revision of the book, once Julia version 0.7 (or similar) is released in the future. My recommendation at this point, is to wait for that revision and use Book 1 as a starting point. Nevertheless, I commend Anshul Joshi on taking the initiative to create and publish his book. My personal time spent reading through the book was an important process that made me think about different aspects of Julia and Data Science.

 

So, now focusing on Julia for Data Science by Zacharias Voulgaris (book 1), I summarize my view on this book. I found this an enlightening text, something that I may recommend to students considering studying Data Science on their own. The available on-line data is useful for carrying out the exercises and examples in the book. The way the book introduces Julia is nice. At first, a (rather complex) bare bones implementation of the k Nearest Neighbour, clustering algorithm is presented. I like this, because it exposes the reader to the insides of Data Science algorithms together with Julia code. Only later, in the nicely written Chapters 3 and 4, the author runs the reader through a crash course of Julia fundamentals; types, loops, conditionals and the like. These chapters are neat and tight.

 

Then Chapter 5 is especially nice as it exposes the author’s view on the workflow of a data scientist. Since I have never worked as a data scientist professional myself, I found this reading pleasant and interesting. Indeed, the information that I digested while reading will be useful as I teach my Masters of Data Science students about the inner workings of data scientific linear algebra based algorithms. I could then relate my teaching to real Data Science applications.

 


 

Some inaccuracies and points of dispute are also present (as is always the case). These include some occasional dubious omissions of brackets in code and other minor typos. Of further concern to the statistician is the discussion of Hypotheses testing: Hypotheses are made about the world (or population), not the Data! Indeed, a classic statistician may find some of the interpretations of models and probability in the book disturbing. But frankly, I see these issues as philosophical issues and not practical ones. 

 

The author seems to have planned a clear progression in describing Data Science. Chapters are not split out into categories of algorithms, but are rather moving deeper and deeper into the field. The book touches a variety of methods including principal component analysis (PCA), clustering algorithms, decision trees, regression trees, random forests, neural networks, graphical analysis and much more. All this is augmented with a sensible exposition of elementary descriptive statistics and basic Julia programming while using data examples.

 

So in summary, you will find Julia for Data Science by Zacharias Voulgaris, sitting on my top priority shelf in the coming months. I will recommend it to students that knock on my office door, and I will even occasionally have a further read myself.

 

As for Book 2, I hope to see a future update of the book that attempts to tighten down the details. Indeed there is potential to complement the book of Voulgaris with aspects not covered there.

 

I thank both authors for their books.

Search Tags:

Data Science

Book Review

