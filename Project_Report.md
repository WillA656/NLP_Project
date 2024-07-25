
**NLP PROJECT CLOUD COMPUTING**
Will Antink and Spencer Veatch

**INTRODUCTION**

This report seeks to determine whether or not there exists a statistically significant difference in the subject and object frequencies for feminine and masculine personal pronouns. To begin with, we had to determine what corpus of text to perform our analysis on. We decided to use the top ten most popular fiction novels from Project Gutenberg. We felt that this was the best source of data as it was easy to access and came to us as simple text files. We felt that a larger corpus was necessary to have more statistically valid conclusions, and that ten novels would be a sufficient amount of text.

**HYPOTHESIS**
We hypothesize that there will be a significant difference between subject and object frequencies for feminine and masculine personal pronouns within a given corpus. Primarily, that there will be more male pronouns than female pronouns. We believe this to be the case for our particular data, as the most popular works of fiction on Project Gutenberg are all fairly old, and that literature from 100+ years ago typically featured more male characters, and often had them speaking more than their female peers. One caveat with our data is that we do have an equal balance of male and female authors, which may end up with more balanced frequencies. It is important to address here that the corpus we are working with is a collection of ten books all by different authors, and might differ substantially from a work written by only a single author.

If our statistical test of choice indicates within a reasonable amount of certainty (<0.05 p-value for instance) that our hypothesis is supported, we will accept it as likely.

**METHODOLOGY**
We are defining statistical significance as a p-value of less than 0.05 resulting from our hypothesis test. Our corpus consists of ten novels pulled from Project Gutenberg. We utilized an API called Gutendex to query the top ten most popular fantasy novels on the platform and get links to the text of each work. From there, we added the links of all ten works to a text file in github and used bash methods in a colab document to curl each of the text files and assign new names to them. After that, it was only a matter of putting all of the books together in a single large text file we called corpus.txt.

Initially, we had concerns that our data might be polluted by the extra text added to each book by Project Gutenberg. There is a section before the start of each book that lists some basic information such as title and author, as well as a lengthy disclaimer from Project Gutenberg on the use of the books. We were worried that this extraneous text might influence our analysis, but on further inspection realized it contained few to no pronouns, which is really all we were interested in.

There were a number of methods at our disposal, and we felt that a chi-squared test was the simplest and most vaiable method of determining whether or not there was a statistically significant difference between the frequencies of these gendered pronouns in our given corpus. The test itself requires little more than count data, and the results are easy to both apply and interperet.
--Results of our analysis

**EVALUATION**
--Explain results
--Assess hypothesis validity
